# Week 4: CollectionBuilder Introduction

## Summary

This week we begin working with **CollectionBuilder**, the platform we will use to build digital collections during the semester. CollectionBuilder brings together many of the technologies introduced last week—including Markdown, GitHub, GitHub Pages, YAML, and static-site generation—and adds structured metadata and digital objects to create a functional digital collection.

We will examine the structure of a CollectionBuilder repository, learn how metadata and digital objects become pages in a collection website, and begin working with a CollectionBuilder site ourselves.

The goal this week is not to master CollectionBuilder. Instead, we will become familiar with its basic structure and workflow so that, as we learn more about metadata and digital libraries over the coming weeks, we can apply those concepts directly to a working collection.

## Weekly Learning Objectives

By the end of this week, you should be able to:

- Explain the basic purpose and architecture of CollectionBuilder.
- Identify the major components of a CollectionBuilder repository.
- Explain how metadata, digital objects, configuration files, and templates work together to produce a collection website.
- Navigate and make basic changes to a CollectionBuilder project on GitHub.
- Explain the role of the `objectid` in connecting collection metadata with digital objects.
- Build and publish a basic CollectionBuilder site using GitHub Pages.
- Identify connections between CollectionBuilder and the static-web technologies introduced in Week 3.

# Before Class

## Readings and Resources

### CollectionBuilder

Read:

- [CollectionBuilder](https://collectionbuilder.github.io/)
- [CollectionBuilder Documentation](https://collectionbuilder.github.io/cb-docs/)
- [CollectionBuilder-GH](https://collectionbuilder.github.io/cb-docs/docs/gh/)

Browse:

- [CollectionBuilder-GH repository](https://github.com/CollectionBuilder/collectionbuilder-gh)

As you explore the repository and documentation, don't worry about understanding every file or configuration option. Focus on getting a general sense of:

- where metadata is stored;
- where digital objects are stored;
- where site configuration is stored;
- how the repository becomes a website.

## Tasks

### 1. Review your GitHub setup

Make sure that you can:

- log into GitHub;
- create or access a repository;
- edit a file;
- commit changes;
- locate the **Settings → Pages** options for a repository.

### 2. Explore a CollectionBuilder site

Explore one of the CollectionBuilder example projects in [CollectionBuilder Examples](https://collectionbuilder.github.io/cb-examples/), a CollectionBuilder collection of other collections. 

Identify several features that appear to depend on structured metadata, such as:

- item pages;
- browse;
- search;
- maps;
- timelines;
- subjects or other facets.

Come prepared to discuss what you think is happening "behind" the interface.

# In Class

## Topics

- What is CollectionBuilder?
- CollectionBuilder and the static-web workflow
- Anatomy of a CollectionBuilder repository
- Metadata and digital objects
- `objectid` and item identification
- Configuration files
- From CSV data to collection interfaces
- GitHub Pages and publishing

## Hands-on Activity

We will work through the basic CollectionBuilder workflow together:

1. Create a CollectionBuilder project from a template.
2. Examine the repository structure.
3. Locate the collection metadata and digital objects.
4. Configure basic information about the collection.
5. Publish the site with GitHub Pages.
6. Make a small change to the collection and observe how it changes the published site.

The goal is to leave class with a working CollectionBuilder site that we can use for experiments as we learn additional digital-library concepts.

## Discussion

- How is a CollectionBuilder repository different from the simple GitHub Pages site you created last week?
- Which parts of the collection are **data**, which are **content**, and which are **configuration**?
- What aspects of the public interface appear to be generated from metadata?
- What advantages and limitations can you already see in using a static-site approach for digital collections?

## Looking Ahead

Next week we begin **Metadata I: Metadata Fundamentals and Dublin Core**.

CollectionBuilder has already shown us that metadata does much more than provide labels for digital objects: it structures item pages, search, browse, and other forms of discovery. Next week we'll step back from the software and examine what metadata is, what purposes it serves in digital libraries, and how the **Dublin Core** standard provides a common vocabulary for describing digital resources.