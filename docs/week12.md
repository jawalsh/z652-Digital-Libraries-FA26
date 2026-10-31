# Week 12: Text Objects 2 (of 2): OCR, Character Encoding, and Text Digitization

## Summary

Last week, we explored how XML and TEI represent the structure and meaning of texts. This week, we examine how text becomes machine-readable in the first place: how we move from images of printed pages to text that can be searched, copied, processed, and encoded.

We will introduce optical character recognition (OCR), examine factors that affect its accuracy, and use Tesseract to recognize text in page images. We will also explore character encoding, distinguishing ASCII, Unicode, and UTF-8 and considering what happens when software interprets an encoding incorrectly.

Throughout the week, we will connect technical choices to the purposes and audiences of a digital collection. How accurate does recognized text need to be for searching, reading, accessibility, or computational analysis? What requires human review? What files and documentation should a text digitization workflow produce and retain?

## Weekly Learning Objectives

- _distinguish_ among page images, plain text, and structured text, and _explain_ what each representation supports
- _explain_ the relationships among characters, Unicode code points, and character encodings such as UTF-8
- _recognize_ common symptoms of character-encoding problems
- _use_ Tesseract to perform OCR on image files
- _evaluate_ OCR output against source images and _identify_ errors involving characters, words, layout, and reading order
- _explain_ how image quality, typography, page layout, and language affect OCR results
- _outline_ a text digitization workflow that includes quality control, metadata, access, and preservation

## Before Class: Readings, Resources, and Tasks

### Required Readings

- Willett, P. (2004). [“Electronic Texts: Audiences and Purposes.”](https://companions.digitalhumanities.org/DH/?chapter=content%2F9781405103213_chapter_18.html) In _A Companion to Digital Humanities_.
  - Focus on how different audiences and purposes shape the creation and use of electronic texts. Consider which distinctions remain useful despite changes in technology.
- W3C. [“Choosing & Applying a Character Encoding.”](https://www.w3.org/International/questions/qa-choosing-encodings.en)
  - Focus on what a character encoding does, why UTF-8 is recommended, and why software needs to know a document’s encoding.

### Recommended Reading

- Witten, Ch. 3, pp. 73–86, and Ch. 4, pp. 127–152.
  - Use these selections for additional background on digitization and text processing.

### Software Preparation

- **Install Tesseract.**
  - **macOS:** If you already have [Homebrew](https://brew.sh/), run `brew install tesseract`. If necessary, install Homebrew first using the instructions on its website.
  - **Windows:** Follow the installation guidance linked from the [Tesseract documentation](https://tesseract-ocr.github.io/tessdoc/Installation.html), which directs Windows users to the UB Mannheim installer.
  - Open Terminal on macOS or PowerShell on Windows and run `tesseract --version` to confirm that the command is available.
  - If installation fails or the command is not recognized, record the error message and bring it to class.
- **Install or update Adobe Acrobat Pro** through [IUware](https://iuware.iu.edu/) for comparison with Tesseract.
- Bring a laptop with **VS Code** available for inspecting OCR output and character encodings.

### Questions to Consider

- Is a scanned page necessarily searchable or accessible?
- When might imperfect OCR still be useful?
- When would errors make recognized text unsuitable for its intended purpose?
- How does character encoding differ from the XML/TEI markup we studied last week?

## In Class

### Character Encoding: From Characters to Bytes

- ASCII, Unicode, and UTF-8
- Characters, code points, and their representation as bytes
- Accented characters, non-Latin scripts, and other characters beyond ASCII
- Recognizing and investigating incorrectly decoded text
- Inspecting character encodings in a text editor
- Distinguishing character encoding from structural markup

### OCR: From Page Images to Machine-Readable Text

- What OCR produces and what it does not recover automatically
- Effects of resolution, skew, contrast, typography, language, and page layout
- Character recognition versus layout analysis and reading order
- Plain-text output, searchable PDFs, and output that retains page coordinates
- OCR errors and their consequences for discovery, reading, accessibility, and analysis

### Hands-On OCR Lab

- [OCR exercise](assignment_ocr_exercise.md)
- Run Tesseract on supplied page images.
- Compare recognized text with the source images.
- Identify character errors, omitted text, and reading-order problems.
- Compare results across pages with different visual characteristics.
- Compare Tesseract output with Acrobat output.
- Discuss which errors require correction for different uses.

### Text Digitization Workflows

- Connect source selection, image capture, OCR or transcription, quality control, metadata, and publication.
- Identify where structured markup such as TEI might enter a workflow.
- Distinguish files retained for preservation from files produced for access and analysis.
- Consider how page images and recognized text remain associated.
- Outline a workflow for a sample collection, identifying outputs and points requiring human review.

## Reference Resources

- [Tesseract User Manual](https://tesseract-ocr.github.io/tessdoc/)
- [Tesseract Installation Guidance](https://tesseract-ocr.github.io/tessdoc/Installation.html)
- [W3C: Choosing & Applying a Character Encoding](https://www.w3.org/International/questions/qa-choosing-encodings.en)