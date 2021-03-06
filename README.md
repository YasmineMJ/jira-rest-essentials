# JIRA REST Essentials

This JIRA plugin exists to close some gaps of the [JIRA REST API](https://docs.atlassian.com/jira/REST/ondemand/). 

### FieldScreen

#### `GET /rest/essentials/1.0/screen`

* lists all screens by id and name

#### `GET /rest/essentials/1.0/screen?projectKey={projectKey}`

* lists all screens associated with a given project

#### `GET /rest/essentials/1.0/screen?name={screenName}`

* returns the id for a screen with the given name

### CustomField

#### `GET /rest/essentials/1.0/customfield/description`

* lists all custom field descriptions by field (with prefix `custom_*`)

#### `GET /rest/essentials/1.0/customfield/description?id={id}`

* returns a custom field description for a given field (id as `long` without prefix)

---

### Build the Add-on ###

* Use Maven to build a deployable jar file: `mvn clean package`