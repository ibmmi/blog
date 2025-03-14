# Mihai's Personal Blog

- [Mihai's Personal Blog](#mihais-personal-blog)
  - [What's New](#whats-new)
    - [Attempting to switch from Rancher Desktop to Podman Desktop](#attempting-to-switch-from-rancher-desktop-to-podman-desktop)
  - [About Me](#about-me)

## What's New


### [Attempting to switch from Rancher Desktop to Podman Desktop](./articles/2025/03.March/01.Switch2PD.md)

I have been using linux containers for the last 5 years. I really appreciate WSL2 as it enabled a series of virtuous use cases for Windows users.
In my case, Docker Desktop broke the ice and I had to switch to Rancher Desktop due to licensing issues a few years back.
Now, with the acquisition of webMethods by IBM, I am considering RedHat capabilities more intensely.
I have tried Podman Desktop some time ago and it was not responding to the needs. This week I gave it another go. Let's see [how it went](./articles/2025/03.March/01.Switch2PD.md). 

## About Me

I am a veteran webMethods software architect, currently working in IBM. I have arrived in IBM contextually to the webMethods suite acquisition from Software AG in 2024.

I am keeping separate GitHub profiles according to my employment status. My previous GitHub user, as a Software AG employee, was `miunsag`.

All content in this personal public GitHub space is open source, licensed with the Apache 2.0 license and represents personal contributions. This content is thus not representing IBM or Software AG official positions or commitments of any nature.

Contents I publish in GitHub gravitate around webMethods software delivery, both in terms of installations and development of application components. I am pushing the technology boundaries towards real continuous delivery, providing real world executable use cases following some fundamental principles, including:

- relentless automation
- all code, including application, installation, infrastructure setup, configuration must be managed in source control
  - no "manual" procedures or click adventures
- ephemeral environments
  - only product needs to be permanent, everything else should be ephemeral and thus quickly spinnable on demand
- continuous integration
  - integrate team contribution into a main versioning line, the trunk, multiple times a day. This is also called "trunk based development".
  - avoid branching
- delivery and deployment pipelines
  - all delivery and deployment must be automated behind source control changes
- comprehensive testing
  - implement automation for all types of tests necessary for the delivery. Obviously allow users to spin environments and explore if they want to.
  - testing must be executed in production like ephemeral environments
- shift left
- relentless improvement
- allow for feature toggles, canary deployments and similar DevOps techniques

Moreover, considering the usual webMethods users pain points, the following goals are also pursued:

- deterministically repeatable delivery. 
  - no more "it works for me" or "it works in test, but not production"
  - avoid the [snowflake servers](https://martinfowler.com/bliki/SnowflakeServer.html) phenomenon
- version independence.
  - minimize the friction around version upgrades
  - instantaneous fix levels and version upgrades for service development
- advanced containerization
- cloud adoption, i.e. deploy webMethods in hyperscalers
- orchestration independent DevOps and Continuous Delivery
