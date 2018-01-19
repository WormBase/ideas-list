# Ideas list (2018)

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
* Skills preferred: Docker, DevOps, AWS
* Possible mentors: Adam Wright
* Difficulty rating: medium

### Curation database and tools
[_Fun/Peripheral_]

Serving up to date content is important to WormBase and our users. Unfortunately, it generally takes 2 months before information entered by our curators is available on the website, as a result of the curation happens in separate databases that get build into the production every 2 month. Having a live curated database to power our website has lead to an ongoing effort to migrate from our legacy database solution to Datomic, a transactional database with the added benefit of tracking changes and having historic versions of the database queryable. We would like a prototype of the live-curated website using just our person/lineage data, with an emphasis on the provenance of change.
* Expected outcome: A Datomic database that models person/lineage data and a REST API for submitting and retrieving content, and reviewing change history, (optionally a user interface)
Skills preferred: Clojure, database
* Possible mentors:
* Difficulty rating: medium

### Community-driven curation
[_Risky/Exploratory_]

With a growing number of research publications to curate and a constant number of curators, it becomes an increasing challenge to ensure our content is current and accurate. The solution is outsourcing, encouraging researchers in the community to submit data from published papers to us, but at the same time, having some quality control process in place to ensure the system is not abused.
* Expected outcome: A Datomic database that models "under review" content as well as approved content. A REST API for reviewing and approving content, and accessing content that may or may not include those under review.
* Skills preferred: Clojure, database
* Possible mentors:
* Difficulty rating: difficult


## Contributing to this list

This list is prepared as part of the application for the Google Summer of Code.

Please feel free to add your WormBase project ideas to this list.

Please refer to [these tips on defining a project idea](https://google.github.io/gsocguides/mentor/defining-a-project-ideas-list) and be sure to mention which WormBase developer has agreed to mentor a student on developing your idea.
