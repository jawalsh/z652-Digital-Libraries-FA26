# Week 11: Text Objects I: XML, Markup, and TEI

## Summary

In the previous two weeks, we explored how digital libraries represent, process, and deliver **image objects**. This week we turn to **text objects**: how we represent the structure and meaning of texts, rather than treating them simply as sequences of characters or as images of pages.

We will introduce **markup** and the **Extensible Markup Language (XML)**, a general-purpose language widely used in digital libraries for representing both metadata and textual content. We will examine XML-based metadata formats, including **Dublin Core, MODS, MARCXML, and METS**, before turning to the **Text Encoding Initiative (TEI)**, which provides guidelines and a vocabulary for encoding texts.

We will consider how structured markup supports discovery, display, analysis, interoperability, and preservation. In a hands-on lab, you will use **Oxygen XML Editor** to create and validate a small TEI document.

## Weekly Learning Objectives

By the end of this week, you should be able to:

- *distinguish* plain text, presentation-oriented markup, and descriptive or semantic markup.
- *identify* XML elements, attributes, and hierarchical document structure.
- *recognize* XML-based metadata formats, including Dublin Core,
  MODS, MARCXML, and METS, and describe their different purposes.
- *distinguish* XML as a general-purpose markup language from
  specific XML vocabularies and schemas used in digital libraries.
- *explain* the difference between well-formed and valid XML.
- *describe* the purposes of TEI and the roles of the `teiHeader` and `text` elements.
- *create*, *edit*, and *validate* a basic TEI XML document using Oxygen XML Editor.
- *explain* how structured text objects can support digital library services and workflows.

# Before Class

## Readings and Resources

### Required: Markup, XML, and TEI

Watch:

- [A brief introduction to markup, part 1](https://www.youtube.com/watch?v=Z2Nsq613uHk).
- [A brief introduction to markup, part 2](https://www.youtube.com/watch?v=JhhKyyP0e18).

Read:

- TEI Consortium, [**A Gentle Introduction to XML**](https://tei-c.org/release/doc/tei-p5-doc/en/html/SG.html). Focus on what markup does, elements and attributes, document hierarchy, and well-formedness; you do not need to memorize the full range of XML-related technologies.

### Preparation: Oxygen XML Editor

Install **Oxygen XML Editor** before class using [IUware](https://iuware.iu.edu/). Make sure you can launch the application. We will use it during the in-class TEI exercise.

### Optional Background and References

- Witten, Ian H., David Bainbridge, and David M. Nichols. *How to Build a Digital Library* (2010), Chapter 4, pp. 152–213, for additional background on document formats and text representation.
- Renear, Allen H., [“Text Encoding”](https://www.digitalhumanities.org/companion/view?docId=blackwell/9781405103213/9781405103213.xml&chunk.id=ss1-3-5&toc.depth=1&toc.id=ss1-3-5), in *A Companion to Digital Humanities* (2004), for a more conceptual discussion of text encoding.
- TEI Consortium, [**The TEI Header**](https://tei-c.org/release/doc/tei-p5-doc/en/html/HD.html), for reference when documenting the source and encoding of a text.

## Tasks

### 1. Install and test Oxygen XML Editor

Before class, install Oxygen XML Editor and confirm that it opens. If you have difficulty installing it, bring the problem to class so we can troubleshoot before the lab.

### 2. Examine a text as a structured object

Choose a short text, such as a letter, poem, recipe, or news article. Consider:

- What parts of the text have recognizable structures (for example, a title, paragraphs, lines, a date, or a signature)?
- Which features are visible because of typography or layout?
- Which features would be useful to identify explicitly in machine-readable markup?

Come prepared to discuss one or two examples.

# In Class

## Topics

- Text objects in digital libraries: transcription, structure, and
  representation
- Plain text, HTML, XML, and descriptive markup
- XML elements, attributes, nesting, and document hierarchy
- Well-formed XML versus valid XML
- XML schemas and validation in Oxygen
- XML in digital library metadata:
  - Dublin Core in XML
  - MODS and MARCXML
  - METS and the organization of digital objects
- XML vocabularies and schemas: different applications of a common
  markup language
- TEI: goals, applications, and basic document structure
- The `teiHeader`, `text`, and common text-structure elements
- Encoding decisions and their consequences for display, discovery,
  and analysis
- Connections to digital library architecture and image-based
  collections

## Hands-on Activity: Exploring Markup

We will examine how different kinds of texts can be represented with markup, using the [Genre Encoding Exercises](https://dcl.ils.indiana.edu/teiworkshop/genres.html). We will compare possible encoding choices and discuss what each choice makes explicit or leaves implicit.

## Hands-on Activity: TEI Encoding Exercise — Fan Mail

Using Oxygen XML Editor, we will create and validate a simple TEI document based on a piece of fan mail. See [TEI Encoding Exercise: Fan Mail](assignment_tei_encoding_exercise.html) for instructions and submission details.

You will:

1. Identify meaningful structural features of the source text.
2. Create a basic TEI document with a `teiHeader` and `text`.
3. Encode selected textual structures using TEI elements.
4. Check XML well-formedness and validate the document.
5. Consider how different encoding decisions affect what can be done with the text.

## Discussion

- What can structured markup represent that plain text or a scanned page cannot?
- What is the difference between describing how a text looks and describing what its parts mean?
- Why might two people encode the same text differently?
- How can TEI complement page images and metadata in a digital library?
- When might full TEI encoding be unnecessary for a digital collection?
- How is XML used differently in a MODS metadata record, a METS
  document, and a TEI-encoded text?

## Looking Ahead

Next week we will continue exploring **text objects**, considering how encoded texts can be transformed, presented, searched, and integrated into digital library collections.