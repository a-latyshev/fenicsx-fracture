# FEniCSx Fracture mechanics examples

This repository automatically generates a jupyter-book here: PUT THE LINK HERE

## Installation

### Conda
To create the conda environement and activate it

```bash
conda env create -f fenicsx-fracture.yml
conda activate fenicsx-fracture
```
To generate the book the book locally:
```bash
jupyter-book build notebooks
```
To visualize the results, open in your browser the generated file `_build/html/index.html`.

### Docker
To build a docker image for this documentation, you can run

```
docker build -t fenicsx-fracture -f docker/Dockerfile docker/
```
from the root of this repository. To create a one-time usage container you can call:

```
docker run -ti -v $(pwd):/root/shared -w /root/shared --rm fenicsx-fracture
````

## Binder
Although we recommend to execute the notebook locally, you can also use the cloud-based binder service to execute the notebooks:

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/newfrac%2Fnewfrac-fenicsx-training/HEAD)

## Acknowledgements

The funding received from the European Union’s Horizon 2020 research and
innovation programme under Marie Skłodowska-Curie grant agreement No.
861061-NEWFRAC is gratefully acknowledged.

## License

MIT License, see `LICENSE` file.
