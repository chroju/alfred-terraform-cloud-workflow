alfred-tfcloud-workflow
=======================

[Terraform Cloud](https://www.terraform.io/docs/cloud/index.html) Workflow for [Alfred 4](https://www.alfredapp.com/) .

Setup
--------

Download the latest `.alfredworkflow` file from here and import it to your Alfred.

https://github.com/chroju/alfred-tfcloud-workflow/releases

You need to set some workflow environment variables.

| Variable name | Required | Description | Default |
|---|---|---|---|
| organization | yes | Your Terraform Cloud organization name | N/A |
| TF_CLI_CONFIG_FILE | no | See https://www.terraform.io/docs/commands/cli-config.html#development-overrides-for-provider-developers | N/A |

### Credentials

This workflow uses an API token in `$HOME/.terraformrc` . If you want to use an other file, set the path in the variable `TF_CLI_CONFIG_FILE` .

### Usage

3 commands are available. Search workspaces, registry modules, and Terraform current runs which needs a confirmation. Pressing enter will open the page for the selected workspace or registry module and runs.

```
tfcws <workspace>
tfcmd <registry module>
tfcruns <runs>
```

[![Usage sample](https://i.gyazo.com/a6ddc5a3f1aee2d8a41f5fc43639138e.gif)](https://gyazo.com/a6ddc5a3f1aee2d8a41f5fc43639138e)
