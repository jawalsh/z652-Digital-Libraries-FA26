# Week 3: Markdown, GitHub, and Static Sites

## Summary

This week introduces three foundational technologies that support many
contemporary digital library and digital humanities projects:
**Markdown**, **GitHub**, and **static websites**.

Rather than focusing on a particular digital library platform, we'll
explore why so many digital collections today are built from plain-text
files stored in version control and published as static websites.
Students will learn basic Markdown syntax, become comfortable navigating
GitHub repositories, and understand how GitHub Pages can publish a
website directly from a repository.

These skills will provide the technical foundation for later work with
CollectionBuilder and each student's final digital library project.

------------------------------------------------------------------------

## Weekly Learning Objectives

By the end of this week, students should be able to:

-   Explain the advantages of plain-text formats for digital library
    projects.
-   Write and edit documents using basic Markdown syntax.
-   Navigate a GitHub repository and understand its organization.
-   Describe how GitHub Pages publishes static websites.
-   Explain the difference between static and database-driven web
    applications.
-   Recognize why static-site approaches have become increasingly
    popular for cultural heritage collections.

# Before Class

## Readings

### Required

-   Wikle, Olivia M., and Evan Peter Williamson. *Static Web Methodology
    as a Sustainable Approach to Digital Humanities Projects.* Code4Lib
    Journal (2025).
-   Wikle, Olivia, Evan Williamson, and Devin Becker. *What is Static
    Web and What's it Doing in the Digital Humanities Classroom?* dh+lib
    (2020).

### Lib-Static

Read:

-   Why Lib-Static?
-   Plain Text
-   Static Site Generators
-   Version Control (if available)
-   GitHub
-   Command Line

Explore other concepts as time permits.

## Watch

GitHub Skills:

-   Introduction to GitHub
-   Markdown Basics

(approximately 20--30 minutes total)

## Tasks

### 1. Create a GitHub account

If you do not already have one.

### 2. Complete the GitHub Markdown tutorial

Create a small Markdown document that includes:

-   headings
-   lists
-   emphasis
-   links
-   an image
-   a table
-   a code block

Commit it to a GitHub repository.

### 3. Explore an existing repository

Browse the source code for CollectionBuilder or another open-source
digital humanities project.

Identify:

-   README
-   license
-   configuration files
-   documentation
-   content
-   assets

Come prepared to discuss what each appears to do.

### 4. Reflection (Canvas)

In approximately 300 words:

> Why might a static website be an attractive approach for publishing a
> digital library or digital exhibit?

Discuss:

-   sustainability
-   preservation
-   security
-   maintenance
-   cost

# In Class

## Lecture

### Markdown

-   Plain text
-   Why Markdown?
-   Comparison with Word
-   Documentation as infrastructure

### Git and GitHub

-   repositories
-   commits
-   history
-   collaboration
-   issues
-   pull requests (overview)

### Static websites

-   HTML generated from source files
-   GitHub Pages
-   Jekyll
-   Why "no database" can be an advantage

Compare:

``` text
WordPress
↓
Database
↓
Dynamic page
```

versus

``` text
Markdown
↓
Static site generator
↓
HTML
↓
GitHub Pages
```

### Case Study

CollectionBuilder

Rather than installing CollectionBuilder, examine:

-   repository organization
-   `_config.yml`
-   `_data`
-   `objects`
-   layouts
-   pages

Explain how these pieces fit together.

## Hands-on Activity

Working in pairs:

1.  Edit a Markdown document.
2.  Commit a change.
3.  Publish it with GitHub Pages.
4.  Make another change and observe how the website updates.

## Discussion

-   What surprised you about static websites?
-   Why are libraries increasingly adopting static approaches?
-   What tradeoffs exist compared to Omeka, Islandora, or Hyrax?

## Looking Ahead

Next week we'll shift from infrastructure to **metadata**, examining how
structured descriptive information powers discovery, organization, and
reuse in digital libraries. We'll begin designing the metadata that will
eventually support your own course project.
