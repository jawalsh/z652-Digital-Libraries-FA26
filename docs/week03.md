# Week 3: Markdown, GitHub, and Static Sites

## Summary

Many contemporary digital library and digital humanities projects are built using a simple but powerful workflow based on plain text, version control, and static web publishing. This week introduces the technologies that make that workflow possible: **Markdown**, **Git**, **GitHub**, and **GitHub Pages**.

Over the course of the week, you'll learn how documents written in Markdown become files stored in a Git repository, how those repositories are managed and shared using GitHub, and how GitHub can publish them as public websites through GitHub Pages.

```text
Markdown
        ↓
Git repository
        ↓
GitHub
        ↓
GitHub Pages
        ↓
Public website
```

Although we’ll use GitHub Pages this week to publish a simple website, this same workflow underlies many contemporary digital library projects, including CollectionBuilder, which you’ll use later in the semester to build your own digital collection. Understanding this workflow will provide the technical foundation for the remainder of the course and your final project.

## Weekly Learning Objectives

By the end of this week, you should be able to:

* Explain the roles of Git, GitHub, GitHub Pages, and Markdown in a modern static-site publishing workflow.
* Explain the advantages of plain-text formats and version control for digital library and digital humanities projects.
* Create and edit documents using basic Markdown syntax.
* Navigate a GitHub repository and identify its major components (e.g., README, folders, configuration files, and project documentation).
* Describe how GitHub Pages publishes a static website directly from a GitHub repository.
* Explain the differences between static and database-driven websites and identify the advantages and limitations of each approach.
* Recognize why static-site methodologies have become increasingly popular for digital libraries, digital exhibits, and other cultural heritage projects.

# Before Class

## Readings

### Required

-   Wikle, Olivia M., and Evan Peter Williamson. [“Static Web Methodology
    as a Sustainable Approach to Digital Humanities Projects.”](https://journal.code4lib.org/articles/18372) [*Code4Lib*](https://journal.code4lib.org)
    Journal (2025).
-   Wikle, Olivia, Evan Williamson, and Devin Becker. [“What is Static
    Web and What's it Doing in the Digital Humanities Classroom?”](https://acrl.ala.org/dh/2020/06/22/what-is-static-web-and-whats-it-doing-in-the-digital-humanities-classroom) _dh+lib_ (2020).

### [Lib-Static](https://lib-static.github.ioi)

Read:

- [Why Lib-Static?](https://lib-static.github.io/about/)
- On the [Concepts](https://lib-static.github.io/concepts/) page read the following:
    - [Command Line](https://lib-static.github.io/concepts/cli/);
    - [Static Site Generators](https://lib-static.github.io/concepts/static-site-generators/);
    - [Plain Text](https://lib-static.github.io/concepts/plaintext/).
    - [Version Control](https://lib-static.github.io/concepts/version-control/)
    - Explore other concepts as time permits.

- [What is GitHub?](https://docs.github.com/en/get-started/start-your-journey/what-is-github)
- [About Git?](https://docs.github.com/en/get-started/using-git/about-git)
- [Basic writing and formatting syntax (Markdown)](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

	
<!--
	
## Watch

GitHub Skills:

-   Introduction to GitHub
-   Markdown Basics

(approximately 20--30 minutes total)

-->

## Tasks

### 1. Create a [GitHub](https://github.com) account

If you do not already have one.


### 2. Explore an existing repository

Browse the source code for [CollectionBuilder](https://github.com/CollectionBuilder/collectionbuilder-gh) or another open-source digital humanities project.

Identify:

-   README
-   license
-   configuration files
-   documentation
-   content
-   assets

Come prepared to discuss what each appears to do.

### 3. Create Your First GitHub Page

1. Create a GitHub repository.
2. Add a README.md.
3. Use Markdown to introduce yourself and your project interests.
4. Include:
    * one heading
    * one image
    * one table
    * one link
    * one code block
    * one bulleted list
5. Commit your changes.
6. Enable GitHub Pages.
7. Visit your published site.

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

- What surprised you about Markdown, GitHub, or static websites?
- What advantages might plain-text files and version control offer for a digital library project?
- What limitations or challenges might arise when publishing a digital collection as a static website?
- What parts of this workflow still feel unclear or unfamiliar?

## Looking Ahead

Next week we'll shift from infrastructure to **metadata**, examining how
structured descriptive information powers discovery, organization, and
reuse in digital libraries. We'll begin designing the metadata that will
eventually support your own course project.
