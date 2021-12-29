# Data analysis
- Document here the project: Fuzi_project
- Description: the idea is to use restaurant billing history, wheather and several other factors to predict how many customer a restaurant will have. 
- Data Source: API wheather + history of friends restaurants.
- Type of analysis: I tried for now basic regression and Facebook Prophet.


# Startup the project

The initial setup.

Create virtualenv and install the project:
```bash
sudo apt-get install virtualenv python-pip python-dev
deactivate; virtualenv ~/venv ; source ~/venv/bin/activate ;\
    pip install pip -U; pip install -r requirements.txt
```

Unittest test:
```bash
make clean install test
```

Check for Fuzi_project in gitlab.com/{group}.
If your project is not set please add it:

- Create a new project on `gitlab.com/{group}/Fuzi_project`
- Then populate it:

```bash
##   e.g. if group is "{group}" and project_name is "Fuzi_project"
git remote add origin git@github.com:{group}/Fuzi_project.git
git push -u origin master
git push -u origin --tags
```

Functionnal test with a script:

```bash
cd
mkdir tmp
cd tmp
Fuzi_project-run
```

# Install

Go to `https://github.com/{group}/Fuzi_project` to see the project, manage issues,
setup you ssh public key, ...

Create a python3 virtualenv and activate it:

```bash
sudo apt-get install virtualenv python-pip python-dev
deactivate; virtualenv -ppython3 ~/venv ; source ~/venv/bin/activate
```

Clone the project and install it:

```bash
git clone git@github.com:{group}/Fuzi_project.git
cd Fuzi_project
pip install -r requirements.txt
make clean install test                # install and test
```
Functionnal test with a script:

```bash
cd
mkdir tmp
cd tmp
Fuzi_project-run
```
