# Experimental Organization

## Projects

### What are projects ?
A research project is the higher level of organisation in Phis.
It is generally the object of a contract or a grant agreement between the laboratory performing the research activities and funding agencies providing the financial support.
A project can hold many experiments from various experimental campaigns.
Besides, several projects can participate to the same experimentation.

### What are project properties ?
Projects fact sheets are all public, i.e. visible for every Phis user, including those unrelated to them.
However, experimental data included in a project is also necessarily related to a given experiment.
This data is accessible only to users who belong to a group (either owner or guest) authorized to access the experimentation it is related to: access rights are managed by experiment and not by project.
Please see the [Restrictions to a group](../community/#restrictions-to-a-group) section of this documentation for further details on data access matters.

The complete list of projects is available in the `Projects` menu, accessible from Phis top navigation bar.
The projects list is preceded by a research bar enabling the user to filter projects by their acronym, their main source of funding, and their start and end dates.
There's no need to use the same case as the expected results: a lowercase search returns every results matching the characters, disregarding whether those match are lowercase or uppercase.
Further information on a given project is available on its information sheet, accessed to from the projects list through the eye-icon on the right-hand side of this project row.

![project-menu](img/projects-list_eye-icon.png)

### Create a project
Within the `Projects` menu, one can create a new project with the
<span class="btn btn-success">Create Project</span> button.

Tool tips are provided for most fields: they appear on the left hand side when one drags the pointer on those fields.

![tooltips](img/create-project_tooltips.png)

The mandatory fields, followed by a red asterisk, are:

- acronyme
- name
- date (start / end)

However, it is highly recommended to fill every field. If possible, fields requiring plain text (keywords, description) should be answered to in English.

`URI`. The project URI is automatically created using the acronym provided by the user.

`Acronym`. Short and meaningful, the acronym will be the preferred way to refer to the created project.
The acronym provided here is usually the one of the research project.
A project acronym cannot include spaces.
Once the project created, its acronym can no longer be modified.

`Name`. Full name of the project, it will seldom be refered to but allows a project creator to explicit the acronym. For instance, *RAPeSeed Oil content anD Yield under low Nitrogen input* would be an adequate name for the project whose acronym is *RAPSODYN*.

`Subproject Of`. If the new project is part of an existing project (requisitly known to Phis), one can select the name of the given mother-project within the exhaustive list of projects registered to the Phis instance where the new project is created.

`Subproject Type`. The subproject type can optionnaly be provided. It can be either an existing type to be selected from the list of proposed project types, either a new type provided by the user. In the later case, one has to type the new subproject type (e.g. *phd thesis* or *internship*) in the search field of **Subproject Type** and then click on the newly proposed type.

![subproject-type](img/create-project_subproject-type.png)

`Objective`. A short synthesis of the project objectives is to be provided in plain text, preferably in English. A more complete description will be asked in the **Description** field.

`Financial Support`. Organism, institution or funding agency providing the financial support of the research project. Only one organism supporting financially the project can be cited for now. Same as the **Subproject Type** field, the answer can be both from a predefined list or a new one (the user has to type the new organism name and then click on the search result matching the organism name).

`Financial Name`. As indicated in the tool tip, this field is meant for the user to provide the identification of the financial support document (e.g. a grant agreement number).

`Date Start` and `Date End` are to be provided in the format YYYY-MM-DD (year-month-day), directly or through the calendar view.

???

If the end date of the project is unknown, the start date can be reused in `Date End` temporarily. *TO CHECK*

`Scientific Contacts`. Email adresses of the scientists involved in the project.
The email adresses refer uniquely to persons existing on Phis.
If unavailable in the predefined list, emails can be added to Phis from the `Persons` menu, prior to the new project creation. Please see the [Persons](../community/#persons) section of this documentation for further details.

`Administrative Contacts`. Email adresses of the administrative personnel linked to the project (e.g. human ressources people).
The email adresses refer uniquely to persons existing on Phis.

`Project Coordinators`. Email adresses of the project coordinators.
The email adresses refer uniquely to persons existing on Phis.

`Website`. If available, URL of the website of the project.

`Keywords`. Keywords, preferably in English, characterizing the project. Each keyword should be separated by a comma and not include any capital letter, e.g. *drought, maize*.

![keywords](img/create-project_keywords.png)

`Description`. Complete plain text description of the project, preferably provided in English language. Additionally to the description, additional information can be provided as uploaded files, after the project has been created.

## Experiments

### What are experiments ?
Field plant phenotyping experimentations are refered to in Phis2 as **Experiments**.
Experiments in Phis form self-sustained organizational units occuring in a delimited and known time frame.
Every agronomical objects and environmental data stored in Phis field have to be related to an experiment.
Experiments include both raw and cleaned data.
The data types found in Phis experiments are including but not limited to :
- phenotypic data
- environmental data
- analysis, workflows and their associated results

### What are experiment properties ?
Contrary to projects, experiments information sheets are not public, but accessible only to the Phis members which are part of the groups involved in these experiments.
Please go to [Access rights](../community/#access-rights) for further details on this matter.

From the `Experiments` menu, a Phis user has access to the list of experiments it has the rights to access to.
Every experiment on this list is characterized by :

- its **URI** which identies it uniquely
- its **Alias**, a short internal denomination
- its stat and end dates
- the experimental installation in which is has been performed
- the campaign it is part of, i.e. the year

From **Home / Experiments**, one can click on the eye icon on the right to see a given experiment information sheet.
Further information on the experiment is provided on this information sheet, such as the groups of users that have been given access to the experiment's data.
For more detail on experimental data access restrictions, see the section [Restrictions to a group](../community/#restrictions-to-a-group).

On top of the experiment information sheet, several buttons are displayed.
The buttons <span class="btn btn-info">Map Visualization</span> and <span class="btn btn-success">Generate Map</span> enable the visualization of the agronomical objects (e.g. plots) of the experiment on a map centered on the experiment intallation location.
The use of the other buttons is described at the end of the next section entitled [Create an experiment](../experimental-organization/#create-an-experiment).

### Create an experiment
Within the `Experiments` menu, a Phis user can create a new experiment with the
<span class="btn btn-success">Create Experiment</span> button.

Tool tips are provided for some fields: they appear on the left hand side when one drags the pointer on those fields.

The mandatory fields, followed by an asterisk, are:

- projects
- date (start / end)
- campaign

However, it is highly recommended to fill every field. If possible, fields requiring plain text (keywords, description) should be answered to in English.

`URI`. The project URI is automatically created by Phis web service which uses the acronym of the Phis instance from where the experiment is created (e.g. *DIA* for Diaphen) and the **campaign** provided by the user (e.g. *2018*).

`Alias`. Internal name of the experiment, usually provided in all caps.

`Projects`. Name of the project(s) the new experiment is part of.
A single experiment can be linked to several projects.
One can select the name of the given projects only within the exhaustive list of projects registered to the Phis instance where the new experiment is created.

`Date Start` and `Date End` are to be provided in the format YYYY-MM-DD (year-month-day), directly or through the calendar view.
It it compulsory to give a value to the **Date End** field in order to create an experiment.
If the end date of the experiment is unknown, the start date can be reused in **Date End** temporarily.
Typical **Date Start** values correspond to a sowing date, while **Date End** typically concur with an harvesting date.

`Installation`. Name or ID of the installation where the experiment is carried.
No specific format is yet required for submitting an installation name. *todo*.

`Campaign`. Year (format YYYY) in which the experiment has been carried, or the year of the harvest/end of the experiment in case it has been carried on several years (*to be confirmed*).
Once the experiment created, the information on the campaign in which it has been carried can no longer be modified.

`Place`. Locality or town name used internally to situate the installation location.
This field will later be removed in the upcoming developments of Phis.

`Scientific supervisors`. Email adresses of the experiment supervisor(s).
The email adresses refer uniquely to persons existing on Phis.
If unavailable in the predefined list, emails can be added to Phis from the `Persons` menu, prior to the new project creation. Please see the [Persons](../community/#persons) section of this documentation for further details.

`Technical supervisors`. Email adresses of the technicians and scientists (including phd students, interns, etc.) involved in the experiment implementation.
The email adresses refer uniquely to persons existing on Phis.

`Crop Species`. Common name of the crop species which are the object of the experiment.
Each crop species names must be separated by a comm.
Preferably provided in English, without any capital letters.
A link to the internal ontology is under development.

`Groups`. List of the Phis users groups authorized to access the new experiment.
This field is crucial when creating an experiment.
Only a Phis user belonging to at least one of the groups specified in this field will be authorized to access the newly created experiment.
An experiment assigned to no group is by default set as public.
Please go to [Access rights](../community/#access-rights) for further details on this matter.

`Objective`. A short synthesis of the experiemnt objectives is to be provided in plain text, preferably in English. A more complete description will be asked in the **Comment** field.

`Keywords`. Keywords characterizing the experiment. Each keyword, should be separated by a comma and not include any capital letter, e.g. *nitrogen use efficiency, rapeseed*.

`Comment`. Complete plain text description of the experiment, preferably provided in English language. Additionally to the description, detailed knowledge on the experimentation can be provided through uploaded files, but only after the experiment has been created.

Completing the experiment creation within Phis is then achieved by clicking on the <span class="btn btn-success">Create</span> button.

From **Home / Experiments**, one can click on the eye icon on the right to see the newly created experiment information sheet.

The <span class="btn btn-warning">Add document</span> button at the top of the experiment sheet remains orange until a first document has been added, e.g. an experimental design.
See the [Documents](../experimental-organization/#documents) section below for further information on documents.

Once created, the experiment specifics can be modified with the <span class="btn btn-primary">Update</span> button.

## Documents

### What are Phis documents ?

In order to ease the comprehension of projects and experiments, it is possible to upload various documents Phis and connect them to projects or experiments.
The same document can be linked to several projects and experiments.
A document can be related to no project nor experiment, but this is not recommanded.
Documents that could help persons understand a project are typically (reasearch) contract, phd (or master) thesis, or various multimedia content such as photos or beamer presentations.
Similarly, one could expect knowledge about an experimentation to be provided through documents that could be protocols, experimental designs, technical or scientific files, data files, research papers, etc.
Examples of document formats are PDF, txt, csv, png images, etc.
However, large files are not yet supported by Phis: a document cannot exceed 2MB.

The documents uploaded to Phis through the `Documents` section are meant for human consultation.
However, metadata (intelligible to machines) must be provided for every new document.
These metadata contain the document properties:

- title
- creator
- language
- creation date
- document type

Information of a document can later be changed, while the document itself cannot be modified.

Metadata are specified with [Dublin Core](http://dublincore.org/documents/dc-rdf/) recommendations.
Metadata enables the documents to be stored in the Phis triplestore.

### Upload a document

Within the `Documents` menu, as well as from a project or experimentation information sheet, any Phis user can upload a new document and specify its metadata with the <span class="btn btn-success">Create Document</span> button.
No admin rights are required from a Phis user to add a new document.

`Title`. Title of the uploaded document.
No specific naming convention is required for filling this field.
A document title does not have to match the name of the uploaded file it is imported from.

`Creator`. Name(s) of the document creator(s), separated by commas
No specific naming convention is required for filling this field.

`Language`. Language in which the document is provided.
In accordance to the [Dublin Core Element Set v1.1](http://dublincore.org/documents/1999/07/02/dces) document, the value of the language element is defined by [RFC 1766](http://www.ietf.org/rfc/rfc1766.txt) which includes a two-character language code taken from the [ISO639](http://xml.coverpages.org/iso639a.html) standard.
The language code should be provided in lower case (e.g. *fr* for French, *en* for English, etc.).

`Creation Date`. Date of the document creation.
If unkown, the current date (i.e. the date at the moment of the document upload into Phis) can be used.

`Concerned Projects`. Project(s) for which the document is relevant.
One can select the name of the given project(s) only within the exhaustive list of projects registered to the Phis instance where the new document is uploaded.

`Concerned Experimentation`. Experiment(s) for which the new document is relevant.
A Phis user can select the name of the given experiment(s) only within the exhaustive list of experiments it has access to.

`Document Type`. The nature of the document's content.
A single type has to be selected from a predefined list.
Only one doucment type can be selected.
Phis controlled vocabulary of document types is defined in Phis ontology.
If an element seems to be missing from the proposed predefined list, please contact Phis managers (see *README.md* for Phis managers contact).

`File`.
This field enables Phis users to upload the new document from their computer through the <span class="btn btn-primary">Browse</span> button.
Only one document at a time can be created, since every document is identified uniquely through an automatically generated URI.
The uploaded file cannot be empty (it has to exceed 0B).
For now, a document cannot exceed 2MB, due to technical problems encountered with **Apache** server.

Once the file has been uploaded, do not click on the <span class="btn btn-primary btn-file">Upload</span> button but <span class="btn btn-success">Create</span> underneath, only when all fields have been completed.
The upload button is bound to be abandonned in the following Phis development.

![upload-file](img/create-document_file.png)

`Comment`. Complete plain text description of the new document, preferably provided in English language.

Click on the <span class="btn btn-success">Create</span> button to complete the document creation, i.e. the document upload and the specification of its metadata with Dublin Core standards.

The list of documents a given user has access to is avaible from the navigation bar through the `Tools > Documents` menu.
From **Home / Documents**, one can click on the eye icon on the right to see a given document information sheet (metadata).
From there, the document cannot be modified or deleted (in Phis current version).
However, the document can be downloaded with the <span class="btn btn-primary">Download</span> button, and its metadata can be modified with the <span class="btn btn-primary">Update</span> button.

![update-document](img/document-update.png)

## Agronomical Objects

### Object types
TODO
plot : link toward AGROVOC: smallest partial unit (one treatment maximum per plot)

block: combination of plots

field : large spatial unit that includes plots and possibly blocks

### Importing Objects
TODO
Plots: geometrical objects such as polygons, provided with Well-known text standard (see [WKT Wikipedia page](https://en.wikipedia.org/wiki/Well-known_text)).

| Alias          | Geometry       | ExperimentURI  | Species     | Variety | ExperimentModalities | Repetition |
| :------------- | :------------- | :------------- | :---------- |:------------- | :------------- | :--------- |
| platformX_experimentY_plotZ       | POLYGON (( ... ... , ... ... ))       | http&#58;//www.phenome-fppn.fr/.../...   | http&#58;//www.phenome-fppn.fr/id/species/...    | e.g. varietyX      | e.g. nitrogen-1     | e.g. 1 (or A-I)     |

![new-objects-browse](img/create-agronomical-objects_browse.png)

![new-objects-find-file](img/create-agronomical-objects_find-file.png)

<!---
![new-objects-create](img/create-agronomical-objects_click-create.png)
--->

![new-objects-success](img/create-agronomical-objects_result.png)

### Visualize objects

In the case of plots...

Alt+Shift

Ctrl+Drag

## Variables

### Variables properties
Phis variables characterize Phis **agronomical objects** or their **environment**.
Variables characterizing agronomical objects are **phenotypic variables**, while variables characterizing the environment in which those agronomical objects are studied are refered to as **environmental variables**.
Phis variables can be either directly mesured by a sensor, either computed from one or several variables.

Every variable produced by an experiment must have been previously created in Phis, and every variable created in Phis has to be defined unambuigusously.
Consequently, when a user refers to a variable in an experiment, there is no ambiguity about the concept he is refering to.
Moreover, the usage of unequivocal variables in experiments is a necessary step towards a more intelligible, reliable and reproducible Science.

Phis variables are listed in the `Variables` menu.
A Phis user with access arestricted access (e.g. *guestphis*) is likely to be unable to see the `Variables` menu, since there is no variable for him/her to see.

Variables are all unequivocally characterized by the following triplet:

- a single **trait**, either a phenotypic trait or an environmental feature, which is the subject of the new variable
- a single **method** of measurement or computation of the trait
- a single **unit** in which is expressed the value of the trait

Further information on a given variable is available on its information sheet, accessed to from the variables list through the eye-icon on the right-hand side of this project row.

![variables-list](img/variables_list.png)

A variable information sheet provides knowledge on this variable, but also on the three elements that define it, namely the **trait**, **method** and **unit** related to this variable.
The variable and those three defining features all display a **label**, that should be meaningful and unique, but does not have to be so, an **URI** which is however unique, a **Definition** (or **Comment**) meant for human comprehension, and **related references** meant for Semantic Web applications.
Reference to external ontologies is achieved through [SKOS](https://www.w3.org/2004/02/skos/intro) standards

*NB: for now, only phenotypic variables are present*

### Create variables, traits, methods and units

Every variable found on Phis has been previously created by a Phis user.
Within the `Variables` menu, one can create a new project with the
<span class="btn btn-success">Create Variable</span> button.

`Variable label`. This field is automatically produced with the concatenation of the trait, method and unit labels, separated by underscores.
The resulting variable label is not necessarily unique, but it would be better if it was.
On the contrary, the automatically generated URI (not shown in the `Create Variable` menu) is unique.

`Trait`. If the trait associated to the new variable has already been created in Phis, one can select it through the predefined list of the **Trait label** field.
Otherwise, it has to be created, which can be achieved by clicking on the <span class="btn btn-success">**+**</span> green icon on the right-hand side of the **Trait label** field.

<!--- <button class="btn btn-success"><span class="glyphicon glyphicon-plus"></span></button> --->

![new-trait](img/create-variable_new-trait.png)

In the case of a new trait, do not fill the `Trait label` field but the `Internal label` one, below the <span class="btn btn-danger">**-**</span> red icon that replaced the <span class="btn btn-success">**+**</span> green icon.
This new trait label should be if possible meaningful, distinct from other trait labels, and underscores "\_" should be avoided since trait, method and unit labels are concatenated to generate the new variable name with the format *Trait_Method_Unit*.

<!---
<button class="btn btn-danger">
<span class="glyphicon glyphicon-minus">
</span>
</button>
--->

A `Comment` should be added, preferably in English, in order to explicit the trait specifics as clearly as possible.

![new-trait-label](img/create-variable_new-trait-label.png)

`Method`. If the method associated to the new variable has already been created in Phis, one can select it through the predefined list of the **Method label** field.
Otherwise, it has to be created, which can be achieved by clicking on the <span class="btn btn-success">**+**</span> green icon on the right-hand side of the **Method label** field.

![new-method](img/create-variable_new-method.png)

In the case of a new method, do not fill the `Method label` field but the `Internal label` one, below the <span class="btn btn-danger">**-**</span> red icon that replaced the <span class="btn btn-success">**+**</span> green icon.
This new method label should be if possible meaningful, distinct from other method labels, and underscores "\_" should be avoided.

A `Comment` should be added, preferably in English, in order to explicit the method specifics as clearly as possible.

`Unit`. If the unit associated to the new variable cannot be found on the `Unit label` predefined list, a new unit has to be created.
This can be achieved by clicking on the <span class="btn btn-success">**+**</span> green icon on the right-hand side of the **Unit label** field.
In the case of a new unit, do not fill the `Unit label` field but the `Internal label` one, below the <span class="btn btn-danger">**-**</span> red icon that replaced the <span class="btn btn-success">**+**</span> green icon.
This new unit label should be if possible meaningful, distinct from other unit labels, and underscores "\_" should be avoided.

Otherwise, if the appropriate unit is already register in Phis, then one only has to select it from the `Unit label` field, without clicking on the <span class="btn btn-success">**+**</span> green icon (or clicking on the <span class="btn btn-danger">**-**</span> red icon if the <span class="btn btn-success">**+**</span> green icon had previously been clicked on).

![existing-trait](img/create-variable_existing-unit.png)

`Related References`.
In order to unambiguously define the new variable, semantic relations are established by the user between the new variable and concepts already defined in reliable ontologies existing on the world wide web.
These relations to external ontologies are established using **SKOS** (Simple Knowledge Organization System).
`Entity` refers to the Phis entity that will be associated to a concept found in an ontology.
This **Entity** be either the new variable, trait, method or unit.
It is not required to specify related concepts for traits, methods and units, however it is recommanded.
`Relation` refers to the nature of the relation between the entity and the concept defined in an ontology.
This semantic relation is provided using SKOS.
The entity can either be, compared to an ontology concept, an **exact match**, a **close match**, **narrower** or **broader**.
These SKOS semantic relations are explicited at this [w3 web page](https://www.w3.org/TR/skos-reference/#semantic-relations).
`Reference URI` refers to the URI of the concept found on ontologies such as the ones suggested in the short list above the **Related References** field.
Do not erroneously provide in this field the URL of the web page of the ontology on which the targeted concept is defined.
Indeed, the URI of a given concept does not necessarily match with the URL of the web page where this concept has been found.
`Hyperlink` (optionnal) refers to the URL where are located the related concept whose URI has been provided in the previous field.

When a variable is created, multiple references using SKOS can be stated, using the <span class="btn btn-default">**+**</span> white icon.

![add-relation-to-a-reference](img/create-variable_add-relation.png)

The main ontologies differ on the following features:

The **AgroPortal** project aims to offer a reference ontology repository for agronomy, reusing the NCBO BioPortal technology.
The scientific outcomes and the experience of the biomdical domain are thus exploited and transposed into the agronomy domain, including plants, food, environment and possibly animal sciences.

**AGROVOC** is a controlled vocabulary covering all areas of interest of the United Nations Food and Agriculture Organization (FAO), including food, nutrition, agriculture, fisheries, forestry, environment, etc.
It is published by the FAO and edited by a community of experts.

The **Plant Ontology** is a sgructured vocabulary and database resource that links plant anatomy, morphology, growth and development to plant genomics data.

The **Planteome** project is a centralized platform where reference ontologies for plants will be used to access plant genomics data.

The **Crop Ontology (CO)** current objective is to compile validated concepts along with their inter-relationships on anatomy, structure and phenotype of crops, on trait mesurement and methods, as well as on germplasm with the multi-crop passport terms.

The **Unit Ontology** gathers metrical units for use in conjunction with **PATO** (Phenotype And Trait Ontology), which is a phenotypic quality ontology.

`Variable Definition`. Text defining clearly the concept underlying the new variable.
This definition should ideally be provided in English.


### Modifiy existing variables
TODO
