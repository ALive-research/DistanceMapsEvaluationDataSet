This is a dataset which combines the following datasets

    - Task03_Liver
    - Task08_HepaticVessels
    
originally found in http://medicaldecathlon.com/

In this dataset, the different labels have been separated (e.g, liver, tumor,
vessels) and unified in a single dataset in `.nrrd` format, instead of the
original `.nii.gz`.

The repository contains hash files (`.nrrd.sha`) which contain the SHA256 hash of the
file. In order to download the file you can use the url
https://github.com/ALive-research/ALiveResearchTestingData/releases/download/SHA256/%(hash),
replacing `%(hash)` by the actual hash of the file. This organization allows a
separation between metadata and the actual data (which couldn't be uploaded to a
repository). This scheme is particularly fit for its use with the `ExternalData`
module of CMake (https://cmake.org/cmake/help/latest/module/ExternalData.html).
    
