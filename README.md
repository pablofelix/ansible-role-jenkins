Jenkins Ansible Role
====================
This role installs and configures Jenkins on a OpenShift cluster.

Requirements
------------
This role requires Ansible 2.9 or higher, molecule, an OpenShift cluster and a user logged.

collections
-----------
- kubernetes.core
- podman.podman

Role Variables
--------------
The variables that can be passed to this role and a brief description about them are as follows:

| Name | Default Value | Description |
|------|---------------|-------------|
| jenkins.project | jenkins-pipeline | The namespace where Jenkins will be installed |
| jenkins.base.image | jenkins/jenkins | The base image to use |
| jenkins.image.tag | 2.396 | The tag of the base image to use |
| jenkins.plugins | [] | A list of plugins to install |
| jenkins.containerfile.name | Containerfile | The containerfile to use |
| jenkins.containerfile.path | tmp | The path of the containerfile |
| jenkins.image.name | jenkins | The name of the image to build |
| jenkins.image.tag | latest | The tag of the image to build |


