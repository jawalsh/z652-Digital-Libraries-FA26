# Activity: Introduction to APIs Using IIIF

**Z652 Digital Libraries — Week 10: Image Objects II**  
**Time:** 20–25 minutes (plus optional extension)  
**Materials:** Web browser and Google Sheets

> **Adaptation and attribution:** Adapted and updated from Owen Stephens, *Introduction to APIs using IIIF* (June 13, 2016), developed on behalf of the British Library. Original work licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/). **Developed by Owen Stephens on behalf of the British Library.** This adaptation updates the activity for the [IIIF Image API 3.0](https://iiif.io/api/image/3.0/), uses HTTPS, and adds a short image-information exercise. [Original activity](https://www.meanboyfriend.com/overdue_ideas/2016/06/introduction-to-apis-using-iiif/).

## Learning goals

By the end of the activity, you should be able to:

- Explain an API request and response using a concrete example.
- Construct a IIIF Image API URL from separate parameters.
- Request different representations of an image by changing URL parameters.
- Distinguish an image response from an image-information (`info.json`) response.
- Explain how requesting a derivative from an image server differs from creating one in advance with ImageMagick.

## 1. Understand the request

An **API** defines how software can make requests and receive responses. The [IIIF Image API](https://iiif.io/api/image/3.0/) lets a client request an image, or a modified representation of it, from a compatible image server.

An Image API 3.0 request generally looks like this:

```text
{base-URI}/{identifier}/{region}/{size}/{rotation}/{quality}.{format}
```

| Part | Purpose | Example |
|---|---|---|
| Base URI and identifier | Identify the image service and image | Supplied below |
| Region | Entire image or a selected portion | `full` |
| Size | Requested dimensions | `600,` (600 pixels wide) |
| Rotation | Rotation in degrees; `!` requests mirroring | `0` |
| Quality | Image representation | `default` |
| Format | Output file format | `jpg` |

**Important:** IIIF defines the syntax, but individual servers may not support every optional transformation. If a request fails, try a simpler value and consult the image service's `info.json`.

## 2. Build a request in Google Sheets

Create a **blank Google spreadsheet**. In column A enter the labels below; in column B enter the corresponding values. The example uses a IIIF Image API 3.0 image service from Princeton University Art Museum. **Before class, the instructor should test the endpoint and the specific transformations below; remote services can change.**

| Cell | Column A: label | Column B: value |
|---|---|---|
| B1 | Base image URI | `https://media.artmuseum.princeton.edu/iiif/3/collection/y1982-103` |
| B2 | Region | `full` |
| B3 | Size | `600,` |
| B4 | Rotation | `0` |
| B5 | Quality | `default` |
| B6 | Format | `jpg` |
| B7 | Constructed URL | Formula below |
| B8 | Returned image | Formula below |

In **B7**, enter:

```excel
=CONCATENATE(B1,"/",B2,"/",B3,"/",B4,"/",B5,".",B6)
```

In **B8**, enter:

```excel
=IMAGE(B7,3)
```

You have constructed a URL from separate parameters and asked Google Sheets to retrieve the image returned by that URL. If the image does not appear, open the URL in B7 in a browser to determine whether the image server returns an image or an error. Some image servers may reject requests from Google Sheets even when their URLs work in a browser.

**Questions:** Which parts of this URL identify the source image? Which parts tell the server how to transform the response? What is the response to this request?

## 3. Experiment with the parameters

Change **one parameter at a time**, observe the result, and record what happened.

1. **Resize:** Change B3 from `600,` to `200,`, then to `800,`. What changes? What remains the same? Restore `600,`.
2. **Rotate:** Change B4 from `0` to `90`, then `180`. What happens? Restore `0`.
3. **Mirror:** Try `!0` in B4. Does the server return a mirrored image? Restore `0`.
4. **Crop:** Change B2 from `full` to `pct:25,25,50,50` to request the central half of the image by width and height. What part of the original do you see? Restore `full`.
5. **Optional:** Try B5 = `gray`. Does the service support grayscale output? Restore `default`.

**Record:** At least two parameter changes, the resulting URL, what you expected, and what actually happened. A failed request is also evidence: note the response or error rather than assuming every server implements every option.

## 4. Request information about the image

Open this URL in a new browser tab:

[Princeton IIIF image information (`info.json`)](https://media.artmuseum.princeton.edu/iiif/3/collection/y1982-103/info.json)

An image request returns image data. An **Image Information Request** returns JSON describing the image service and the image, including dimensions and potentially supported features.

Find the following, if present:

- The image's `width` and `height`.
- Its `id` (the image service URI).
- Its `type` and `protocol`.
- Any `profile`, `sizes`, or `tiles` information.

**Discuss:** Why would a viewer need to obtain this information before deciding what image requests to make? Why might an image server provide tiled images instead of sending the entire original file?

## 5. Connect the exercise to ImageMagick and CollectionBuilder

Earlier, you created JPEG access images and 200-pixel thumbnails with ImageMagick. Compare that workflow with IIIF:

| ImageMagick workflow | IIIF Image API workflow |
|---|---|
| Create derivative files ahead of time | Request representations from a server when needed |
| Store and publish access JPEGs and thumbnails | Server may generate or retrieve appropriately sized images |
| Simple to deploy on a static site | Requires access to a compatible image service |
| Appropriate for many small CollectionBuilder projects | Useful for zooming, large images, shared viewers, and interoperable access |

**In pairs, answer:** Would your final CollectionBuilder collection benefit from IIIF, or are pre-generated derivatives sufficient? Give one concrete reason.

## Optional extension: explore a second image

Find another IIIF Image API service through a digital collection or the [IIIF examples](https://iiif.io/api/image/3.0/#examples). Replace the base image URI in B1, leaving your formulas unchanged. Does the same spreadsheet work? Which transformations differ?

For multi-page objects, a **IIIF Presentation API** manifest can describe canvases, sequences, metadata, and image services. The Image API by itself transforms an identified image; it does not define a book's page order. Explore the [Presentation API 3.0](https://iiif.io/api/presentation/3.0/) if you want to investigate how viewers navigate complex objects.

## Exit question

In two or three sentences, explain what you learned about **APIs**, **image derivatives**, and **interoperability** from constructing and modifying the URL.

---

### Instructor notes (remove from student handout if desired)

- Allow about **3 minutes** for the introduction, **5 minutes** for constructing the spreadsheet, **7–8 minutes** for experimentation, **4 minutes** for `info.json`, and **3–5 minutes** for the CollectionBuilder discussion.
- Check the Princeton image endpoint immediately before class, including rotation, mirroring, cropping, and Google Sheets `IMAGE()` access. Its use here is an example, **not a guarantee of current availability**.
- If the service is unavailable, substitute a verified IIIF Image API 3.0 base image URI; the spreadsheet formulas and activity sequence remain the same.
- If the returned image is visually too large in the spreadsheet, resize row 8 and column B. Google Sheets may also cache images; opening the generated URL in a browser helps verify the actual response.
- The central distinction to emphasize: **the Image API returns representations of an individual image; the Presentation API describes structured digital objects and their associated resources.**
