# Week 13: CollectionBuilder: Configuration, Metadata Integration, and Customization

## Summary

This week, we bring together our work on metadata, digital objects, and web publishing to develop our final CollectionBuilder projects. We will connect project metadata and collection files to the site, configure how information appears, and build pages that provide context and interpretation.

We will examine the relationships among metadata spreadsheets, configuration files, Markdown pages, and the resulting website. Most class time will be devoted to applying these techniques to your final project, checking the published results, and addressing problems with assistance from the instructors and your classmates.

## Weekly Learning Objectives

- _navigate_ and _use_ CollectionBuilder documentation to address project-specific needs
- _integrate_ collection metadata and digital objects into a CollectionBuilder site
- _verify_ that identifiers, filenames, paths, and metadata fields produce the intended results
- _configure_ site information, theme options, navigation, and metadata display
- _edit_ existing pages and _create_ contextual or interpretive pages
- _evaluate_ whether the published site represents the collection accurately and supports its intended audience

## Before Class: Readings, Resources, and Tasks

### Readings and Reference Resources

Read the following documentation with your own project repository open. Examine the corresponding files as you read.

- [Initial Site Configuration](https://collectionbuilder.github.io/cb-docs/docs/config/)
  - Review `_config.yml`, especially site information, URL settings, and the selection of your metadata file.
- [CollectionBuilder Metadata](https://collectionbuilder.github.io/cb-docs/docs/metadata/)
  - Follow the sections for the version of CollectionBuilder you are using.
  - Review the instructions for formatting and adding metadata.
- [Theme Configuration](https://collectionbuilder.github.io/cb-docs/docs/theme/)
  - Focus on the home page, browse page, and item page. Consult other sections as needed for your collection.
- [Add a Page](https://collectionbuilder.github.io/cb-docs/docs/pages/add_page/)
  - Review Markdown pages, YAML front matter, and navigation.

You do not need to read every subsection. Use the documentation to investigate the settings and features relevant to your project.

### Project Preparation

Come prepared to work in your **final project repository**.

- If you have not yet created a separate repository for your final project, create it before class.
- Have your current metadata spreadsheet and metadata application profile available.
- Prepare a small, representative set of collection objects and metadata records to test in your site. Include different formats or types of objects if your collection uses them.
- Have drafts or notes for your collection’s contextual background or interpretive content available.
- Review your published site and identify specific questions or problems you want help resolving.

There is no separate discussion post this week. Bring your project questions to class.

## In Class

### CollectionBuilder Files and Configuration

We will review how the main components work together:

- `_config.yml`: core site information and settings
- `_data/theme.yml`: theme and display options
- `_data/config-*.csv`: configuration for navigation, metadata display, and other interface features
- the collection metadata CSV: descriptions of collection objects
- collection files or object URLs: the resources described by the metadata
- Markdown pages and YAML front matter: contextual and interpretive content

We will also review the roles of CSV, YAML, Markdown, and HTML and common formatting problems that can affect a site build.

### Metadata Integration and Verification

Using your own project materials work on the following tasks, as time allows:

- Export your metadata spreadsheet as a UTF-8 CSV and add it to the appropriate location in your repository.
- Configure the site to use your metadata file.
- Check that object identifiers, filenames, and paths match the collection files or URLs.
- Compare sample records with your MAP, checking required fields, repeated values, and formatting conventions. 
	- Update your MAP or your metadata to make sure they are consistent.
- Inspect the resulting item pages, browse interface, and search results.
- Configure which metadata fields appear and how they are labeled.
- Check whether metadata supports any enabled maps, timelines, or other browsing features.

A successful build is only the first check. Verify that the published site displays the intended objects and information.

### Configuration and Customization

Apply changes that support your collection and its audience:

- Replace remaining template titles, descriptions, and other placeholder content.
- Configure the home page and relevant browse and item-page options.
- Review navigation and remove or revise links that do not serve your collection.
- Edit the About page.
- Create or develop a contextual or interpretive page.
- Add links between your discussion and relevant collection items.

### Final Project Lab

Most class time will be devoted to work on your final project, with demonstrations and individual assistance as needed.

Prioritize:

1. Getting your own metadata and collection objects working together.
2. Checking and correcting the published results.
3. Configuring useful metadata display and navigation.
4. Developing contextual and interpretive content.

Feel free to work collaboratively during lab time. Help one another troubleshoot problems, share solutions and ideas, and ask classmates to test features or provide feedback on your collections. The instructors will also be available for questions and individual assistance.

## Project Progress

By the end of this week, aim to have:

- a published final-project site using your own metadata and at least a representative set of collection objects;
- working item pages with appropriate metadata labels and fields;
- site information and navigation adapted to your collection;
- contextual or interpretive content underway;
- specific remaining problems identified for the Week 14 deployment and troubleshooting session.

Continue expanding and checking your collection after class. Use the final project assignment to guide the scope and required components of your submission.

For the final project, you will also create a short recorded video walkthrough of your collection. The video will introduce your collection, demonstrate its principal features, and explain important design decisions. We will discuss expectations in more detail during Week 14.
