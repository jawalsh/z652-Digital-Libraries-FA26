# Week 10: Image Objects II: Image Processing, IIIF, and Interoperability

## Summary

Last week we examined the technical characteristics of digital images and the reasons libraries create different files for preservation and access. This week we turn to **image processing and delivery**: how institutions prepare images for publication, automate repetitive operations, and provide access to very large images.

We will introduce batch-processing workflows and tools such as **ImageMagick**, then explore the **International Image Interoperability Framework (IIIF)**. We will connect image servers, viewers, APIs, and persistent identifiers to the enterprise digital library architectures discussed in Week 8.

## Weekly Learning Objectives

By the end of this week, you should be able to:

- *describe* resizing, cropping, format conversion, and derivative generation.
- *explain* the advantages of batch processing and reproducible workflows.
- *perform* or interpret basic image-processing operations using ImageMagick.
- *explain* the purpose of IIIF and the basic roles of its Image and Presentation APIs.
- *distinguish* an image server from an image viewer.
- *describe* how APIs and persistent identifiers support interoperability.
- *evaluate* appropriate image delivery approaches for a small digital collection.

# Before Class

## Readings and Resources

### Required: Technologies and Interoperability

Read:

- Banerjee, Kyle, and Terry Reese Jr. *Building Digital Libraries*, 2nd ed. (2019), **Chapter 5, “General Purpose Technologies Useful for Digital Repositories,”** and **Chapter 7, “Sharing Data: Harvesting, Linking, and Distribution.”** Available through [IUCAT eBook](https://iucat.iu.edu/catalog/19362782). Focus especially on sections relevant to APIs, exchanging digital content and metadata, and interoperability; detailed implementation examples are optional.
- IIIF Consortium, [**How IIIF Works**](https://iiif.io/get-started/how-iiif-works/). Focus on image servers, viewers, and the roles of the Image API and Presentation API.

### Preparation: Image Processing

Browse:

- [ImageMagick](https://imagemagick.org/).
- [ImageMagick Command-Line Processing](https://imagemagick.org/script/command-line-processing.php).

Find examples of resizing, cropping, and format conversion. Treat these pages as references for the in-class activity, not material to memorize.

### Optional Background and References

- Witten, Ian H., David Bainbridge, and David M. Nichols. *How to Build a Digital Library* (2010), **Chapter 7, §7.4**, for background on web services. [IUCAT access](https://kg6ek7cq2b.search.serialssolutions.com/?V=1.0&L=KG6EK7CQ2B&S=JCs&C=TC0000298940&T=marc).
- [IIIF introductory training materials](https://training.iiif.io/intro-to-iiif/index.html).
- [IIIF Image API](https://iiif.io/api/image/3.0/) and [Presentation API](https://iiif.io/api/presentation/3.0/) — specifications for reference only.
- [Mirador](https://projectmirador.org/) (viewer) and [Cantaloupe](https://cantaloupe-project.github.io/) (image server).

## Tasks

### 1. Plan an image transformation

Choose an image from your project or a sample collection. Consider:

- Does it need resizing, cropping, rotation, or format conversion?
- Which file should be retained as a preservation master?
- What derivative would be appropriate for web access?
- How would you document the transformation?

### 2. Explore a IIIF viewer

Explore [Mirador](https://projectmirador.org/) or a digital collection with a IIIF viewer. Look for zooming, panning, multiple-image display, and sharing features. Come prepared to compare this experience with viewing an ordinary JPEG on a website.

# In Class

## Topics

- Preservation masters and access derivatives (review)
- Resizing, cropping, and format conversion
- ImageMagick and batch processing
- Reproducible image workflows
- IIIF architecture and use cases
- IIIF Image API and Presentation API
- Image servers and viewers: Cantaloupe and Mirador
- APIs, persistent identifiers, and interoperability
- CollectionBuilder and image delivery

## Hands-on Activity: Image Processing

Using sample images, we will:

1. Inspect dimensions and formats.
2. Create a resized access derivative.
3. Convert an image to another format.
4. Compare file sizes and visual results.
5. Document the transformations performed.

## IIIF Demonstration

We will examine a IIIF-enabled image and trace the roles of the source image, image server, API requests, and viewer. The goal is to understand the workflow, **not** to deploy an image server.

## Discussion

- Why automate image processing rather than editing each image separately?
- How is a IIIF image server different from a folder of JPEGs?
- What can institutions accomplish through shared APIs?
- When is CollectionBuilder's simpler approach sufficient?

## Looking Ahead

Next week we turn to **text objects**, beginning with XML, markup, and the Text Encoding Initiative (TEI). As with images, we will consider how the structure and representation of digital objects affect their discovery, preservation, and use.
