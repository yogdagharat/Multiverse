# Systemic Crisis Analysis

## Introduction

What is **Systemic Crisis**? 

Economists call systemic risk and systemic crisis extremely danger destructive troubles that menace (risk) or affect (crisis) the whole global sous financial and monetary system.

Such cataclysmic avalanches can entail
- A meltdown of most financial instruments and institutions,
- With dire negative effects on the whole economic system (trade, production, spending, employment)

A systemic financial or monetary crisis would result from a "domino effect" in which the collapse of an important financial institution (bank, investment or pension fund, insurance company) spread to all the worldwide financial and monetary system.

The datasets **Main.xlsx** and **OECD_Euro.xlsx** used for this analysis is taken from the analysis done by Carmen Reinhart (with her coauthors Ken Rogoff, Christoph Trebesch, and Vincent Reinhart) and the OECD Public Finance Dataset respectively.

The focus of this study is to understand the interconnectedness of systemic crisis to macroeconomic factors and how these influences may lead to financial crisis.

### Prerequisites

- [Python](https://www.python.org/downloads/)
- [Git](https://git-scm.com/downloads)
- [Docker](https://docs.docker.com/get-docker/)

### Installation

The steps are:
 1. [Setting up Docker Environment](#step-1---setting-up-docker-environment)
 2. [Cloning the Git Repository](#step-2---cloning-the-git-repository)
 3. [Running Docker](#step-3---running-docker)
 4. [Setting up the Jupyter Notebook](#step-4---setting-up-the-jupyter-notebook)
 5. [Running the Analysis](#step-5---running-the-analysis)

### Step 1 - Setting up Docker Environment


- Visit the Docker Page(https://docs.docker.com/get-docker).

- Install the .dmg file (Based on the OS).

- Install Docker as per the installation steps (Based on the OS).

- Check the installation and the version. 

```
$ docker --version
```

### Step 2 - Cloning the Git Repository

- Clone the source code Git Repository.

```
$ git clone https://github.com/yogdagharat/Multiverse.git 
```

### Step 3 - Running Docker 

- Run the Jupyter Notebook Docker container from the Docker Hub.

```
$ docker run -p 8888:8888 jupyter/minimal-notebook
```

- Once you run the command, select the given URL of the format:
http://127.0.0.1:8888/?token=[TOKEN].

- Start the Jupyter Notebook server using the URL.

### Step 4 - Setting up the Jupyter Notebook

- Upload the source codes cloned from the Git repository to Jupyter Notebook.

- Install all the dependencies.

```
$ docker ps
```

- Copy the container ID on which the Jupyter Notebook server is running.

- Run the Docker exec commands on another terminal the Jupyter Notebook server.

```
$ docker exec -it <container-id> /bin/bash
```

- This step will allow you to run commands on the Jupyter Notebook server through your terminal.

- Navigate to the code directory.

```
$ cd work/[DIR]
```

- Run the requirements.txt file.

```
$ pip3 install -r requirements.txt
```

- This command will install all libraries required for the source code to run.

- The Jupyter Notebook server is now ready to run the analysis.

### Step 4 - Running the Analysis

- Run all the cells together.

- Cell > Run All

