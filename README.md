[Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Here-Cheatsheet)
# MINISHIFT SHOOTING LINE ;)
============

## Installation


## Terminology
|Acronym|Description|
|:------:|:------:|
|OCP|OpenShift Container Platform|
|OC| OpenShift Client (Command)|
|CLI|Command Line Interface|
|DC|Deployment Config|
|BC|Build Config|
|IS|Image Stream|
|SA|Service Account|
|PV|Persistent Volume|
|PVC|Persistent Volume Claim|


> Note:
	:warning: - Atention / Alert
	:information_source: - Information

## Running minishift
> On CLI run the commands bellow:
```bash
$ minishift start [--memory=4GB]

"Setting variable environment into bashrc file!"
$ minishift oc-env >> ~/.bashrc

"Web console"
$ minishift console --url

"Check Openshift Client (OC) command"
$ oc status
In project My Project (myproject) on server https://192.168.42.200:8443

You have no services, deployment configs, or build configs.
Run 'oc new-app' to create an application.
```

### Working with projects
> Create project
```bash
"Logging on CLI"
$ oc login -u <username> -p <password> "Log With user developer and pass developer"

"Show all projects"
$ oc projects 

"Creating a project called myproject"
$ oc new-project myproject --display-name="Sample Project" --description="Project created just for trainning."
```

### Clean up all about minishift
> To clean up all minishift instances and configuration. 
> Run the commands below:
```bash
$ sudo virsh list --all
$ sudo virsh destroy minishift
$ sudo virsh undefine minishift
$ rm -rf ~/.minishift/machine
$ rm -rf ~/.minishiff
```

## Problems and solutions

