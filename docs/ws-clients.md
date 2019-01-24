# Web Service Clients

## Python Clients

### Images import Python client

An up-to-date version of said client can be found on GitHub at the following URL: [https://github.com/OpenSILEX/phis-ws-clients/blob/master/python/images/post.py](https://github.com/OpenSILEX/phis-ws-clients/blob/master/python/images/post.py).

Download this `post.py` script and change with the help of a text editor (e.g. Notepad++ if you are using Windows) its rows n° 17, 27, 28 and 58.

#### Modification of the Python script
Having installed [Python](https://www.python.org/) is required to run the `post.py` script.
Here is the list of changes you need to make to this script in order to import your images to PHIS:

**Row n° 17**:

Replace the default host name `'http://localhost:8084/phis2ws/rest/'` by the host name associated to your occurence of PHIS.
The URL of your documentation link should be of the form `'http://[...]/[occurence name]/api-docs/'`. The host name you need to provide on row 17 of `post.py` is this URL but with "api-docs" replaced by "rest": `'http://[...]/[occurence name]/rest/'`.
Do not forget the single brackets.

**Row n° 27 & 28**:

Rows 27 and 28 are used for indicating your own login, the one you use when connecting to PHIS via a web browser.

On row 27, replace the second occurence of 'username' by your username between single brackets: it should be an email adress, e.g. `'username': 'example@supagro.inra.fr',`.

On row 28, the simplest thing to do is to replace the second occurence of 'password' by your password between single brackets, e.g. ` 'password': hashlib.md5('type your password here').hexdigest(),`.

However, if you do not wish to right your password in clear, replace `hashlib.md5('password').hexdigest()` by an encrypted version of your password: a md5 checksum of your password (also between single brackets), e.g. `'1a79a4d60de6718e8e5b326e338ae533'` (this is the md5 encryption of "example").
Creating a md5 checksum version of your password can be achieved either using the official [md5 webpage](https://www.md5.fr/) and typing there your password, either from a linux terminal typing `echo example | md5sum`, replacing "example" by your actual password.

**Row n° 58**:

Replace `"POSTImages-template.csv"` by the name of the CSV file containing the information on the images you would like to import to PHIS.
Do not forget the double brackets.
If you execute the Python script from a different repository than the one where the CSV file is stored, then in addition to the CSV file name, you need to inform the path to the CSV file, e.g. `"path/to/POSTImages-template.csv"`.

A template of the required CSV file can be found on GitHub at the following URL: [https://github.com/OpenSILEX/phis-ws-clients/blob/master/python/images/POSTImages-template.csv](https://github.com/OpenSILEX/phis-ws-clients/blob/master/python/images/POSTImages-template.csv).

#### Modification of the CSV

The first row of the CSV file displays its header:

| path_image_ref     | imageType     | concernedUri     | concernedType     | position    | date     |  sensorUri   |
| :------------- | :------------- | :------------- | :------------- | :------------- | :------------- | :------------- |

Then, each row of this CSV file is associated to an image imported in PHIS.
Each image is characterized by:

- **path_Image_ref**: the name and path of the image (e.g. `image001.png`)
- **ImageType**: the URI associated with the type of the image (e.g. `http://www.phenome-fppn.fr/vocabulary/2017#HemisphericalImage` or `http://www.phenome-fppn.fr/vocabulary/2017#RGBImage`)
- **concernedUri**: the URI of the entity associated to the image, typically an agronomical object such a plot (e.g. `http://www.phenome-fppn.fr/mtp/2017/o1000001`)
- **concernedType**: the URI associated with the type of the entity associated with the image (e.g. `http://www.phenome-fppn.fr/vocabulary/2017#Plot`)
- **position** (optionnal): if a sensor can display several positions, then you might want to fill the position from which the image has been shot (e.g. `1`)
- **date**: date at which the image has been shot, using the *YYYY-MM-DD HH:MM:SS* format (e.g. `2017-06-15 09:00:00`)
- **sensorUri**: URI of the sensor who captured the image (the URI of the sensors you registered in PHIS are available on the [Sensors menu](../phis-docs-community/experimental-organization/#sensor))

All of these information are filled in plain text and without brackets.

Both image types and entity types have to be submitted using the controlled vocabulary linked to PHIS application ontology.
The list of images types can be found in the `Tools / Vocabulary` menu of PHIS webapp.

#### Execution of the Python script
Like any other Python script, e.g. using ipython or a linux terminal:

```
python post.py
```
