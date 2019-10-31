+++
title = "Why did we create the POET Pipeline?"
description = "Initial project description"
date = "2019-10-31"
author = "Sarat Rajan"
sec = 1
+++

<img src="https://raw.githubusercontent.com/wiki/tmobile/POET-pipeline-library/images/POET_logo_final-480.png"
     alt="POET-logo"
      />

The POET pipeline is designed around leveraging a dynamic DevOps culture. Developers should spend their time on development, not creating and maintaining their CI/CD pipeline, be able to on-board their solutions to the pipeline without having to be Jenkins “(R).” experts. POET pipeline provides recognized value to Devops teams without compromising the quality.

Values such as:

- Make it **easier to implement new pipeline capabilities**, without having to impact pipeline users.
- Make pipeline usage and onboarding faster and easier.
- Designing a service for **scalability, reusability and flexibility** across Dev teams. 
- Help teams **avoid having their own CI/CD pipeline specialists** to maintain their own custom pipeline. 
- Continue to **abstract the underlying technologies** that drive the pipeline (no need to know about Jenkins and associated tool chain).

# What is the POET pipeline framework?

The POET pipeline framework is built with a containers-first architecture. Pipelines are configured using a YAML files that you check-in to your git repository. The syntax is designed to be easy to read and expressive so that anyone using the repository can understand the continuous delivery process.

POET Pipeline executes build, test and deployment commands against your code inside isolated containers. 

### Example representation of a pipeline workflow
<img src="https://opensource.t-mobile.com/blog/poet-pipeline/workflow.png"
     alt="POET-workflow" style="width:900px;"
      />

Jenkins Groovy code is limited, error-prone, and difficult to incorporate with 3rd party libraries. For these reasons, our approach has been to keep the core pipeline code small, and push functionality out into containers.

One of the key design features is that we define a pipeline as a list of steps that include building, testing, and deploying code, along with sending notifications, or any other type. Each step is self-contained and implemented as a container. The pipeline workflow is responsible for executing each step but does not need to understand the step container internals. Step containers are a key strategy to empowering teams to develop their own containers to solve unique problems within their CI/CD, but they can also use existing containers developed by our team for immediate use.

## Managing and Running a CI/CD pipeline is complex

Below is a diagram that looks to depict the different aspects of managing a CI/CD pipeline. Often a team building their own pipeline doesn’t have time to do all these items and they tend to do “just enough” to run but the solution doesn’t provide the robustness one is typically looking for in a pipeline critical to a highly available CI/CD flow. Doing it as a one off also consumes a greater percentage of a development team’s time.

This often moves organizations or teams to a more centralized approach, but this can create too “prescriptive” of a solution that doesn’t leave engineering teams the flexibility they need. To that end the POET pipeline looks to bridge that gap where we could have a reusability of capabilities, eliminate the need for “deep” knowledge of Jenkins for development teams.
