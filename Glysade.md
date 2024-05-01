
# Glysade build intstructions

Using powershell

```
.\build.ps1
```

Then in Linux

```
cd solution
dotnet.exe pack /p:ApiCompatGenerateSuppressionFile=true NPOI.Pack.csproj
```

The nuget package is in Release. To install locally without uploading to nuget.org

```
cd Release
nuget.exe init . 'C:\Users\jones\.nuget\packages' -Expand
```


