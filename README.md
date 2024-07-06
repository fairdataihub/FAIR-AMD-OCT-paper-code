[![Contributors][contributors-shield]][contributors-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.12662728.svg)](https://doi.org/10.5281/zenodo.12662728)

[contributors-shield]: https://img.shields.io/github/contributors/fairdataihub/FAIR-AMD-OCT-paper-code.svg?style=flat-square
[contributors-url]: https://github.com/fairdataihub/FAIR-AMD-OCT-paper-code/graphs/contributors
[stars-shield]: https://img.shields.io/github/stars/fairdataihub/FAIR-AMD-OCT-paper-code.svg?style=flat-square
[stars-url]: https://github.com/fairdataihub/FAIR-AMD-OCT-paper-code/stargazers
[issues-shield]: https://img.shields.io/github/issues/fairdataihub/FAIR-AMD-OCT-paper-code.svg?style=flat-square
[issues-url]: https://github.com/fairdataihub/FAIR-AMD-OCT-paper-code/issues
[license-shield]: https://img.shields.io/github/license/fairdataihub/FAIR-AMD-OCT-paper-code.svg?style=flat-square
[license-url]: https://github.com/fairdataihub/FAIR-AMD-OCT-paper-code/blob/master/LICENSE

# Code: FAIR AMD OCT Datasets Paper

## About
This is the code associated with the paper titled "Publicly Available Imaging Datasets for Age-related Macular Degeneration: Evaluation according to the Findable, Accessible, Interoperable, Reproducible (FAIR) Principles". Age-related macular degeneration (AMD), a leading cause of vision loss among older adults, affects more than 200 million people worldwide. In this paper, We evaluated openly available AMD-related datasets containing optical coherence tomography (OCT) data against the FAIR principles. This repository contains the Jupyter notebook developed to analyze data for the paper and generate figures. See this [inventory](https://github.com/fairdataihub/FAIR-AMD-OCT-paper-inventory) for all related resources, including the paper.


## Standards followed
The overall code is structured according to the [FAIR-BioRS guidelines](https://fair-biors.org/). The Python code in the Jupyter notebook [main.ipynb](main.ipynb) follows the [PEP8 guidelines](https://peps.python.org/pep-0008). Functions are documented with docstring formatted following [Google's style guide](https://google.github.io/styleguide/pyguide.html#38-comments-and-docstrings). All the dependencies are documented in the [environment.yml](environment.yml) file.

## Using the Jupyter notebook

### Prerequisites 
We recommend using Anaconda to create and manage your development environment and using JupyterLab to run the notebook. All the subsequent instructions are provided assuming you are using [Anaconda (Python 3 version)](https://www.anaconda.com/products/individual) and JupyterLab.

### Clone repo
Clone the repo or download as a zip and extract.

### cd into the code folder

Open Anaconda prompt (Windows) or the system Command line interface then naviguate to the code
```sh
cd .FAIR-AMD-OCT-paper-code

```

### Setup conda env
```sh
$ conda env create -f environment.yml
```

### Setup kernell for Jupyter lab
```sh
$ conda activate FAIR-AMD-OCT-paper-code
$ conda install ipykernel
$ ipython kernel install --user --name=<any_name_for_kernel>
$ conda deactivate
```
### Launch Jupyter lab
Launch Jupyter lab and naviguate to open the main.ipynb file. Make sure to change the kernel to the one created above (e.g., see [here](https://doc.cocalc.com/howto/jupyter-kernel-selection.html#cocalc-s-jupyter-notebook)). We recommend to use the [JupyterLab code formatter](https://github.com/ryantam626/jupyterlab_code_formatter) along with the [Black](https://github.com/psf/black) and [isort](https://github.com/PyCQA/isort) formatters to facilitate compliance with PEP8 if you are editing the notebook.

## Inputs/outputs
The Jupyter notebook makes use of files in the dataset associated with the paper [(see here)](https://github.com/fairdataihub/FAIR-AMD-OCT-paper-inventory). You will need to download the dataset at add it in the input folder (call the dataset folder 'dataset').

Outputs of the code include plots displayed in the notebook but also saved as files. These saved plot files are included in the [output](output) folder. 

## License
This work is licensed under
[MIT](https://opensource.org/licenses/mit). See [LICENSE](LICENSE) for more information.

## Feedback and contribution
Use the [GitHub issues](https://github.com/fairdataihub/FAIR-AMD-OCT-paper-code/issues) for submitting feedback or making suggestions. You can also work the repository and submit a pull request with suggestions.

## How to cite
If you use this code, please cite the related paper (it will be listed [here](https://github.com/fairdataihub/FAIR-AMD-OCT-paper-inventory) when available) and also cite this repository as:

```bash
Gim, Nayoon, Patel, Bhavesh. Code: FAIR AMD OCT Datasets Paper [Software]. Zenodo. https://doi.org/10.5281/zenodo.12662728
```
