# OCR Lab

In this lab, you will use optical character recognition (OCR) to produce machine-readable text from page images. You will compare tools, examine recognition errors, and consider how the characteristics of a source affect the usefulness of the resulting text.

## Tools

Use both:

- **Adobe Acrobat Pro**
- **Tesseract**

Optionally, try an online OCR service as a third comparison. Use only the supplied samples or other material appropriate for uploading to an external service; do not upload private or sensitive documents.

## Sample Images

Perform OCR on each of the following:

- [Swinburne. _Poems_. 1904.](images/swinburne_sm.jpg)
- [“Kid Colt’s Roundup” (fan mail).](images/kid_colt_sm.jpg) _Kid Colt Outlaw_ #122. May 1965.
- [William Carlos Williams. _Pictures from Brueghel_. Manuscript](images/williams_sm.jpg). From  [YCAL MSS 116. Beinecke Rare Book and Manuscript Library, Yale University](https://collections.library.yale.edu/catalog/2003526).

If you have scans of textual content for your final project, try one or more of your own images as well.

## Procedure

### 1. Inspect the Images

Before running OCR, examine each image. What might make its text easy or difficult to recognize?

Consider:

- image clarity, contrast, and orientation;
- typeface, type size, and handwriting;
- columns, illustrations, and other layout features;
- unusual spelling, punctuation, or characters.

### 2. Run OCR

Process each image with Acrobat and Tesseract.

For Tesseract, a basic command is:

`tesseract input.tif output -l eng`

Replace `input.tif` with your image’s filename. Tesseract will create `output.txt`; the second argument supplies the output filename without its extension.

Use distinct output names for each image and tool. Retain the original images and the recognized text.

Record the tools and settings you use, including any language or page-layout settings you change.

### 3. Compare the Results

For each image, select the same short passage—approximately 50–100 words, or the available text if shorter—and compare each tool’s output with the image.

Look for:

- incorrect, missing, or inserted characters and words;
- punctuation and capitalization errors;
- problems with line breaks and hyphenated words;
- omitted text or text recognized from illustrations;
- incorrect reading order, especially across columns;
- loss of meaningful formatting or structure.

Record a few specific examples. Include both successful recognition and errors.

Open the Tesseract text files in VS Code and inspect their character encoding. If unusual characters appear, investigate whether they are present in the OCR output or result from interpreting the file with the wrong encoding.

### 4. Evaluate Usefulness

Consider the results for different purposes:

- Would this text support useful keyword searching?
- Could someone read it comfortably without consulting the image?
- What correction or restructuring would it need for accessible reading?
- Could errors distort computational analysis?
- What work would remain before encoding the text in TEI?

Choose one problematic image and try one adjustment, such as cropping a text region, correcting its orientation, or changing an OCR layout setting. Compare the new result with the original output.

## Submission

In Canvas, submit:

1. **A brief comparison table:** one row per sample image, identifying its main challenges and the relative strengths and weaknesses of Acrobat and Tesseract.
2. **Two or three paragraphs:** explain the most significant differences, include specific error examples, describe the adjustment you tried, and assess whether the results would be sufficient for keyword searching or would require further correction.
3. **The Tesseract `.txt` output files** for the three supplied images.

If you tested an image from your final project, briefly explain what you learned about processing that material.

You are evaluating the OCR output; you do not need to correct all of it.