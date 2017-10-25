# The megSAP pipeline as a Singularity container
[![DOI](https://zenodo.org/badge/107653419.svg)](https://zenodo.org/badge/latestdoi/107653419)

A singularity container for the [megSAP pipeline](http://github.com/imgag/megSAP/)to be used in our reporting in the future. We use specific tags for releasing updated containers, so stay tuned :-) 

## Creating the container

To create the container from scratch, run for example:

```bash
git clone https://github.com/qbicsoftware/qbic-singularity-megSAP.git
cd qbic-singularity-megSAP
sudo singularity build qbic-singularity-megSAP.simg Singularity.megSAP
```

## Running the containers applications

```bash
singularity exec qbic-singularity-megSAP.simg php /megSAP/src/Pipelines/analyze.php --help
```
Check out our nextflow workflow scripts to see how we utilize the container directly on our infrastructure. 

If you have further questions, ask here via GitHub or alexander.peltzer@qbic.uni-tuebingen.de
