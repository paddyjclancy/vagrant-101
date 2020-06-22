# Development Environment


### Levels of Abstraction:
- Higher level, higher control, higher requirements


1) Mainframe                                   (IBM, HP, Dell)
  - Your computer, your solution, your problem (client)
  - Planning, serving, maintaining, manning, setting up everything (except producing)


2) IaaS  -  Infrastructure as a service        (AWS, Azure, Google Cloud)
  - Rent out computing and storage power required
    - Rent by the second
    - Scalable
  - Provider has shared responsibility model - their job to secure / maintain cloud
  - Client job to do INTERNAL security
  (- All of Netflix, Amazon, Prime Video runs on AWS)


3) PaaS  -  Platform as a service              (Above, Heroku)
  - Built on top of IaaS, technical knowledge still required by client
  - Better GUIs
  - Relatively higher cost
  - Less control, more vendor lock in
  - Client can push code, it will read and deploy


4) SaaS  -  Software as a service              (Salesforce, Dropbox, Teams, Gmail)
  - No downloads / physical install
  - Everything within the cloud & accessed by browser / API
  - Web native SaaS / other (downloadable) SaaS
    - Downloadable means updates required, runs on independent environment
    - Web native + steadier connection --> better quality of experience




### Four Pillars of DevOps
Defines the role


1) Ease of use
  - Infrastructure needs to be easy to use for entire team

2) Flexibility
  - Allows ability to evolve

3) Robustness
  - 100% uptime
  - Fast deployment
  - Strength / Reliability of Infrastructure

4) Cost
  - Cap-ex & Op-ex
  - Cost of downtime
  - Cost of slow innovation
  - Cost of time to market
  - Cost of infrastructure



## Environments

A location where code runs and data lives eg this laptop (not GitHub)

- Development
  - Python, SQL, HTML, CSS...
- Testing
  - Ensures functionality and quality
  - Has its own tools / infrastructure that dev environments lack
- Production


- Pipelines transfer code from dev --> test --> production
