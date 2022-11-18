# DATC Cloud Native Enablement of Large-Scale DoE

## Introduction

Machine learning requires data, hence ML EDA also requires data. 
However, in the EDA and IC design context, generating large amounts of data typically requires enormous compute resources and takes significant time. 
To enable efficient generation of the large volume of data needed to support ML EDA, our efforts focus on bringing attention to use of cloud computing resources which are now prevalent and easily accessible from commercial providers. 
Cloud-native enablement will help enable scalable CAD/EDA optimizations that leverage massive data and parallelism.

An important question is how to _best utilize_ a public cloud to generate large-scale data for ML EDA. 
Merely obtaining bare cloud instances, installing libraries and compiling tools every time does not scale well and is not easily portable to alternate cloud/compute environments. 

This section provides Jupyter notebooks that demonstrate cloud-native way of enabling large-scale designs of experiments for ML-enabled EDA using public cloud services.


## Prerequisites (common across the demos)

* Docker Desktop: [installation instruction](https://docs.docker.com/desktop/windows/install/)
* Python 3.9.6, with Ray, matplotlib, and webp
    - Refer to a reference conda environment [./environment.yaml](./environment.yaml).
    - Example to create the fresh conda environment on your own:

        ```bash
        conda create -n rdf-ray python=3.9.6
        conda activate
        conda install -c conda-forge jupyterlab
        pip install ray matplotlib webp
        ```

## Notebooks

- DATC RDF demo: [Link](./datc-rdf-demo)
- Single-node Kubernetes demo: [Link](./k8s-single-node-demo)
- Sngle-node Kubernetes/Ray demo: [Link](./k8s-single-node-ray-demo)
- Multi-node Kubernetes/Ray demo: [Link](./k8s-multi-node-ray-demo)



## Contact

Jinwook Jung (jinwookjung@ibm.com)
