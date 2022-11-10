# Schema store for METRO.digital

This repository is intended to distribute JSON schemas used inside METRO.digital.

## How to add a JSON schema to VSCode to validate `yaml` files?

1. This requires to have a special plugin installed.
    It is the plugin *YAML Language Support by Red Hat.*
1. Go to the menue *File-->Preferences-->Settings*
1. Decide whether you want to do this change for every project (tab *User*) or 
    only for a single project (tab *Workspace*)
1. Search for *yaml schema*
1. Find the section *Yaml: Schemas* on the right hand side and 
    klick on *Edit in settings.json*
1. Add the schema for a file

    ```yaml
    "yaml.schemas": {
        "https://raw.githubusercontent.com/metro-digital-inner-source/md-schema-store/master/repository/waas.json": "waas.yaml",
    },

    ```

For more information see the documentation of the used vscode plugin:

[YAML Language Support by Red Hat](https://github.com/redhat-developer/vscode-yaml)

## Information about the hosted schemas

Some useful information on a schema level.

### waas.json

This schema is only supporting validation
for [WaaS v2](https://github.com/metro-digital-inner-source/waas/blob/master/documentation/apiVersion/waas-v2/v2.yaml).
