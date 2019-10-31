+++
title = "Why did we create POET Pipeline?"
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

# What is POET pipeline framework?

The POET pipeline framework is built with a containers-first architecture. Pipelines are configured using a YAML files that you check-in to your git repository. The syntax is designed to be easy to read and expressive so that anyone using the repository can understand the continuous delivery process.

POET Pipeline executes build, test and deployment commands against your code inside isolated containers. 
