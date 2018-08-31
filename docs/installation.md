# Installation

## Sensors

### Sensors properties

In order to track where Phis data is coming from, users can declare in the `Sensors` menu the name and attributes of the sensing devices producing experiments' raw data.

The `Sensors` menu displays the list of individual sensors that have been declared by the user on Phis.
The sensor list is preceded by a research bar enabling the user to filter registered sensors by their URI, Alias, type, brand and optionnal attributes, such as the date of their purchase, the date of their first use the date of their last calibration.

![sensor-menu](img/sensor-list.png)

From **Home / Sensors**, one can click on the eye icon on the right of any listed sensor to see its information sheet.

![sensor-information](img/sensor-information.png)

At the top of the sensor sheet lies the <span class="btn btn-warning">Add document</span> button which remains orange until a first document has been added.
Documents linked  to a sensor are typicaly a technical notice or an user manual.
See the [Documents](../experimental-organization/#documents) section below for further information on documents and how to insert them in Phis.
The <span class="btn btn-default">Add annotation</span> button can be used by any user in order to annotate the selected sensor using the [Web Annotation Data Model](https://www.w3.org/TR/annotation-model/) (oa).
See the [Annotation](../experimental-organization/#annotation) section below for further information on annotations within Phis.

### Add sensors

Manually add multiple sensors can be achieved by selecting the <span class="btn btn-success">Create Sensor</span> button at the top-left side of the `Sensors` menu.

The `Add Sensors` menu consists of an editable table in which each additionnal row should contain the information of an additionnal individual sensor to be entrered in Phis database.
The user interface has been built using Handsontable, a JavaScript spreadsheet that allow the user (i) to check quickly the data he is creating and (ii) to copy and paste entire tables into the `Add Sensors` menu.

The mandatory fields, in red, are:

- Alias
- Type
- Brand
- Person In Charge

However, it is highly recommended to fill every field, expect the `Generated URI` field which is automatically produced by Phis after the user clicks on <span class="btn btn-success">Create Sensors</span>.

`Alias`. Internal name of the sensor (free text).

`Type`. Type of the sensor, chosen from a closed list.
Proposed sensor types are mainly greenhouse sensors : don't hesitate to contact OpenSILEX development team to add sensor types that cannot be found in the list in order to make it evolve.
If the dropdown list isn't displayed correctly, try selecting any element of the list : the column width will then expand automatically.

![sensor-type](img/sensor-type.png)

`Brand`. Brand of the sensor (free text).
"homemade" is a valid answer for sensors engineered/modified on site.

`Serial Number`. Free-text used to store the sensor serial number. Optionnal.

`Date of Purchase`. Date of the purchase (or creation for homemade sensors) of the sensor, provided in the YYYY-MM-DD (year-month-day) format. Optionnal.

`In Service Date`. Date provided in the YYYY-MM-DD (year-month-day) format of the first use of the sensor. Optionnal.

`Date of Last Calibration`. Date provided in the YYYY-MM-DD (year-month-day) format of the last calibration of the sensor. Optionnal.

`Person In Charge`. Username (email adress) of the person in charge of the sensing device (typically, the manager of the installation).
If the person in charge is not displayed in the dropdown list, you should first add it to the list of persons through the `Tools > Persons` menu. See the [Create a Person](../community/#create-a-person) section for details.

Not correctly filled fields appear in red.
As long as cells are displayed in red, no sensor can be created.

![add-sensor](img/add-sensor.png)

Note that when you add a single sensor only, you need to remove the second row displayed by default, using the `Remove row` button which appears after a right-click anywhere on the row to delete.
The number of rows has to match the number of added sensors.

![add-sensor-success](img/added-sensor.png)

The `delete sensor` function has not been implemented yet : contact the OpenSILEX development team in order to ask for a sensor to be removed.

### Characterize sensors

Once sensors have been added to the information system, you can characterize them extensively by selecting the <span class="btn btn-success">Characterize Sensors</span> button at the top-left side of the `Sensors` menu.

Not all sensors can be characterized through the `Characterize sensors` menu, but only cameras (all camera types : RGB, multispectral, etc.), spectrometers and LiDAR.

The `Characterize Sensors` button leads to two sequential menus : in the first one you select the sensor (already integrated in the information system) you want to characterize, in the second one you characterize it.

One selects the sensor that need to be characterized providing two pieces of information :

- Type
- URI (will be changed to Alias in a future version of PHIS)

#### Cameras

Camera characteristics common to all cameras are :

`Height (pixels)`.

`Width (pixels)`.

`Pixel Size (µm)`.

The camera types "camera", "hemispherical camera" and "hyperspectral camera" require only those fields to be informed.

In the case of the types "RGB camera" and "TIR camera", additionnal `Lens` fields need to be informed :

`Label`. Internal name of the lens (free text).

`Brand`. Brand of the lens (free text).

`Person In Charge`. Username (email adress) of the person in charge of the sensing device (typically, the manager of the installation).
If the person in charge is not displayed in the dropdown list, you should first add it to the list of persons through the `Tools > Persons` menu. See the [Create a Person](../community/#create-a-person) section for details.

`In Service Date`. Date of the first use of the lens, provided in the format YYYY-MM-DD (year-month-day), directly or through the calendar view.

`Focal length (mm)`.

`Aperture (f-number)`. Ratio of the camera lens' focal length to the diameter of the entrance pupil.

When it comes to multispectral cameras, in addition to the common "height", "width" and "pixel size" fields, one has to provide for each band of spectral discrimination information on :

`Wavelength (nm)`.

`Focal Length (nm)`.

`Attenuator Filter (%)`. Set up by the manufacturer of the camera. Between *0* and *100*. If the camera displays no attenuator filter, then set this value to *100*.

Up to 6 distinct bands of spectral discrimination can be informed in the form, each column matching a specific band and each row a different characteristic.
Not all column have to be filled up (if the camera captures 4 distinct bands, just inform the first 4 columns).

#### Spectrometers

When selecting the sensor type "Spectrometer", the following characteristics need to be filled up :

`Half Field Of View (°)`.

`Minimum Wavelength (nm)`.

`Maximum Wavelength (nm)`.

`Spectral Sampling Interval`.

#### LiDAR

When selecting a LiDAR, the following characteristics need to be filled up :

`Wavelength (nm)`.

`Scanning Angular Range (°)`.

`Scanning Angular Range (°)`.

`Scanning Angular Resolution (°)`.

`Spot width (°)`.

`Spot height (°)`.

## Vectors

### Vectors properties

Sensors used for plant phenotyping can be carried on vectors such as UAVs or field robots.

The `Vectors` menu displays the list of vectors that have been declared by the user on Phis.
The vector list is preceded by a research bar enabling the user to filter registered vectors by their Alias, type, brand and optionnal attributes, such as the date of their purchase, the date of their first use or their serial number.

![vector-menu](img/vector-list.png)

From **Home / Vectors**, one can click on the eye icon on the right of any listed vector to see its information sheet.

<!---
![vector-information](img/vector-information.png)
--->

At the top of the vector information sheet lies the <span class="btn btn-warning">Add document</span> button which remains orange until a first document has been added.
Documents linked  to a vector are typicaly a technical notice, an user manual or a brochure.
See the [Documents](../experimental-organization/#documents) section for further information on documents and how to insert them in Phis.
The <span class="btn btn-default">Add annotation</span> button can be used by any user in order to annotate the selected vector using the [Web Annotation Data Model](https://www.w3.org/TR/annotation-model/) (oa).
See the [Annotation](../experimental-organization/#annotation) section below for further information on annotations within Phis.

### Add vectors

Manually add multiple vectors can be achieved by selecting the <span class="btn btn-success">Create Vector</span> button at the top-left side of the `Vectors` menu.

The `Add Vectors` menu consists of an editable table in which each additionnal row should contain the information of an additionnal vectors to be inserted in Phis database.
The user interface has been built using Handsontable, a JavaScript spreadsheet that allow the user (i) to check quickly the data he is creating and (ii) to copy and paste entire tables into the `Add Vectors` menu.

The mandatory fields, in red, are:

- Alias
- Type
- Brand
- In Service Date
- Person In Charge

However, it is highly recommended to fill every field, expect the `Generated URI` field which is automatically produced by Phis after the user clicks on <span class="btn btn-success">Create Vectors</span>.

`Alias`. Internal name of the vector (free text).

`Type`. Type of the vector, chosen from a closed list.
There is onmly a handful of proposed vector types : don't hesitate to contact OpenSILEX development team to add vector types that cannot be found in the list in order to make it evolve.
If the dropdown list isn't displayed correctly, try selecting any element of the list : the column width will then expand automatically.

![vector-type](img/vector-type.png)

`Brand`. Brand of the vector (free text).
"homemade" is a valid answer for vectors engineered/modified on site.

`Serial Number`. Free-text used to store the vector serial number. Optionnal.

`Date of Purchase`. Date of the purchase (or creation for homemade vectors) of the vector, provided in the YYYY-MM-DD (year-month-day) format. Optionnal.

`In Service Date`. Date provided in the YYYY-MM-DD (year-month-day) format of the first use of the vector.

`Person In Charge`. Username (email adress) of the person in charge of the vector (typically, the manager of the installation).
If the person in charge is not displayed in the dropdown list, you should fisrt add it to the list of persons through the `Tools > Persons` menu. See the [Create a Person](../community/#create-a-person) section for details.

![add-vector](img/add-vector-red.png)

Not correctly filled fields appear in red.
As long as cells are displayed in red, no vector can be created.
Note that when you add a single vector only, you need to remove the second row displayed by default, using the `Remove row` button which appears after a right-click anywhere on the row to delete.
The number of rows has to match the number of added vectors.

![add-vector](img/add-vector.png)

Complete the vector insertion in Phis clicking on the <span class="btn btn-success">Create Vectors</span> button.

![add-vector-success](img/added-vector.png)

Once created, the vector specifics can be modified with the <span class="btn btn-primary">Update</span> button located on top of any vector information sheet.

The `delete vector` function has not been implemented yet : contact the OpenSILEX development team in order to ask for a vector to be removed.
