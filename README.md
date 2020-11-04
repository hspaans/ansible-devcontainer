# Devcontainer for Ansible

## Using within you project

Add `.devcontainer/devcontainer.json` to your repository.

```json
{
  "image": "ghcr.io/hspaans/ansible-devcontainer:latest",
  "name": "Ansible",
  "settings": {
    "terminal.integrated.shell.linux": "/bin/bash"
  },
  "appPort": [],
  "postCreateCommand": "ansible-galaxy install -r roles/requirements.yml",
  "remoteUser": "vscode",
  "extensions": [
    "github.vscode-pull-request-github",
    "ms-python.python",
    "redhat.vscode-yaml"
  ]
}
```
