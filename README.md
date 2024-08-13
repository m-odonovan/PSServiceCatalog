# Online Service Catalogue - for Public Sector Organisations
Public sector service catalogue sample solution, which runs on Microsoft Power Pages, Dataverse, Power Apps and Copilot Studio. The solutions super power, is that it allows non technical people to define forms and form fields to render on web site for citizens to complete. These forms don't need to be created in Power Pages, but can be if you would like.

## Background
This is provided as a solution accelerator. It's a sample solution which is not supported by Microsoft or myself. Use it as a starter/accelerator to help you get going quickly. It allows for non-technical people to define online services and associated forms for these services. These services are then rendered on the web site, and citizens can search or browse for services, and interact with the service e.g. complete an application form. This solution uses the Dataverse for storage, and has both a Model Driven application (for the service and form management) and a Power Pages site as the site for citizens.

Here is a video overview of the solution

- [Solution Demonstration](https://youtu.be/FpwpNxEsTxw)

## Features
Here is a list of core features of the solution

- Define Indicator and Data Element templates. These are used to generate indicators/elements for collection, based on reporting period i.e. Anually / Quarterly
- Allow users who are assigned indicators (via their business unit), to save values as draft and submit final values. Users can submit value or reasoning for no values. Along with other comments as per Circular 88.
- Send reminders to users who haven't submmited yet
- Allow for user defined formula for each indicator based on child data elements e.g. in some cases it could be sum of values of all child elements, and sometimes more complex forumal e.g. (child1 + child2) * 365 / 3

## How it works
There are 2 main applications which makeup this solution. 1 - Admin Model Driven App (Indicator Manager) 2 - User Indicator Canvas App. All data resides in the Microsoft Dataverse. There are a few Power Automate Flows which are used to notify users to submit their indicators, or to setup indicators, perform rollup calculations and more.

![Model and Canvas App](https://github.com/m-odonovan/Circular88-KPI/blob/main/images/Circular88GIF.gif?raw=true "Model and Canvas App")

## Video Demos

- [Solution Demonstration](https://youtu.be/7LnTThswnD8)
- [Under the hood, how it works](https://youtu.be/vPHJJu4UMMc)

## Installation
There are 2 solution files which need to be imported into a Power Platform environment for the solution to work.
1 - Calculation Connector solution - this contains a custom connector only. This connector is used for C# based formula logic, and doesnt actually connect to any backend service. This must be imported first.
2 - Circular 88 solution - this contains the rest of the solution i.e. model driven app, canvas app, several flows, several tables, some web resources and a few custom roles.

Once imported, use the model driven apps setup section to add a default settings record, add Collection Business Unit records and Unit of Measure records. There are 3 custom roles which users will need to be assigend to i.e. Performance Indicator User, Performance Indicator Manager, and Performance Indicator Admin.

## Provided "As-Is"
This is a a starter / sample. It hasn't been well tested, and is missing some key features that I hope to add over time. It not officialy supported by myself or Microsoft. However, because the unmanaged and managed solution is provided, you should be able to support it yourself, either directly or through a certified Microsoft partner.


