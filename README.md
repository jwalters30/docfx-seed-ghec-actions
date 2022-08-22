# docfx-seed
[![Build status](https://ci.appveyor.com/api/projects/status/psjd5g56kr0vayiw?svg=true)](https://ci.appveyor.com/project/qinezh/docfx-seed)

View the GitHub Pages site at https://jwalters30.github.io/docfx-seed-ghec-actions/ 

## Description
This is a sample docfx documentation project. It contains .NET source code and markdown files.
`docfx.json` is the configuration file for running `docfx`.
`docfx` will generate a static website as similar to http://docascode.github.io/docfx-seed/index.html

## How to run 
### Under Windows
#### Install from Nuget
* Install [Nuget.exe](https://dist.nuget.org/index.html)
* Create a folder, e.g. *C:\Tools\docfx*, under the folder, `nuget install docfx.console`
* Open command line: 
```batch
set PATH=%PATH%;C:\Tools\docfx\docfx.console\tools
docfx docfx-seed\docfx.json --serve
```
#### Install from choco
* Install [chocolatey](https://chocolatey.org/install)
* Open command line:
```batch
choco install docfx
docfx docfx-seed\docfx.json --serve
```

### Cross platform
* Install [Mono](http://www.mono-project.com/download/#download-lin)
* Install [Nuget.exe](https://dist.nuget.org/index.html)
```sh
> mono nuget.exe install docfx.console
> mono docfx.console/tools/docfx.exe docfx-seed/docfx.json
```

## Further information about `docfx`
`docfx` is a tool to generate documentation towards .NET source code and markdown files. Please refer to [docfx](http://dotnet.github.io/docfx/tutorial/docfx_getting_started.html) to get start. The `docfx` website itself is generated by `docfx`!
