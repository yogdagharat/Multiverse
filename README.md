# Multiverse

## Introduction

What is Systemic Risk?
Systemic risk refers to the breakdown of the entire financial system due to a domino effect of negative events cascading to a severe economic downturn.
Systemic risk, commonly viewed as a ‘domino effect’ can be defined as the risk associated with the collapse or failure of a company, industry, financial institution, or an entire economy. It is the risk of a major failure of a financial system, whereby a crisis occurs when providers of capital, i.e., depositors, investors, and capital markets, lose trust in the users of capital, i.e., banks, borrowers, leveraged investors, etc. or in a given medium of exchange (US dollar, Japanese yen, gold, etc.). It is inherent in a market system, and hence unavoidable.


### Prerequisites


- [Python](https://www.python.org/downloads/)
- [Git](https://git-scm.com/downloads)
- [Docker](https://docs.docker.com/get-docker/)

### Installing


The steps are:
 1. [Setting up Docker Environment](#step-1---setting-up-docker-environment)
 2. [Cloning the Git Repository](#step-2---cloning-repo)
 3. [Running Docker](#step-3---running-docker)
 4. [Setting up the Jupyter Notebook](#step-4---setting-up-the-jupyter-notebook)
 5. [Running the Analysis](#step-5---running-the-analysis)

### Step 1 - Setting up Docker Environment


- Visit the Docker Page(https://docs.docker.com/get-docker).

- Install the .dmg file (Based on the OS).

- Install Docker as per the installation steps based on the OS.

- Check the installation. 


```
$ docker --version
```

### Step 2 - Cloning the Git Repository

- Clone the source code Git Repository.

```
$ git clone https://github.com/yogdagharat/Multiverse.git 
```

### Step 3 - Running Docker 

- Run the Jupyter Notebook Docker container from Docker Hub.

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

- This will allow you to run commands on the Jupyter Notebook server through your terminal.

- Navigate to the code directory 

```
$ cd work/[DIR]
```

- Run the requirements.txt file.

```
$ pip3 install -r requirements.txt
```

- This will install all libraries required for the source code to run.

- The Jupyter Notebook server is now ready to run the analysis.

### Step 4 - Running the Analysis

- Run all the cells together.

- Cell > Run All

