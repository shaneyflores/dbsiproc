# dbsiproc
Pipeline for extracting DBSI values for FreeSurfer ROIs. 

## Pre-requities
Before a user can launch this pipeline, [FSL](https://fsl.fmrib.ox.ac.uk/fsl/fslwiki/FslInstallation) must be installed with the fsl.sh setup script sourced. 

Additionally, a local install of [FreeSurfer](https://surfer.nmr.mgh.harvard.edu/fswiki/DownloadAndInstall) and [AFNI](https://afni.nimh.nih.gov/pub/dist/doc/htmldoc/background_install/install_instructs/index.html) are also needed.

## Usage
```bash
dbsiproc session.params
```
session.params is a user-generated parameters file that declares some of the variables needed by the pipeline. An example params file can be found in test.params in the repository.

## Data Structure
The pipeline assumes that the parent folder (e.g., a MR session folder) will contain a subfolder that stores all the DBSI NIFTI files (this folder is typically called 'diffusion'). The parent folder should also contain the FreeSurfer output, in its entirety. 
