# OGC Processing API client Python package

This Python package creates a client for the OGC Processes API to list describe processes, to run and monitor jobs and to retrieve results.

For the automatically generated documentation, including the installation of the package and some code examples, continue reading [here](README-generated.md):

The remainder of this page explains how to setup a test environment and run the test notebooks.

## Requirements

Python 3.8+

## Software installation

### Clone the repository for the test server

```bash
git clone https://github.com/eoap/dev-platform-eoap/
cd dev-platform-eoap
```

Use the `develop` branch

```bash
git checkout develop
```

Part of the following steps are taken from that repository's documentation (see [here](https://eoepca.github.io/document-processing/oa/getting-started/quick-start/) and should be sufficient to set up the test environment. If in doubt, refer to that documentation as well.


### Install software necessary for the test server

Note that this software is needed only for the server the test environment uses. The client independent of it.

**Install *minikube***

Follow the installations instructions from the [official Minikube website](https://minikube.sigs.k8s.io/docs/start/)

**Install *skaffold***

Follow the installations instructions from the [official Skaffold website](https://skaffold.dev/docs/install/)

**Install *helm***

Follow the installations instructions from the [official Helm website](https://helm.sh/docs/intro/install/)


**Add Helm repositories**

```bash
helm repo add zoo-project https://zoo-project.github.io/charts/  
helm repo add localstack https://helm.localstack.cloud 
```

### Create and activate a Python environment

Create a new Python environment to isolate (setting a proper path in the command)

```bash
python3 -m venv /path/to/new/env
```

Activate the environment (using the path where the environment was created):

```bash
. /path/to/new/env/bin/activate
```

Within the environment (usually indicated by a changed shell prompt) and from the root folder of this repository's local working copy, install the necessary Python packages:

```bash
pip3 install pyyaml requests loguru pystac ipykernel ./src
```

## Start the test environment

**Start *minikube***

```bash
minikube start
```

**Start the server using *skaffold***

From the root folder of the local working copy of the **dev-platform-eoap** repository, run the following commands

```bash
cd ogc-api-processes-with-zoo
skaffold dev
```

## Run the test notebooks

This procedure uses Visual Studio Code for running the Jupyter notebooks as this works across the common operating systems.

If necessary, (re-)activate the environment (using the path where the environment was created previously, see above):

```bash
. /path/to/new/env/bin/activate
```

Within the environment (usually indicated by a changed shell prompt) and from the root folder of this repository's local working copy, open Visual Studio Code (this ensures it is availabe for the Python kernel selection):

```bash
code .
```

Inside Visual Studio Code, open the various Jupyter notebooks that are under the [test-notebooks folder](test-notebooks).

For each notebook, select the Python kernel of the environment created above and run the notebooks step by step.
