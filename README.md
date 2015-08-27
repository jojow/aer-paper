# Supplementary Material for AER Paper

Supplementary material for the paper "Enabling DevOps Collaboration and Continuous Delivery Using Diverse Application Environments"



## DevOps Lifecycle

In the following, we outline the DevOps lifecycle, which we follow in the paper. It consists of a *dev-centric* and an *ops-centric* phase:

![DevOps Lifecycle](/devops_lifecycle.png)



## Application Environment Requirements (AERs)

We consider *application environment requirements (AERs)* as a specific class and subset of non-functional requirements:

![Application Environment Requirements (AERs)](/requirements_scope.png)



## AER Classification

First of all, an AER may be relevant for a single or multiple environments (development, test, production, etc.).
Thus, AERs can be classified according to the **(i) environment** dimension, i.e., which environments they target.
In addition, we identified another orthogonal categorization of AERs, namely *application-specific* and *common* AERs such as requirements that are not bound to the application but bound to a specific organizational unit; these may appear on different levels, such as a company, a department, or a team.
This is the **(ii) scope** dimension for AERs.
Finally, the **(iii) type** dimension characterizes AERs on a technical level by considering multiple sub-dimensions such as:

* Inclusive requirement *(e.g., environment must use Git)* vs. exclusive requirement *(e.g., environment must not use Subversion)*
* Immediately required *(e.g., environment must contain a PHP runtime)* vs. eventually required *(e.g., environment must be eventually hosted on an Ubuntu OS)*
* Existence *(e.g., environment requires a PHP runtime)* vs. property-value match *(e.g., environment requires PHP version 5.5 or better)*

Example: the AER *Web shop development environment requires Git version 2.1.3* is an *inclusive, immediate,* and *property-value match* type of requirement, scoped to the Web application, and relevant for development environments only.



## Knowledge Base

Our approach to resolve AERs (attached to unresolved topologies) based on a knowledge base is outlined in the following:

![Knowledge Base](/knowledgebase.png)



## Knowledge Base Model

The knowledge base is structured an centered around multiple taxonomies (Middleware, Infrastructure, Supplementware, etc.) to categorize the solutions and implementations it contains:

![Knowledge Base Model](/knowledgebase_model.png)



## Evaluation

Based on the Web shop application (our motivating scenario and running example), we conducted an [evaluation](evaluation.pdf) to show that AERs can be systematically resolved using the knowledge base to create topologies, which are then utilized to establish diverse application environments.
