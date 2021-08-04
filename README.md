# AWS Enablement Workshop Curator

AWS Enablement Workshop Curator.

Q: What problem does this solve?
A: SA/TAMs are often challenged at finding workshop content that is up to date, this project aims to solve that using open source / crowd sourcing (community feedback).

MVP1:
Define the objective and value-add
Define the workshops schema (see previous msg with JSON example).
Define the GitLab repo and shell of what it could look like (starting with the AWS workshop template).
Input some data (JSON/YAML) and have the website import it automatically.
Serve static website content on an S3 bucket that Tim provides.


MVP2:
CI/CD pipeline that updates and adds new requests to the catalog


```
.
├── metadata.yml                      <-- Metadata file with descriptive information about the workshop
├── README.md                         <-- This instructions file
├── deck                              <-- Directory for presentation deck
├── resources                         <-- Directory for workshop resources
│   ├── code                          <-- Directory for workshop modules code
│   ├── policies                      <-- Directory for workshop modules IAM Roles and Policies
│   └── templates                     <-- Directory for workshop modules CloudFormation templates
└── workshop                          
    ├── config.toml                   <-- Hugo configuration file for the workshop website
    └── content                       <-- Markdown files for pages/steps in workshop
    └── static                        <-- Any static assets to be hosted alongside the workshop (ie. images, scripts, documents, etc)
    └── themes                        <-- AWS Style Hugo Theme (Do not edit!)
```
