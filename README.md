# Online Service Catalogue - for Public Sector Organisations
A Public Sector tailored service catalogue sample solution, which runs on Microsoft Power Pages, Dataverse, Power Apps and Copilot Studio. The solution's super power, is that it allows non-technical people to create forms and form fields e.g. application form, through a simple user interface, without having to create table(s) or use Power Pages to create the form. It also supports configurable Microsoft Office forms, and Power Page basic and multi-step forms.

## Background
This is provided as a solution accelerator. It's a sample solution which is not supported by Microsoft or myself. Use it as a starter/accelerator to help you get going quickly. It allows for non-technical people to define online services and associated forms for these services. These services are then rendered on the web site (Power Pages), and citizens can search or browse for services, and interact with the service e.g. complete an application form. This solution uses the Dataverse for storage, and has both a Model Driven application (for the service and form management) and a Power Pages site as the site for citizens.

Here is a video overview of the solution

- [Solution Demonstration](https://youtu.be/FpwpNxEsTxw)

## Features
Here is a list of core features of the solution

- Define online services, departments, forms, office location and review submissions from citizens from a model driven Power App.
- Citizens navigate or search for services in the portal, and interact with the online service via external web link, Microsoft Office Form, Power Pages form or custon defined user driven form
- View all service submissions in a central place, both for citizens and the organisation

## How it works
There are 2 main applications which makeup this solution. 1 - Model Driven App (Service Catalogue Manager) 2 - Citizen Web Site (Power Pages). The Power Pages site was based off the blank site templates and uses the enhanced data model and Bootstrap v5.

![Model App and Web Site](https://github.com/m-odonovan/PSServiceCatalog/blob/main/images/psservice.gif?raw=true "Model App and Web Site")

## Installation
There are 2 unmanaged solution files which need to be imported into a Power Platform environment for the solution to work.
1 - Government Online Services - import this one first. This contains the Dataverse tables and Model Driven App.
2 - Government Online Services Portal - this contains the Power Pages web site and its related components. Once this has been imported, navigate to make.powerpages.microsoft.com, and select inactive web sites tab. You will find this government web site there, activate it and use it.

Once imported, use the model driven app to setup departments, categories and services.

## Provided "As-Is"
This is a a starter / sample. It hasn't been well tested, and is missing some key features that I hope to add over time. It not officialy supported by myself or Microsoft. However, because the unmanaged and managed solution is provided, you should be able to support it yourself, either directly or through a certified Microsoft partner.


