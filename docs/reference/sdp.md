# Software Delivery Platform

The Solutions Delivery Platform (SDP) is an accumulation of Booz Allen’s lessons learned implementing DevSecOps practices across multiple client projects and RFP Tech Challenges.

It's an open source and reusable pipeline framework that jump starts projects. SDP has allowed the typical time to develop a pipeline from 3 to 4 months down to just a week.

Instead of creating per-application pipelines, SDP allows you to create tool-agnostic, templated workflows that can be used by multiple teams to achieve organizational governance.

## Components

Of the SDP components UIP incorporates the following:

### Jenkins Templating Engine (JTE)

The Jenkins Templating Engine is a custom plugin written by Booz Allen that enables the capabilities of the Solutions Delivery Platform; such as organizational governance through templating and hierarchical configuration files.

> This plugin is available in the Jenkins Update Center under the name Templating Engine Plugin.

#### How Does It Work?

JTE allows pipeline developers to create common workflows (called pipeline templates) and share them across teams. These workflows define the business logic of your pipeline in a tool-agnostic way by calling generic functions (called steps). These functions are then implemented by one or more reusable modules (called libraries).

Each team is able to tailor the pipeline template through their own pipeline configuration. The pipeline configuration declares which libraries to load prior to executing the pipeline template.

Through this approach, the same pipeline template can be reused for an arbitrary number of teams, each with their own tool integrations, by loading different libraries.

Additional Documentation: [Click Here](https://boozallen.github.io/sdp-docs/jte/2.2.2/index.html)

### Sonarqube

SonarQube is a tool used for static code analysis. Static code analysis is validating code as-written against industry standard practices. It will help you find best practice violations and potential security vulnerabilities.

Organizations can define Quality Profiles which are custom rule profiles that projects must use. Quality Gates are then rules defining the organizational policies for code quality. SDP will, by default, fail the build if the Quality Gate fails.

Additional Documentation: [Click Here](https://boozallen.github.io/sdp-docs/sdp-libraries/libraries/sonarqube.html)
