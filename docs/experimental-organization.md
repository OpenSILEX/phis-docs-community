# Experimental Organization

## Projects

### What are projects ?
A project is the higher level of organisation in PHIS.
A single experimentation can include several experiments from various experimental campaigns.

### What are project properties ?
Projects fact sheets are all public, i.e. visible for every PHIS user, including those unrelated to them.
However, experiments and objects included in a project are accessible only to the users defined as owner or guest of this project.

### Create a project
Within the `Projects` menu, one can create a new project with the
<span class="btn btn-success">Create Project</span> button.

Tool tips are provided for most fields: they appear on the left hand side when one drags the pointer on those fields.

The mandatory fields, followed by an asterisk, are:
- acronyme
- name
- date (start / end)

However, it is highly recommended to fill every field. If possible, fields requiring plain text (keywords, description) should be answered to in english.

`URI`. The project URI is automatically created using the acronym provided by the user.

`Acronym`. Short and meaningful, the acronym will be the preferred way to refer to the created project.
A project acronym cannot include spaces.

`Name`. Full name of the project, it will seldom be refered to but allows a project creator to explicit the acronym, e.g. the name "RAPeSeed Oil content anD Yield under low Nitrogen input" would be adequate for the project whose acronym is "RAPSODYN".

`Subproject Of`. If the new project is part of an existing project (requisitly known to PHIS), one can select the name of the given mother-project within the exhaustive list of projects to which the user has access.

`Subproject Type`. The subproject type can optionnaly be provided. It can be either an existing type to be selected from the list of proposed project types, either a new type provided by the user. In the later case, one has to type the new subproject type (e.g. "phd thesis" or "internship") in the search field of `Subproject Type` and then click on the newly proposed type.

![Subproject-type](img/create-project_subproject-type.png)

`Objective`. A short synthesis of the project objectives is to be provided in plain text, preferably in English. A more complete description will be asked in the `Description` field.

`Financial Support`. Organism, institution or funding agency providing the financial support of the research project. Only one organism supporting financially the project can be cited for now. Same as the **Subproject Type** field, the answer can be both from a predefined list or a new one (the user has to type the new organism name and then click on the search result matching the organism name).

`Financial Name`. As indicated in the tool tip, this field is meant for the user to provide the identification of the financial support document (e.g. a grant agreement number).

`Date Start` and `Date End` are to be provided in the format YYYY-MM-DD (year-month-day), directly or through the calendar view. If the end date of the project is unknown, the start date can be reused in `Date End` temporarily. *TO CHECK*

`Scientific Contacts`. Email adresses of the scientists involved in the project.
The email adresses refer uniquely to persons existing on Phis.
If unavailable in the predefined list, emails can be added to Phis from the `Persons` menu, prior to the new project creation. Please see the [Persons](../community/#persons) section of this documentation for further details.

`Administrative Contacts`. Email adresses of the administrative personnel linked to the project (e.g. human ressources people).
The email adresses refer uniquely to persons existing on Phis.

`Project Coordinators`. Email adresses of the project coordinators.
The email adresses refer uniquely to persons existing on Phis.

`Website`. If available, URL of the website of the project.

`Keywords`. Each keyword should  be separated by a comma, e.g. *drought, maize*.

`Description`. Complete plain text description of the project, preferably provided in english language. Additionally to the description, informations can be provided as uploaded files, after the project has been created.

## Experiments

### What are experiments ?
...

### What are experiment properties ?

<span class="btn btn-primary">Update</span>

<span class="btn btn-warning">Add document</span> This button remains orange until a first document has been added to the experiment.

<span class="btn btn-info">Map Visualization</span>
<span class="btn btn-success">Generate Map</span>

### Create an experiment

## Agronomical Objects

### Object types
plot : link toward AGROVOC: smallest unit (one treatment maximum per plot)

block: combination of plots

field : ...

### Importing Objects

| Alias          | Geometry       | ExperimentURI  | Species     | Variety | ExperimentModalities | Repetition |
| :------------- | :------------- | :------------- | :---------- |:------------- | :------------- | :--------- |
| platformXXX-experimentYYY-plotZZZ       | POLYGON (( ... ... , ... ... ))       | http&#58;//www.phenome-fppn.fr/.../...   | http&#58;//www.phenome-fppn.fr/id/species/...    | variety-1      | nitrogen-1     | 1 (or A-I)     |


## Variables

### Phenotypic variables

### Environmental variables
