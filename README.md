# VisioComAddinNet5
Visio Addin based on .NET 5 (core) "Hello World" example. Adds a two buttons to the ribbon.
Basically the same as the starter project created by my main extension, but for .NET 5 (core)

![](https://i.paste.pics/944464cd1fc1a9999dfcc8912c9920a0.png)

The base wizard for the "normal" .NET:

https://marketplace.visualstudio.com/items?itemName=NikolayBelyh.ExtendedVisioAddinProject

Changes include:
- retargeting everything to use .net5-windows
- adding windows forms support
- allow com hosting
- Fix the method that reads bitmaps from resources
- Replacing PIA references with COM references
- Fix the installer to use AppId
- Fix the installer to use self-registration
```
  <PropertyGroup>
    <TargetFramework>net5.0-windows</TargetFramework>
    <UseWindowsForms>true</UseWindowsForms>
    <EnableComHosting>true</EnableComHosting>
  </PropertyGroup>
```
