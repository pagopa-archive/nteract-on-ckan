# nteract-on-ckan

### INFO

nteract-on-ckan is a [customized](https://github.com/teamdigitale/daf-nteract) fork of [nteract](https://nteract.io/) that
queries [ckan](https://ckan.org/) api throught an [api server](https://github.com/teamdigitale/pdnd-openapi-server) that exposes openapi 3 specifications. It enables to search and load directly from [data.gov](https://data.gov) in your notebook, but can be connected easily with every ckan you want.

This repo contains the instructions for launching a working environment via docker compose and contains a set of notebooks and tutorials.

- [Tutorial](notebooks-example/tutorial.ipynb)
- [Analyses](notebooks-example/) for example about [mortality by cancer in Italian regions](notebooks-example/italy_mortality.ipynb) or [European election](notebooks-example/eu_elections_2019_italy.ipynb)

If you are a data scientist try to contribute by using the tools and share your work on this repository by making a PR.

### Open on binder

- List of examples and analyses on [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/teamdigitale/nteract-on-ckan-on-ckan/master?urlpath=%2Fnteract%2Fedit)

### Technological stack

The stack is composed of:

- [daf-nteract](https://github.com/teamdigitale/daf-nteract) is a customisation of [nteract](https://nteract.io/).
- [An api server](https://github.com/teamdigitale/pdnd-openapi-server)
- [Ckan](https://data.gov/), as metadata store for dataset.

With nteract-on-ckan you can:

- search datasets stored on ckan
  through the api
- automatically load data by running an autogerated snippet of code with many programming languages
- creating chart semi-automatically.

Can be used to have the first
approach on notebooks, open data and visualizations.

### Old material it refers on daf / pdnd but the concepts are the same.

- [Medium post](https://blog.nteract.io/creating-a-platform-for-querying-open-datasets-with-pdnd-nteract-6ac8107828f7)
- [Video tutorial](https://www.youtube.com/watch?v=nlZnYcz66YE)

### GETTING STARTED

[Docker](https://www.docker.com/) MUST be installed on your local machine

```
git clone git@github.com:teamdigitale/nteract-on-ckan.git
cd nteract-on-ckan
docker-compose up
```

It can take some time to download from dockerhub.

Save the token from the output of your console as:
http://(b4fd9e3ef290 or 127.0.0.1):8888/?token=XXXXXXXXXXXXXX
and open your browser at [http://localhost:8888]. If you are asked the token paste it.

You should see something like this:
![start](https://raw.githubusercontent.com/teamdigitale/nterat-on-ckan/master/img/nterat-on-ckan-home.png)

CONGRATULATIONS NOW YOU ARE READY TO CONTRIBUTE.

### HOW TO CONTRIBUTE

Never made an open source contribution before?

1.  Fork this repository to your local GitHub organization.

2.  Clone the repository to your local machine using:

```
$ git clone https://github.com/github-username/repository-name.git
```

3. Set the upstream repository by

```
$ git remote add upstream git@github.com:teamdigitale/nterat-on-ckan.git
```

4.  Install the image and launch as in the steps described [above](https://github.com/teamdigitale/nterat-on-ckan)

5.  Create a new branch for your new analyses using:

```
$ git checkout -b branch-name-here
```

6.  Create a new analysis on some public data provided by the platform

7.  Add and commit the changed files using `git add` and `git commit`.

8.  Push the changes to the remote repository using:

```
$ git push origin branch-name-here
```

9. Submit a pull request to the upstream repository.

10. Title the pull request per the requirements outlined in the section below.

11. Set the description of the pull request with a brief description of what you did and any questions you might have about what you did.

12. Wait for the pull request to be reviewed by a maintainer.

13. Make changes to the pull request if the reviewing maintainer recommends them.

14. Celebrate your success after your pull request is merged! :tada:
