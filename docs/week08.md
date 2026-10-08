# Week 8: From CollectionBuilder to Enterprise Digital Libraries + Project Lab

## Summary

In Weeks 4–7, we built a CollectionBuilder site and learned how to design and document metadata for a small digital collection. This week we ask how a large research library manages **millions of digital objects**, multiple contributors, preservation requirements, and sophisticated discovery services.

We will survey the components of enterprise digital library systems, including **repositories, databases, object storage, search indexes, web interfaces, and preservation services**. We'll introduce software such as Fedora, Samvera/Hyrax, Solr, and PostgreSQL. Our goal is to understand how the components fit together—not to install or administer them. The second half of class will be a **project lab**.

## Weekly Learning Objectives

By the end of this week, you should be able to:

- *identify* the major layers of an enterprise digital library architecture.
- *distinguish* repositories, databases, object storage, search indexes, and public interfaces.
- *describe* the roles of Fedora, Samvera/Hyrax, Solr, and PostgreSQL.
- *explain* basic ingest, derivative generation, indexing, access, and preservation workflows.
- *compare* enterprise repository systems with CollectionBuilder's static-site approach.
- *identify* and work toward concrete milestones for your final project.

# Before Class

## Readings and Resources

### Required: Repository Architecture

Read:

- Banerjee, Kyle, and Terry Reese Jr. *Building Digital Libraries*, 2nd ed. (2019), **Chapter 2, “Choosing a Repository Architecture.”** Available as an eBook through [IUCAT eBook](https://iucat.iu.edu/catalog/19362782).

Focus on the decisions involved in choosing and organizing a repository architecture: which functions a repository needs to support, how components relate, and how an institution's requirements affect technology choices. You do not need to memorize particular products or configurations.

### Brief Software Exploration

Browse (approximately 10–15 minutes total):

- [Fedora Repository](https://fedorarepository.org/) — repository software.
- [Hyrax](https://hyrax.samvera.org/) — a repository application in the [Samvera](https://samvera.org/) ecosystem.

Compare these systems with [CollectionBuilder](https://collectionbuilder.github.io/). Focus on the kinds of problems each is designed to solve, rather than implementation details.

### Optional Background and References

- Witten, Ian H., David Bainbridge, and David M. Nichols. *How to Build a Digital Library*, 2nd ed. (2010), **Chapter 7, §§7.3–7.6**, for additional background on object identification, web services, security, and repository systems. [IUCAT access](https://kg6ek7cq2b.search.serialssolutions.com/?V=1.0&L=KG6EK7CQ2B&S=JCs&C=TC0000298940&T=marc). Some software descriptions are dated.
- [Apache Solr](https://solr.apache.org/), [PostgreSQL](https://www.postgresql.org/), [DSpace](https://dspace.lyrasis.org/), and [Archivematica](https://www.archivematica.org/) — reference sites, not assigned readings.

## Tasks

### 1. Think about scale

Consider what would need to change if your CollectionBuilder collection contained one million objects, required several librarians to edit records simultaneously, or had to be preserved for decades. Bring **one question** about enterprise digital libraries to class.

### 2. Prepare for the project lab

Bring your MAP, your collection materials, and access to your CollectionBuilder repository. Identify **two or three specific tasks** you can accomplish during lab time.

# In Class

## Topics

- CollectionBuilder and the architecture of a static digital collection
- Enterprise digital library architecture
- Digital repositories: Fedora
- Repository applications: Samvera and Hyrax
- Relational databases: PostgreSQL
- Search indexes: Solr and OpenSearch
- File and object storage
- Ingest, derivatives, metadata, and preservation workflows
- IIIF, APIs, and interoperability (overview)
- Institutional staffing and infrastructure

## Architecture Activity

Map your CollectionBuilder project onto the enterprise architecture we discuss. Where do your metadata, objects, presentation, and search functions reside? What additional services would a large institution require?

## Project Lab

Use the remainder of class to work on your final collection. Possible tasks include:

1. Revise metadata records using your MAP and peer-review feedback.
2. Organize digital objects and check filenames and `objectid` values.
3. Update and test your CollectionBuilder site.
4. Identify and resolve technical problems with instructor assistance.
5. Document remaining work and priorities.

Before leaving, record what you completed and your next steps.

## Discussion

- What does a digital repository do that a folder of files does not?
- Why do institutions separate storage, metadata management, and search?
- What advantages does CollectionBuilder offer for a small collection?
- What new requirements arise when a digital collection must be maintained for decades?

## Looking Ahead

Next week we focus on **image objects**: raster and vector graphics, formats, resolution, and the distinction between preservation masters and access derivatives. These concepts will help explain the storage and delivery requirements introduced today.
