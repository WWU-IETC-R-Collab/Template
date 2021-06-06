# Template
The following elements should be included in every repository README in this order:
- Description
  - Brief scope of the code within the repo. This can/should be elaborated in the R markdown instead of the README.
  - Link to repository issues page
  - Link to GitHub page or wiki (if available)
  - Usage
    - Output Data notes and location
    - Other Interpreted result/conclusions/outcomes
    - Requirements for and examples of how to load products
  - Link to related, previous, or next repo
- Spatial metadata
  - Datum (please include information about any transformations or assumptions i.e. source data was WGS84 and we transformed to NAD83 or we assumed some data with was NAD83)
  - Projected coordinate systems, if used (this will only apply to data requiring State Plane projection for spatial analysis)
- Source Information
  - Data Sources
  - Relevant journal citations if needed
- WIP
  - Details about additional enhancements or changes not yet implemented can optionally be included here
- Basic environment requirement information
  - R version used
  - R Packages (WIP)
   
# Example Repository README
This repository contains various templates for common repository items. We should conform to these templates to make finalizing our products easier. This README template can be copied and reused for other repositories. A brief description of your repository should be included at the top. If your repository is complex and contains multiple parts, be sure to include a brief overview describing how the parts are connected.

#### Table of Contents

1. [Issues](#issues)
2. [Usage](#usage)
3. [Methods](#methods-optional)
4. [Spatial Metadata](#spatial-metadata)
5. [Source Information](#source-information)
6. [Required Environment.](#required-environment)

### Issues
For problems or suggestions, please open an [issue](https://github.com/WWU-IETC-R-Collab/Template/issues) or create a [pull request](https://github.com/WWU-IETC-R-Collab/Template/pulls).
### Usage
A description of the output datasets, how they should be used, and any other relevant usage information or caviats could go here.
I'd advise creating a markdown table with linked locations for both the markdown of the code for the output created as well as the GitHub file location for the output (if any).
Lastly, a reproducible example (reprex) for accessing the output should be included (if possible). GitHub markdown supports the insertion of [code blocks](https://guides.github.com/features/mastering-markdown/). Please format your example code to use R syntax so that it can be copied directly from the README. This reprex should include any packages needed to load the output such as our IETC package install/load information.
### Methods (optional)
Sometimes our methods are complicated or exist outside of our regular R environment. I would include a short description here for things such as ArcGIS models or other external modifications.
### Spatial Metadata
If your repository utilizes spatial data and/or analyses, please specifically state the datum here as well as any projection information. I highly recommend providing a link to the projection information on www.spatialreference.org. i.e. The spatial data in this reposity has been transformed from WGS84 datum to NAD83 and is projected in [State Plane California III FIPS 0403](https://www.spatialreference.org/ref/esri/102643/).
### Source Information
Data sources should be listed here with a weblink (if available) or instructions for accessing the data. Preferably a weblink would be included along with an accompanying contact email address for the providing organization. PLEASE also include links to accompanying metadata of the original datasets.
Any relevant journals, papers, or other cited works should be listed here, especially if they accompany a dataset.
### Required Environment
Details about your R environment you used to run code within this repo should be described. At a minimum, you should include an R version here. I'd also recommend including the package versions used for packages required to run the code. Please ensure this information is documented; eventually I hope to transition our work to a containerized R environment that will include a single version of R and a complete set of libraries as it existed at the time we developed this project.

```R
# Example: This will provide your R version from the console
R.Version()$version.string

# There are many ways to find package versions
sessionInfo()
packageVersion("sf")

# You could also try solutions such as: https://github.com/hadley/requirements
```



