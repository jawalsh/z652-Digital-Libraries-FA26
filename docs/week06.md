# Week 6: Metadata II: Controlled Vocabularies, Value Standards, and Metadata Application Profiles (MAPs)

## Summary

Last week we examined metadata records, elements, values, Dublin Core, obligation, and cardinality. This week we focus on a different problem: even when a collection has chosen the right metadata fields, how do we ensure that the **values entered into those fields are consistent and useful**?

We will distinguish among three important ways of controlling metadata values: **controlled vocabularies**, **encoding schemes/value standards**, and **content guidelines**. We will explore examples such as the Getty vocabularies and consider when locally developed vocabularies or guidelines may be appropriate.

We will then bring the concepts from Weeks 5 and 6 together through the **Metadata Application Profile (MAP)**. A MAP documents how a particular collection uses metadata: which elements it uses, what they mean, whether they are required, how many values they may contain, and what rules govern those values.

This week formally launches the Metadata Application Profile assignment. You will begin designing a MAP for your final CollectionBuilder project and bring a working draft to next week's Metadata Studio for structured peer review.

## Weekly Learning Objectives

By the end of this week, you should be able to:

- *define* **controlled vocabulary** and explain how controlled vocabularies support consistency, discovery, and retrieval.
- *distinguish* controlled vocabularies from encoding schemes/value standards and content guidelines.
- *identify* appropriate controlled vocabularies and value standards for common metadata elements.
- *evaluate* whether an established vocabulary, a local controlled vocabulary, or free text is appropriate for a particular field.
- *explain* the purpose and major components of a metadata application profile.
- *specify* elements, definitions, obligation, cardinality, controlled vocabularies/value standards, and content guidelines in a MAP.
- *identify* CollectionBuilder-specific fields needed for a functioning CollectionBuilder collection.
- *begin designing* a metadata application profile for your final project.

# Before Class

## Readings and Resources

### Controlled Vocabularies and Metadata Values

Read:

- Miller, S. J. (2022). *Metadata for Digital Collections*, 2nd ed., Ch. 6, “Controlled Vocabularies for Improved Resource Discovery” (pp. 165–186). **See Canvas → Files → Readings.**

As you read, pay attention to the problems controlled vocabularies are intended to solve, including synonyms, variant names, ambiguity, and inconsistent terminology.

### Getty Vocabularies

Read the brief descriptions of the following Getty vocabularies, then explore **at least one** using its online search interface:

- [Art & Architecture Thesaurus (AAT)](https://www.getty.edu/research/tools/vocabularies/aat/)
- [Getty Thesaurus of Geographic Names (TGN)](https://www.getty.edu/research/tools/vocabularies/tgn/)
- [Union List of Artist Names (ULAN)](https://www.getty.edu/research/tools/vocabularies/ulan/)

Consider what kinds of metadata fields each vocabulary could help control.

### Metadata Application Profiles

Read:

- Miller, S. J. (2022). *Metadata for Digital Collections*, 2nd ed., Ch. 12, “Metadata Application Profile Design,” pp. 393–404. Skim the examples that follow. **See Canvas → Files → Readings.**
- [Metadata Application Profile assignment](assignment_metadata_application_profile.md)

### CollectionBuilder Metadata

Review the CollectionBuilder documentation for metadata:

- [CollectionBuilder Documentation](https://collectionbuilder.github.io/cb-docs/)

Pay particular attention to the metadata fields required or used by CollectionBuilder. Consider which fields describe the intellectual content of an item and which fields exist primarily to support CollectionBuilder functionality.

## Tasks

### 1. Explore a controlled vocabulary

Using one of the Getty vocabularies above—or another established vocabulary relevant to your project—search for several concepts, people, places, or object types that might appear in a digital collection.

Be prepared to discuss:

- what the vocabulary controls;
- how preferred and variant terms are represented;
- whether the vocabulary would be useful for your project.

### 2. Prepare for MAP design

Review your proposed final project and make a preliminary list of metadata fields you think the collection will need.

For each field, begin considering:

- What does the field mean?
- Is it required, recommended, or optional?
- Can it contain one value or multiple values?
- Should its values come from a controlled vocabulary?
- Is there a standard format or encoding scheme for the value?
- Are content guidelines needed to tell someone how to enter the value?

Bring this preliminary work to class.

# In Class

## Topics

- Why metadata values need rules
- Controlled vocabularies
- Preferred terms, variant terms, and authority control
- Established versus local controlled vocabularies
- Encoding schemes and value standards
- Content guidelines
- Choosing between controlled values and free text
- Metadata application profiles
- Elements and definitions
- Obligation
- Cardinality and repeatability
- Value rules
- CollectionBuilder-specific metadata fields
- Metadata Application Profile assignment

## Hands-on Activity

We will work through a sample metadata application profile together, using actual digital objects to test our decisions.

For each field, we will consider:

| MAP component | Question |
| --- | --- |
| Element / field | What information are we recording? |
| Definition | What exactly does this field mean? |
| Obligation | Is it required, recommended, or optional? |
| Cardinality | How many values may or must be supplied? |
| Controlled vocabulary | Must values come from an approved set of terms? |
| Encoding scheme / value standard | Is there a standard form for representing the value? |
| Content guidelines | What instructions does a metadata creator need in order to enter the value consistently? |
| Example | What does a valid value look like? |

We will then begin applying the same process to your own projects.

## MAP Assignment: Working Draft for Week 7

Begin developing your Metadata Application Profile after class. Bring a **substantive working draft** to Week 7.

The Week 7 draft is **not a graded submission**. It is material for structured peer review and project consultation. The goal is to identify problems while there is still time to revise—not to have the instructor grade the same assignment twice.

Your draft should be developed enough that another student can evaluate whether your metadata rules are understandable and usable.

## Looking Ahead

Next week is a **Metadata Studio**. Rather than introducing a large amount of new material, we will test and improve your MAPs through structured peer review, sample metadata creation, and project consultation.

The central question will be practical:

> Could another person use your application profile to create consistent metadata for your collection without having to ask you what you meant?
