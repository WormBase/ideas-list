# Ideas list (2018)

### User interface re-design and implementation
[_Core development_]
* Expected outcome:
* Skills preferred: HTML, CSS, JavaScript
* Possible mentors: Sibyl Gao
* Difficulty rating: medium

### Multi-container cloud deployment
[_Infrastructure/Automation_]
* Expected outcome:
* Skills preferred: HTML, CSS, JavaScript
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
