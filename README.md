
# pdnd-open-notebooks

  

### INFO

  

This repo contains a set of notebooks devoloped using [pdnd-nteract](https://github.com/teamdigitale/daf-nteract) on top of a [datascience docker image](https://github.com/jupyter/docker-stacks/tree/master/datascience-notebook) provided by [jupyter project](https://jupyter.org/). The image contains a ready to use datascience environment with the most used datascience libraries for **python3**, **R**, and **Julia**. If you want to deepen about the set of libraries you can read [this](https://jupyter-docker-stacks.readthedocs.io/en/latest/). 

[Pdnd-nteract](https://github.com/teamdigitale/daf-nteract) is a customisation of [nteract](https://nteract.io/) that allows users registered into the [pdnd](https://dataportal.daf.teamdigitale.it/) to search and load datasets into the notebook from about 7000 italians public datasets. If you want to know more about the project you can start from [here](https://github.com/teamdigitale/daf-nteract).  Some material to understand how it works can be:

 - TODO Medium post still draft
 - [Video tutorial]([https://www.youtube.com/watch?v=nlZnYcz66YE](https://www.youtube.com/watch?v=nlZnYcz66YE))
 - [Tutorial](open-notebooks-example/tutorial.ipynb) in this repo
 - [Examples](open-notebooks-example/) in this repo

### GETTING STARTED

[Docker]([https://www.docker.com/](https://www.docker.com/)) MUST be installed on your local machine

TODO change image with the datascience one
From [dockerhub](https://hub.docker.com/r/teamdigitale/daf-nteract)

```
git clone THIS_REPO
cd pdnd-open-notebooks
docker pull teamdigitale/daf-nteract
docker run -p 8888:8888 -v "$PWD":/home/jovyan/work daf-nteract
```
Save the token from the output of your console as:
http://(b4fd9e3ef290 or 127.0.0.1):8888/?token=XXXXXXXXXXXXXX
and open your browser at [http://localhost:8888]. If you are asked the token paste it.

You should see something like this:
![start](https://raw.githubusercontent.com/teamdigitale/pdnd-open-notebooks/img/start.png)
