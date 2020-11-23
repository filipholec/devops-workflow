<p align="center">
  <img src="https://engeto.cz/wp-content/uploads/2018/12/engeto-main-brand.png" alt="ENGETO Academy Presents">
</p>

# DevOps Academy - Lesson #1
## Important links
- [DevOps Academy Tab](https://engeto.com/cs/)
- [Slack workspace for DevOps Academy]()
- [Introduction to DevOps (online course)](https://engeto.com/cs/kurz/introduction-to-devops/lekce)
- [Git course (online course)](https://engeto.com/cs/kurz/git-zaklady-pro-uzivatele/lekce)

## Goal & structure of this lesson
The main goal of this lesson is to get to know the course, ENGETO team and people on the course.

We can break down the lesson to the following blocks:
 * **Introduction to the course, ENGETO and the team [30m]**
 * **Introduction of yourself [20m]**
 * *Break [10m]*
 * **Prerequisites of this course [20m]**
 * **What is DevOps & its Challenges [30m]**
 * *Break [10m]*
 * **Phases of DevOps [30m]**
 * **Tools we'll be using in this course [30m]**

## Timeline
This course consists of 10 weeks of education, each dedicated to one specific technology.

Here is the breakdown of the weeks:
 1. Introduction to DevOps [9.11.2020]
 2. Infrastructure & Cloud Architecture [16.11.2020]
 3. Web servers & certificate management [23.11.2020]
 4. Configuration and Provisioning (Terraform & Ansible) [30.11.2020]
 5. Docker [7.12.2020]
 6. CI/CD (Continuous Integration and Delivery) [14.12.2020]
 7. Kubernetes #1 [4.1.2021]
 8. Kubernetes #2 [11.1.2021]
 9. Monitoring. Logging & Alerting [18.1.2021]
 10. DevOps project / workshop (certification) [25.1.2021]
 
## Certification
One of the benefits of DevOps onsite course is the possibility to have certification at the end of the onsite course.

This certification consists of:
 * mini project on the exam - students will have an assignment to set up systems to a specific state
 * review of minor projects from each lesson that you should complete before the exam

After you've passed the certification exam, you'll be awarded the **ECDJ - ENGETO Certified DevOps Junior** certification.

## Lecturers
We have 4 lecturers, that will help you throughout this course
 * Ivo Klimsa
 * Marek Cermak
 * Martin Beranek
 * Jan Michalcak
 * Petr Skyva

## Education process
In addition to webinar course, you'll have several online courses with additional information and exercises / projects.

They are all available on our online platform https://engeto.com on the Online DevOps Academy Tab:
 * https://engeto.com/cs/onsite/1KlEujJySWGFvj5-ecl75A/online-devops-academy-czechia-2020-11-09  

You are encouraged to ask questions on our [Slack workspace](https://devopsacademy09112020.slack.com).

## Icebreaker - Task at the beginning
We should get to know each other a bit more. We've created an API that you can call and send a request with data about you.

> **TASK:** Create a `curl` command to our API with 2 sentences about you and what you expect from this course. After 5 minutes, we'll go through the submissions. Alternatively, you can use Python requests if that's better for you.

Information:
 * write 2-3 sentences about you - what is your tech background, what do you want from this course, if you want to have career consulting at ENGETO
 * we will use channel #introduction in Slack
 * the Slack hook for writing a news message is `https://hooks.slack.com/services/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`
 * we'll use a `POST` request on this hook
 * send JSON data - parameter text, value will be your introduction
 * you can verify successful task completion in channel #introduction - your message will be sent by App "Intro API"

## What is DevOps
There are many definitions of what the term DevOps means, since it can be ambiguous. When you ask 10 different people, each might come up with their own explanation.

But, let's start with what is the mainstream definition of the word DevOps:
> **DevOps is the software engineering culture that is aimed at unification and cooperation of two major players in IT - Development (Dev) and Operations (Ops).**

What is nice about DevOps:
 * shorter development cycles (similar to agile development)
 * which results in the increased frequency of deployments
 * dependable releases, in alignment with business goals
 * the added value compared to development is the operations part (infrastructure, deployment, automation, ...)   

It also strongly advocates for automation and monitoring of all steps in software development:
 * integration
 * testing
 * releasing
 * deployment
 * infrastructure management
 
## Challenges in DevOps
<p align="center">
  <img src="assets/before-after-devops.png" alt="Before & After DevOps">
</p>

 * Lack of a Standard Definition for DevOps
 * Choice of Tools
 * Cultural Challenges
 * Isolated Teams
 * Expectations do not match reality

<p align="center">
  <img src="assets/wall-of-confusion.png" alt="Wall of Confusion">
</p>

### How to face challenges in DevOps
 * Proper training and focus
 * Bringing teams together
 * Flexible tool orchestration options
 * Metrics & use analytics to visualize

## DevOps workflow
When talking about DevOps, it’s important to divide the process into phases which come together to make a DevOps pipeline. This way, we can break down the problem of describing the tools and processes used throughout the various phases.

Now, we'll describe the phases of DevOps in more depth and in next lesson, we'll talk more about tools used in these phases.

<p align="center">
  <img src="assets/What-is-Devops.png" alt="What is Devops">
</p>

### Plan
The Plan stage covers everything that happens before the developers start writing code, and it’s where a Product Manager or Project Manager earns their keep. Requirements and feedback are gathered from stakeholders and customers and used to build a product roadmap to guide future development. The product roadmap can be recorded and tracked using a ticket management system such as Jira, Azure DevOps or Asana which provide a variety of tools that help track project progress, issues and milestones.

The product roadmap can be broken down into Epics, Features and User Stories, creating a backlog of tasks that lead directly to the customers’ requirements. The tasks on the backlog can then be used to plan sprints and allocate tasks to the team to begin development.

### Code
Once the team had grabbed their coffees and had the morning stand-up (daily meeting about upcoming work in the team), the developers can get to work. In addition to the standard toolkit of a software developer, the team has a standard set of plugins installed in their development environments (e.g. Visual Studio, JetBrains Pycharm, IntelliJ IDEA, ...) to aid the development process. Apart from obvious IDE features, it is also to help enforce consistent code-styling and avoid common security flaws and code anti-patterns.

This helps to teach developers good coding practice while aiding collaboration by providing some consistency to the codebase. These tools also help resolve issues that may fail tests later in the pipeline, resulting in fewer failed builds.

Q: What code editors do you use in your work?

### Build
The Build phase is where DevOps really kicks in. Once a developer has finished a task, they commit their code to a shared code repository. There are many ways this can be done, but typically the developer submits a pull request — a request to merge their new code with the shared codebase. Another developer then reviews the changes they’ve made, and once they’re happy there are no issues, they approve the pull-request. This manual review is supposed to be quick and lightweight, but it’s effective at identifying issues early.

Simultaneously, the pull request triggers an automated process which builds the codebase and runs a series of end-to-end, integration and unit tests to identify any regressions. If the build fails, or any of the tests fail, the pull-request fails and the developer is notified to resolve the issue. By continuously checking code changes into a shared repository and running builds and tests, we can minimise integration issues that arise when working on a shared codebase, and highlight breaking bugs early in the development lifecycle.

### Test
Once a build succeeds, it is automatically deployed to a staging environment for deeper, out-of-band testing. The staging environment may be an existing hosting service, or it could be a new environment provisioned as part of the deployment process. This practice of automatically provisioning a new environment at the time of deployment is referred to as Infrastructure-as-Code (IaC) and is a core part of many DevOps pipelines.

Once the application is deployed to the test environment, a series of manual and automated tests are performed. Manual testing can be traditional User Acceptance Testing (UAT) where people use the application as the end customer in order to highlight any issues or refinements that should be addressed before deploying into production.

At the same time, automated tests might run security scanning against the application, check for changes to the infrastructure and compliance with hardening best-practices, test the performance of the application or run load testing. It is usually done as a new testing without interrupting the flow of developers or impacting the production environment. This is done because you don't want to overwrite the production environment with one that is not properly tested.

### Release
The Release phase is a milestone in a DevOps pipeline — it’s the point at which we say a build is ready for deployment into the production environment. By this stage, each code change has passed a series of manual and automated tests, and the operations team can be confident that breaking issues and regressions are unlikely.

Depending on the DevOps maturity of an organisation, they may choose to automatically deploy any build that makes it to this stage of the pipeline. Developers can use feature flags to turn off new features so they can’t be seen by the customers until they are ready for action. This model is considered the nirvana of DevOps and is how organisations manage to deploy multiple releases of their products every day.

Alternatively, an organisation may want to have control over when builds are released to production. They may want to have a regular release schedule or only release new features once a milestone is met. You can add a manual approval process at the release stage which only allows certain people within an organisation to authorise a release into production.

### Deploy
Now, a build is ready for the big time and it is released into production. We can use several tools and processes that can automate the release process to make releases reliable with no outage window (no downtime).

The same Infrastructure-as-Code that built the test environment can be configured to build the production environment. We already know that the test environment was built successfully, so we can rest assured that the production release will go off without a hitch.

A blue-green deployment - two identical deployment environments - lets us switch to the new production environment with no outage. Then the new environment is built, it sits alongside the existing production environment. When the new environment is ready, the hosting service points all new requests to the new environment. If at any point, an issue is found with the new build, you can simply tell the hosting service (web server, DNS) to point requests back to the old environment while you come up with a fix.

### Operate
The new release is now live and being used by the customers. Great work!

The operations team is now hard at work, making sure that everything is running smoothly. Based on the configuration of the hosting service, the environment automatically scales with the load to handle peaks and troughs in the number of active users.

The organisation has also built a way for their customers to provide feedback on their service, as well as tooling that helps collect and triage this feedback to help shape the future development of the product. This feedback loop is important — nobody knows what they want more than the customer, and the customer is the world’s best testing team, donating many more hours to testing the application than the DevOps pipeline ever could. You need to capture this information, it’s worth is weight in gold.

### Monitor
The 'final' phase of the DevOps cycle is to monitor the environment. This builds on the customer feedback provided in the Operate phase by collecting data and providing analytics on customer behaviour, performance, errors and more.

We can also do some introspection and monitor the DevOps pipeline itself, monitoring for potential bottlenecks in the pipeline which are causing frustration or impacting the productivity of the development and operations teams.

All of this information is then fed back to the Product Manager and the development team to close the loop on the process. It would be easy to say this is where the loop starts again, but the reality is that this process is continuous. There is no start or end, just the continuous evolution of a product throughout its lifespan, which only ends when people move on or don’t need it any more.

## Tools used in DevOps processes
Do you know any tools that you'd use in each of the phases below?

 * Plan
 * Code
 * Build
 * Test
 * Release
 * Deploy
 * Operate
 * Monitor

List of tools can be found [here](https://engeto.com/cs/kurz/introduction-to-devops/studium/pxFaiYQsQnq6v_U1dMUK9g/environment-and-tools-of-devops/overview-of-tools).

## DevOps and Agile development 
Q: What is Agile development?

Agile software development has broken down some of the silos between requirements analysis, testing and development. Deployment, operations and maintenance are other activities which have suffered a similar separation from the rest of the software development process. The DevOps movement is aimed at removing these silos and encouraging collaboration between development and operations.

We can say, that DevOps builds on Agile development practices and takes it even further. In a nutshell, Agile development is a systematic approach to software development with focus on rapid iteration based on customer feedback. DevOps is a concept (set of practices), that has focus on collaboration between development and operations with the goal to reduce time for development cycle. This goal can be achieved by effective collaboration between Dev and Ops teams and automation of the process. **DevOps is therefore in complement to agile development.**

Let's break it down in the following images.

**Stakeholders and communication chain in a typical IT process:**
<p align="center">
  <img src="assets/typicalitprocess.png" alt="Typical IT Process">
</p>

**Agile addresses gaps in Customer and Developer communications:**
<p align="center">
  <img src="assets/agilega.png" alt="Agile Gap">
</p>

**DevOps addresses gaps in Developer and IT Operations communications:**
<p align="center">
  <img src="assets/devopsga.png" alt="DevOps Gap">
</p>

The approach to **software development** has gone through the following evolution:
 * Chaos
 * Waterfall
 * **Agile development**
 * **DevOps**

## Task at the end
You are encouraged to go through scenarios about Git - to test your skills in this version control system. 

They are available at:
 * https://katacoda.com/courses/git
 
Furthermore, you should prepare the following:
 * Virtual machine with CentOS 8 that we'll use during the course
