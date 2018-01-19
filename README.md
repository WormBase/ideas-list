# Google Summer of Code Ideas list (2018)

### User interface re-design and implementation
[_Core development_]
* Expected outcome:
* Skills preferred: HTML, CSS, JavaScript
* Possible mentors: Sibyl Gao
* Difficulty rating: medium

### Multi-container cloud deployment
[_Infrastructure/Automation_]

Being able to continuously deploy code and data is a long term goal of WormBase. Over the past couple of years we have been moving towards a docker based, where we have been using AWS' ElasticBeanstalk to deploy container individually. As we deploy more components of our microservice based architecture, there is a increasing need to coordinate the deployment of the individual services. Unfortunately and fortunately, throughout the process, there has been significant developments in deployment technologies including Kubernetes (https://aws.amazon.com/eks/). We would like a prototype of a provisioning system that will be able to coordinate or deployment process using modern deployment technologies.
* Expected outcome: A proof of concept, Docker based, system for deploying and maintaining our microservice architecture.  
* Skills preferred: Docker, DevOps, AWS, Kubernetes
* Possible mentors: Adam Wright
* Difficulty rating: medium

### Improve relevance search result
[_Core development_]

Search is essential for allowing users to discover the information they need. Hence, it's important to ask: do they find what they look for? If a search is performed immediately followed by another one, maybe they did not. We can probably gain insight on that through some data analysis, by combining keywords that users enter into search with usage metrics captured by Google Analytics.
* Expected outcome: Improve the relevance of search result by improving the code that indexes the content and/or queries the search index
* Skills preferred: Elasticsearch
* Possible mentors: Sibyl Gao
* Difficulty rating: medium

### Revision tracking curation database and tools
[_Fun/Peripheral_]

Serving up to date content is important to WormBase and our users. Unfortunately, we are held back by curation that happens in separate databases, which get build into the production database every 2 months. Having a live-curated database to power our website motivated our ongoing database migration to [Datomic](https://docs.datomic.com/on-prem/getting-started/brief-overview.html), a transactional database with change tracking and a queryable history. It will enable us to build a live-curated website with an emphasis on change tracking. In addition to having curated content immediately available to users, this website will provide information on what has changed recently along with metadata associated with these updates, such as citations and remarks. We'd like to start by making a prototype that works on the person/lineage data.
* Expected outcome: A Datomic database that models person/lineage data and a REST API for submitting and retrieving content, reviewing change history, and optionally a user interface
* Skills preferred: Clojure, database
* Possible mentors:
* Difficulty rating: medium

### Community-driven curation
[_Risky/Exploratory_]

With a growing number of research publications to curate and a constant number of curators, it becomes an increasing challenge to ensure our content is current and accurate. The solution is outsourcing, encouraging researchers in the community to submit data from published papers to us, but at the same time, having some quality control process in place to ensure the system is not abused. We'd like to build a data submission and reviewing system that can be generalized to work on the diverse data types that we curate.
* Expected outcome: A [Datomic](https://docs.datomic.com/on-prem/getting-started/brief-overview.html) database that models "under review" content as well as approved content. A REST API for reviewing and approving content, and accessing content that may or may not include those that are under review.
* Skills preferred: Clojure, database
* Possible mentors:
* Difficulty rating: difficult

### Have your own ideas?
Please let us know at developers@wormbase.org


## Contributing to this list

This list is prepared as part of the application for the Google Summer of Code.

Please feel free to add your WormBase project ideas to this list.

Please refer to [these tips on defining a project idea](https://google.github.io/gsocguides/mentor/defining-a-project-ideas-list) and be sure to mention which WormBase developer has agreed to mentor a student on developing your idea.
