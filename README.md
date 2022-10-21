# About

This is a hobby project created with UiPath. Steps performed by this automation:

- Open Nettiauto.com website.
- Enter search criteria and open the search results.
	- Note: It would make sense to add some search filters in Nettiauto itself. However, as this is a demo project, we will filter the results post search with UiPath activities.
- Extract the search results as datatable.
- Do some extra filtering on the datatable.
- Write the datatable as Excel file on the users desktop.

# Instructions

- Make sure to allow UiPath Edge extension to work in InCognito mode. See https://docs.uipath.com/studio/docs/microsoft-edge-extension-troubleshooting#Enable%20access%20to%20file%20URLs%20and%20InPrivate%20mode for instructions if needed.