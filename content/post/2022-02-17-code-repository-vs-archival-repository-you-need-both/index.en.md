---
title: Code Repository vs Archival Repository. You need both.
authors: 
- admin
date: '2022-02-17'
slug: code-repository-vs-archival-repository-you-need-both
categories:
  - reproducibility
  - archives
  - github
  - version control
tags:
  - repo
  - git
subtitle: ''
summary: 'The imperatives for preserving research data are derived from expressly different motives than those driving version-control repositories.'
lastmod: '2022-04-21T13:16:20-04:00'
featured: no
image:
  caption: ''
  focal_point: ''
  preview_only: no
projects: []
---

> [This blog post](https://blogs.library.duke.edu/data/2022/02/17/code-repository-vs-archival-repository-you-need-both/) is republished from the CDVS blog with permission from the author

Years ago I heard the following quote attributed to Seamus Ross from 2007:

> Digital objects do not, in contrast to many of their analog counterparts, respond well to benign neglect. 

Meaning, you cannot simply leave digital files to their bit-rot tendencies while expecting them to be usable in the future.  Digital repositories are part of a solution to this problem.  But to review, there are many types of repositories, both digital and analog:  repositories of bones, insects, plants, books, digital data, etc.  Even among the subset of digital repositories there are many types.  Some digital repositories keep your data safe for posterity and replication.  Some help you manage the distribution of analysis and code.  Knowing about these differences will affect not only the ease of your computational workflow, but also the legacy of your published works.

## Version-control repositories and their hubs

The most widely known social coding hubs include GitHub, Bitbucket and GitLab.  These hubs leverage Git version-control software to track the evolution of project repositories -- typically a software or computational analysis project.  Importantly, Git and GitHub are not the same thing but they work well together.

Version control works by monitoring any designated folder or project directory, making that directory a local repository or repo.  Among other benefits, using version control enables "time travel." Interactions with earlier versions of a project are commonplace.  It's simple to retrieve a deleted paragraph from a report written six months ago.  However there are many advanced features as well. For example, unlike common file-syncing tools, it's easy to recreate an earlier state of an entire project directory and every file from a particular point in time.  This feature among others makes Git version-control a handy tool in support of many research workflows and the respective outputs:  documents, visualizations, dashboards, slides, analysis, code, software, etc.

Git is one of the most popular, open-source, version-control applications; originally developed in 2005 to facilitate the evolution of the world's most far reaching and successful open-source coding project.  Linux is a world-wide collaborative project that spans multiple developers, project managers, natural languages, geographies, and time-zones.  While Git can handle large projects, it is extensible and can easily scale up or down to support a wide range of workflows.  Additionally, Git is not just for software and code files.  Essentially any file on a file system can be monitored with Git:   MSWord, PDF files, images, datasets, etc. 

There are many ways to share a Git repository and profile your work.  The term push refers to a convenient process of synchronizing a repo up to a remote social coding hub.  Additional features of a hub include issue tracking, collaboration, hosting documentation, and Kanban Method planning.  Conveniently, pushing a repo to GitHub means maintaining a seamless, two-location backup -- a push will simultaneously and efficiently synchronize the timeline and file versions. Meanwhile, at a repo editor's discretion, any collaborator or interested party can be granted access to their GitHub repository.

Many public instances of social-coding hubs operate on a freemium model.  At GitHub most users pay nothing.  It's also possible to run a local instance of a coding hub.  For example, OIT offers a local instance of GitLab, delivering many of the same features while enabling permissions, authorization, and access Via Duke's NetID.

While social coding hubs are great tools for distributing files and managing project life-cycles, in and of themselves they do not sufficiently ensure long-term reproducible access to research data.  To do that simply synchronize version-control repositories with archival research data repositories.

## Research Data Repositories

Preserving the computational artifacts of formal academic works requires a repository focus that is complementary to version-control repositories and social-coding hubs.  Nonetheless, version control is not a requirement of a data repository where the goal is long-term preservation. Fortunately, many special-purpose data repositories exist.  Discipline-specific research repositories are sometimes associated with academic societies.  There also exist more generalized archival research repositories such as Zenodo.org.  Additionally, many research universities host institutional research data repositories.  Not surprisingly, such a research data repository exists at Duke where the Duke University Libraries promotes and cooperatively shepherds Duke's Research Data Repository (RDR).

Unlike social coding hubs, data repositories operate under different funding models and are motivated by different horizons.  Coding hubs like GitHub do not promise long-term retention, instead they focus on immediate distribution of version-control repos and offer project management features. Research data repositories take a long view centered closer to the artifacts of formal research and publication.

By archiving the data milestones of publication, a deposit in the RDR links a formal publication -- book edition, chapter, or serial article, etc. -- with the data and code (i.e., a compendium) used to produce a single tangible instance of publication.  In turn, the building blocks of computational thinking and research processes are preserved for posterity because the RDR maintains an assurance of long term sustainability.

In the Duke RDR, particular effort is focussed on preserving unique versions of data associated with each formal publication.  In this way, authors can associate a digital object identifier, or DOI, with the precise code and data used to draft an accepted paper or research project.  Once deposited in the RDR, researchers across the globe can look at these archives to verify, to learn, to refute, to cite, or be inspired toward new avenues of investigation.

By preserving workflow artifacts endemic to publication milestones, research data repositories preserve the record of academic progress.  Importantly, the preservation of these digital outcomes or artifacts is strongly encouraged by funding agencies.  Increasingly, these archival access points are a requirement for funding, especially among publicly funded research.  As such, the Duke RDR exists with aims to preserve and make the academic record accessible, and to create a library of reproducible academic research.

## Conclusion

The imperatives for preserving research data are derived from expressly different motives than those driving version-control repositories.  Minimally, version-control repositories do not promise academic posterity.  However, among the drivers of scholarship is the intentional engagement with the preserved academic record.  In reality, while unlikely, your GitHub repository could vanish in the blink of the next Wall Street acquisition. Conversely research data repositories exist with different affordances.  These two types of repositories complement each other.  Once more, they can be synchronized to enable and preserve digital processes that comprise many forms of data-driven research.  Using both types of repositories imply workflows that positively contribute to a scholarly legacy. It is this promise of academic transmission that drives Duke's RDR, and benefits scholars by enabling access to persistent copies of research.
