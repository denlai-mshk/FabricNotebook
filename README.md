
# Microsoft Fabric Shortcut: Sink incremental data from Dataverse to Azure
Microsoft Dataverse direct link to Microsoft Fabric enables organizations to extend their Power Apps and Dynamics 365 enterprise applications, and business processes into Fabric. The Link to Microsoft Fabric feature built into Power Apps makes all your Dynamics 365 and Power Apps data available in Microsoft OneLake, the built-in data lake for Microsoft Fabric.

- No need to export data, build extract, transform, load (ETL) pipelines, or use our partner integration tools.
- With shortcuts from Dataverse directly into OneLake, your data stays in Dataverse while authorized users get to work with data in Fabric.
- Link data from all Dynamics 365 apps, including Dynamics 365 Finance and Operations apps.

![story](/fabric_arch_diagram.png)


# Notebook
These notebooks enable you to read data from Dataverse and write to ADLS2 or PostgreSQL incrementally
- No OneLake storage is needed
- Support near-real-time updates by setting a short-period scheduled trigger
- ensuring all data transit occurs within a private network
- leverage Fabric Workspace Identity to simplify the authorization workflow
- Use Dynamics365 Customer Insight Journey, marketing data {EmailOpened / EmailClicked} as datra source
 
  [sink to ADLS2 (CSV, JSON)](/writedata_ADLS2)

  [sink to PostgreSQL database](/writedata_PostgreSQL)

# Setup Workflow
- This reference guideline help you to setup the privatelinks as well as the Fabric shortcut and Notebook.

  [Guideline](/fabric_notebook_workflow.pdf)

# References
 - [Set up and use private links for secure access to Fabric - Microsoft Fabric | Microsoft Learn](https://learn.microsoft.com/en-us/fabric/security/security-private-links-use#step-5-create-a-private-endpoint)

 - [Link your Dataverse environment to Microsoft Fabric and unlock deep insights - Power Apps | Microsoft Learn](https://learn.microsoft.com/en-us/power-apps/maker/data-platform/azure-synapse-link-view-in-fabric#create-a-connection-to-your-dataverse-environment)