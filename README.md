Welcome! This is a template repository for submitting models to Model Atlas of The Earth (**M@TE**). 
<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
[![All Contributors](https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)](#contributors-)
<!-- ALL-CONTRIBUTORS-BADGE:END -->

How model submission works...
-----

<details><summary>CLICK TO EXPAND</summary>
<p>


* create a new repository by clicking on the __Use this template__ button above
* name your repository using this convention:
   * `creatorname_year_keyword` (e.g. `corcho_2022_collision`)
* populate this markdown document (`Readme.md`) with as much information as you can
* information is recorded in 3 recurring structures:
    * **Metadata Fields** (markdown tables)
    * **Metadata Tags** (markdown checkboxes)
    * **File Description** (markdown tables)
* you need to physically edit the markdown (plain text). You can do this directly through github, or on your device with a plain text editor.
    * Many of the fields have place holder / example text to help guide you. Delete this text and replace with your own.   
* add any files to the `model_files` and `web_files` subfolders.
* once you have completed these steps, you can submit your model back to M@TE <https://github.com/ModelAtlasofTheEarth>

> **Note**
> The Wiki provides more detailed information on submission. Create a Github Issue if you have problems or questions. 

  
</p>
</details>

About your model
-----

<details><summary>CLICK TO EXPAND</summary>
<p>

**Metadata fields**

Field | Value | Notes
--- | --- | ---
**Title** | E.g., _my new expanding earth model_ | E.g. additional notes, including problems/questions arising
**Abstract** | _An abstract for your model (preferrably plain language)_ | 
**Keywords** | _keyword 1_ (add rows as needed) | 
**Field of research (FOR) code** | E.g., 3706 ( see <https://vocabs.ardc.edu.au/viewById/316>)  (add rows as needed) |


**Metadata  Tags**

> **Note**
> Place an X in in the boxes to select!

- [ ] published study
- [ ] commmunity benchmark
- [ ] attempted reproduction of a previous model (including with different codes, etc)
- [ ] missing data model (input files available, requires re-running by community)


</p>
</details>


Model computation and reproduction
-----

<details><summary>CLICK TO EXPAND</summary>
<p>

**Metadata fields**


The following fields provide information and references for sources and processes that were used to create the dataset.  Provide software and computing details, versioning, web references, DOIs, Github links, input datasets etc. on any of the components and workflows that went into the generation of the dataset. 


Field | Value | Notes
--- | --- | ---
**software framework** | | 
**software version** | E.g. Models run with UWGeodynamics version 2.15, compatible with versions 2.12-2.15  |
**source code link** |  | 
**input datasets** |  | 
**computer details** | E.g., cluster name, Operating System, MPI version, number of cores  | 
**additional notes** | E.g., This product was generated by XX method as described by XX et al. (yyyy) <paper doi>. Further details and code for the method are available in the Github/code repository XX....This product is derived from dataset XX (dataset doi or link to details). The method is detailed in .... and uses inputs X (link), Y (link), Z (link) to produce this published product. |



**Metadata  Tags**

- [ ] this submission includes input files
- [ ] this submission includes a software container or environent file for __running the model__ (i.e. docker image, dockerfile, conda environment.yml)
- [ ] this submission includes postprocessing files
- [ ] this submission includes a software container or environent file __for postprocessing__
- [ ] postprocessing files are linked to data on the NCI's GeoNetwork (through thredds/OPeNDAP API)


> **Note**
> Please add any additional files (related to model execution, reproduction and postprocessing) to the `model_files` folder. Describe these files in the **File Description** table below.

**File Description**

Filename/pattern | Description | Notes
--- | --- | ---
E.g., `model_files/input.py` (add rows as needed) |  E.g., description of `model_files/input.py`  | 
E.g., `model_files/Dockerfile` (add rows as needed) | E.g., description of `model_files/Dockerfile`  | E.g., link to existing image on Dockerhub
E.g., `log.txt` | E.g., Logfile from original model execution on NCI Gadi  | 




</p>
</details>


Model output data
-----

<details><summary>CLICK TO EXPAND</summary>
<p>


**Metadata  Tags**

- [ ] this submission  includes model output data

> **Note**
> If the above box is ticked, the M@TE team will contact you with details for uploading data. Please fill out the **Metadata fields** Tables below.  Please describe output data files using the **File Description** Table. 
  
**Metadata fields**



Field | Value | Notes
--- | --- | ---
**Summary of dataset** | Pitch for the general user and not just the content expert. Helpful things would include: summary of the dataset, high-level description of the dataset contents, and why this dataset might be useful to experts and non-experts. | ---

**Temporal extents (if applicable)** | e.g., Begin time (YYYY/MM/DD, or 50 Myr)  End time (YYYY/MM/DD, or 20 Myr) | ---
**Spatial extents (if applicable)** | e.g.,  west bounding longitude (degrees), east bounding longitude (degrees), ...| ---
**Local NCI file path** | Completed once data are available on NCI Geonetwork Catalog | 
**DOI (NCI Internal Field)** | Completed once data are available on NCI Geonetwork Catalog | 
**additional notes** | E.g., output data ar saved at time/step increments of (100 Kyr) | 


> **Note**
> Model output data is _Not_ submitted through Github. However the **File Description** Table provides a place to describe those files. Include anything that might be useful for the community (or your future self): datum or reference values, units, nature of the data (scalar/vector/tensor), order of components. 

**File Description**

Filename/pattern | Description | Notes
--- | --- | ---
E.g. `velocity_**.h5`, | E.g. velocity field on mesh nodes, units cm/y, first component is horizontal, second component is vertical (positive up), files saved at 1 Ma intervals  | 
`topography.csv`  | E.g. topography relative to initial (undeformed) upper boundary of model, units m  | 


</p>
</details>


Website material
-----

<details><summary>CLICK TO EXPAND</summary>
<p>


> **Note**
> To feature your model on our website (<https://mate.science>), we will require some images/animations and captions. Please add files to the `web_files` folder, and describe these files using the following **File Description** Table. The **Purpose** field will be used to help direct the content. You do not need to supply all of these, and you may supply multiple files with the same purpose.

**File Description**

File | Purpose | Caption
--- | --- | ---
`image1.png` | landing page image | Caption for `image1.png`, Lorem ipsum dolor sit ame
`filex.png` | visual abstract |  Caption for `filex.jpg`
`figx.jpeg` | model setup | Caption of `figx.jpeg``
`model_animation.avi` | animation | Caption for of `model_animation.avi`


> **Note**
> Acceptible formats: JPEG, PNG, PDF, AVI, GIF, MP4. Total size of files will be limited by Github repository constraints




</p>
</details>



Attribution
-----
<details><summary>CLICK TO EXPAND</summary>
<p>


Field | Value | Notes
--- | --- | ---
**Associated publication DOI** | DOI | 
**Funder(s)** |  Please add rows as required if more than 1 funder. | 
**Author(s)** | Either use "refer to publication", or Author 1 (Last name, first name, organisation name, email address, ORCID ID)| 
**Licence** |  E.g., <a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>. | 

> **Note on Publications**
> Please also add .bib entries for any associated publication to the `CITATIONS.bib` file
> See Wiki for further information on .bib files 

> **Note on Licence**
> we encourage model creators to issue a single licence that will cover all material sumbitted to M@TE.
> we recommend a Creative Commons license
> you can use the following website to choose from a range of options <Chttps://creativecommons.org/choose/> 




</p>
</details>


## Contributors

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tbody>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/dansand"><img src="https://avatars.githubusercontent.com/u/10967872?v=4?s=100" width="100px;" alt="Dan Sandiford"/><br /><sub><b>Dan Sandiford</b></sub></a><br /><a href="#content-dansand" title="Content">🖋</a></td>
    </tr>
  </tbody>
</table>

<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->

<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->

[![All Contributors](https://img.shields.io/github/all-contributors/ModelAtlasofTheEarth/model_template?color=ee8449&style=flat-square)](#contributors)




