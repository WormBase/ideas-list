# Google Summer of Code Ideas list (2018)

### Community-driven curation
[_Risky/Exploratory_]

Scientific databases that curate the primary literature face an enormous challenge: the number of research papers continues to skyrocket, but the process of curation is slow, tedious, and resource-constrained. One solution is to engage the primary research community in curation of their own data, a strategy referred to as "community curation". At the same time, such strategies require careful and automated quality control to ensure the integrity of submissions and to prevent abuse of the system. We'd like to build a data submission and reviewing system that can be generalized to work on the diverse data types that we curate.
* Expected outcome: A [Datomic](https://docs.datomic.com/on-prem/getting-started/brief-overview.html) database that models "under review" content as well as approved content. A REST API for reviewing and approving content, and accessing content that may or may not include those that are under review.
* Skills preferred: Clojure, database
* Possible mentors: Adam Wright, Sibyl Gao, Matt Russell
* Difficulty rating: difficult

### Revision tracking curation database and tools
[_Fun/Peripheral_]

Serving up-to-date content is critical for repositories like WormBase supporting basic scientific research. Our current workflow consists of periodic integration of multiple databases into a single production database every 2 months. While stable, this impedes real-time publication of new data. Having a live-curated database to power our website motivated our ongoing database migration to [Datomic](https://docs.datomic.com/on-prem/getting-started/brief-overview.html), a transactional database with change tracking and a queryable history. It will enable us to build a live-curated website with an emphasis on change tracking. In addition to having curated content immediately available to users, this website will provide information on what has changed recently along with metadata associated with these updates, such as citations and remarks. We'd like to start by making a prototype that works on the person/lineage data.
* Expected outcome: A Datomic database that models person/lineage data and a REST API for submitting and retrieving content, reviewing change history, and optionally a user interface
* Skills preferred: Clojure, database
* Possible mentors: Adam Wright, Sibyl Gao, Matt Russell
* Difficulty rating: medium

### Multi-container cloud deployment
[_Infrastructure/Automation_]

Continuously deploying code and data is a long term goal of WormBase. Over the past several years, we have been moving towards a Docker based approach, using AWS' ElasticBeanstalk to deploy individual containers. As we deploy more components of our microservice based architecture, there is an increasing need to coordinate the deployment of the individual services. This project focuses on the devops side of WormBase, creating a prototype of a provisioning system using modern cloud deployment technologies to streamline our workflow.
* Expected outcome: A proof of concept, Docker based, system for deploying and maintaining our microservice architecture.  
* Skills preferred: Docker, DevOps, AWS, Kubernetes
* Possible mentors: Adam Wright
* Difficulty rating: medium

### Improve search result relevance
[_Core development_]

An effective search is a critical tool for any large data repository. This project seeks to improve an ElasticSearch-backed service at WormBase with improved code for indexing and search queries. A related component of this project will use analytics to better understand user behavior and how it affects search results.
* Expected outcome: Improve the relevance of search result by improving the code that indexes the content and/or queries the search index
* Skills preferred: Elasticsearch
* Possible mentors: Sibyl Gao
* Difficulty rating: medium

### Navigating search with facets
[_Core/UI development_]
Finding meaningful results in biological data is rarely as simple as conducting a single, basic search. Instead, users often need to step through results with filters to gain new insight into the data. This project aims to add facets, counts, and dynamic graphs to search results stored in our main ElasticSearch database.
* Expected outcome: Improve search interface through the use of facets and relevant visualizations.
* Skills preferred: Elasticsearch, JavaScript, d3.js
* Possible mentors: Sibyl Gao, Adam Wright
* Difficulty rating: medium

### User interface re-design and implementation
[_Core development_]
As we have been actively converting the WormBase website from TemplateToolkit/JQuery to React, we have begun to consider new user interface approaches. For example, the current WormBase website is heavily geared towards per-page customization (see [this page](http://www.wormbase.org/species/c_elegans/gene/WBGene00006763, for example)). This project will review the current website, make suggestions, and create user interface implementations more intuitive.
* Expected outcome: Design and implement user interface improvements to make it more intuitive to new users and easier to locate information.
* Skills preferred: HTML, CSS, JavaScript
* Possible mentors: Sibyl Gao
* Difficulty rating: medium



### Have your own ideas?
Please let us know at developers@wormbase.org


## Contributing to this list

This list is prepared as part of the application for the Google Summer of Code.

Please feel free to add your WormBase project ideas to this list.

Please refer to [these tips on defining a project idea](https://google.github.io/gsocguides/mentor/defining-a-project-ideas-list) and be sure to mention which WormBase developer has agreed to mentor a student on developing your idea.
