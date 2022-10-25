# About

This is a hobby project created with UiPath. Steps performed by this automation:

- Open Nettiauto.com website.
- Enter search criteria and open the search results.
	- Note: It would make sense to add some search filters in Nettiauto itself. However, as this is a demo project, we will filter the results post search with UiPath activities.
- Extract the search results as datatable.
- Do some extra filtering on the datatable.
	- Note: If one would desire more results, it would make sense to bundle the filtering with the scraping, since with current setup it could be possible to get very few filter results.
- Write the datatable as Excel file on the users desktop.

The automation reuses some parts of ReFramework, but due to the simplicity, Main workflow is modelled as a Sequence. In case of exception in Initialization or Process, an exception screenshot is saved to location specified by Config Excel.

# Instructions

- Make sure to allow UiPath Edge extension to work in InCognito mode. See https://docs.uipath.com/studio/docs/microsoft-edge-extension-troubleshooting#Enable%20access%20to%20file%20URLs%20and%20InPrivate%20mode for instructions if needed.
- **IMPORTANT** If you use Edge browser: Before running the automation, make sure to save your work. The robot kills the msedge process so there is possibility  to lose unsaved data.