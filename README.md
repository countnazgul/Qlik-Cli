## About
Qlik-Cli is a PowerShell module that provides a command line interface for managing a Qlik Sense environment. The module provides a set of commands for viewing and editing configuration settings, as well as managing tasks and other features available through the APIs.
## Installation
The module can be installed by copying the Qlik-Cli.psm1 file to C:\Windows\System32\WindowsPowerShell\v1.0\Modules\Qlik-Cli\, the module will then be loaded and ready to use from the PowerShell console. You can also load the module using the Import-Module command.
```sh
Import-Module Qlik-Cli.psm1
```
Once the module is loaded you can view a list of available commands by using the Get-Help PowerShell command.
```sh
Get-Help Qlik
```
## Examples
A number of files are provided to demonstrate the use of the module with Vagrant to automate the deployment of a multi-node Qlik Sense environment, this requires that Vagrant and VirtualBox are installed and can be used by running Vagrant commands in the folder where this repository has been cloned.
```sh
vagrant up
```
The installation requires a valid Qlik Sense Site License, and the license details need to be entered into the license.json file, without this none of the APIs will be available and so the Qlik-Cli commands will not work. The license details in the license.json file will be read by the deployment scripts and applied automatically.