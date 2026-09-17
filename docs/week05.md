# Week 5: Metadata I: Metadata Fundamentals and Dublin Core

## Summary

This week we step back from CollectionBuilder to examine the structured data that makes a digital collection work: **metadata**. In Week 4, we saw that CollectionBuilder uses a CSV file in which rows describe collection items and columns represent metadata fields. This week we will ask how those fields are chosen, what they mean, and how metadata standards help collections describe resources consistently.

We will focus especially on **Dublin Core**, a widely used metadata element set and an important foundation for the metadata used in CollectionBuilder. We will also establish vocabulary that we will use throughout the next three weeks, including **metadata record**, **element/field**, **value**, **schema**, **obligation**, **cardinality**, and **repeatability**.

This week also introduces the idea of a **metadata application profile (MAP)**: a documented set of decisions about how a particular collection will use metadata elements. You will not design your MAP yet; first we need to understand the pieces from which one is built.

## Weekly Learning Objectives

By the end of this week, you should be able to:

- *define* metadata and explain several purposes it serves in a digital collection.
- *distinguish* among descriptive, administrative, structural, and technical metadata.
- *identify* metadata records, elements/fields, and values.
- *explain* the purpose of a metadata schema or element set.
- *identify* appropriate Dublin Core elements for describing common digital collection objects.
- *define* **obligation** and explain the distinction among required, recommended, and optional elements.
- *define* **cardinality** and **repeatability** and explain why collections need rules governing the number of values permitted for an element.
- *explain* at a basic level what a metadata application profile does.
- *connect* Dublin Core concepts to metadata fields used in CollectionBuilder.

# Before Class

## Readings and Resources

### Metadata Fundamentals

Read:

- Miller, S. J. (2022). *Metadata for Digital Collections*, 2nd ed., Ch. 1, “Introduction to Metadata for Digital Collections” (pp. 1–26). **See Canvas → Files → Readings.**

Browse:

- Riley, Jenn. (2017). [*Understanding Metadata: What Is Metadata, and What Is It For?*](https://www.niso.org/publications/understanding-metadata-2017). National Information Standards Organization.

As you read, focus on the purposes metadata serves rather than trying to memorize every metadata standard mentioned.

### Dublin Core

Read and explore:

- [Dublin Core Metadata Element Set, Version 1.1](https://www.dublincore.org/specifications/dublin-core/dces/)
- [DCMI Metadata Terms](https://www.dublincore.org/specifications/dublin-core/dcmi-terms/)

Pay particular attention to the fifteen elements in the Dublin Core Metadata Element Set, Version 1.1. You do not need to memorize them.

### Metadata Application Profiles

Skim:

- Miller, S. J. (2022). *Metadata for Digital Collections*, 2nd ed., Ch. 12, “Metadata Application Profile Design,” pp. 393–404. **See Canvas → Files → Readings.**
- [Metadata Application Profile assignment](assignment_metadata_application_profile.md)

At this stage, focus on understanding what an application profile is and what kinds of decisions it documents. We will work with the assignment in detail during Weeks 6 and 7.

## Tasks

### 1. Examine CollectionBuilder metadata

Return to the CollectionBuilder site and repository you worked with last week. Locate the metadata CSV and choose one item record.

Identify:

- the fields used to describe the item;
- the values contained in those fields;
- fields that appear to correspond to Dublin Core elements;
- fields that appear to serve a CollectionBuilder-specific purpose.

Come prepared to discuss what you find.

### 2. Metadata observation

Choose one item from an existing digital collection. Identify at least five pieces of descriptive metadata associated with the item and consider which Dublin Core elements could represent them.

# In Class

## Topics

- What is metadata?
- Purposes and types of metadata
- Metadata records, elements/fields, and values
- Metadata schemas and element sets
- Dublin Core
- Obligation: required, recommended, and optional elements
- Cardinality and repeatability
- From general standards to local collection practices
- Introduction to metadata application profiles
- Dublin Core and CollectionBuilder metadata

## Hands-on Activity

Working with sample digital objects and metadata records, we will:

1. Identify information that should be recorded about each object.
2. Map descriptive information to appropriate Dublin Core elements.
3. Compare different choices for describing the same object.
4. Consider which elements should be required, recommended, or optional.
5. Decide whether particular elements should permit one or multiple values.
6. Compare our decisions with metadata used in CollectionBuilder.

The goal is not to produce a complete application profile yet. Instead, we will practice making the kinds of decisions that an application profile must document.

## Discussion

- What information is essential for describing an item in a digital collection?
- When might two collections use the same Dublin Core element differently?
- Why might a collection require one field but make another optional?
- When should a metadata element allow multiple values?
- What happens when metadata rules are not documented consistently?

## Looking Ahead

Next week we move from **which metadata elements to use** to **what values should go into them and how those values should be recorded**.

We will examine **controlled vocabularies**, **value encoding schemes**, and **content guidelines**, then bring these decisions together in a **metadata application profile** for your CollectionBuilder project.
