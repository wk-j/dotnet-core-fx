## FX

[![Build Status](https://dev.azure.com/wk-j/dotnet-core-fx/_apis/build/status/wk-j.dotnet-core-fx?branchName=master)](https://dev.azure.com/wk-j/dotnet-core-fx/_build/latest?definitionId=56&branchName=master)


```bash
dotnet new classlib \
    --language C# \
    --output src/MyLibrary \
    --framework net45

dotnet new classlib \
    --language C# \
    --output src/MyLibrary \
    --target-framework-override  net45

dotnet add src/MyLibrary/MyLibrary.csproj \
    package Microsoft.NETFramework.ReferenceAssemblies \
    --version 1.0.0-preview.2

dotnet build src/MyLibrary/MyLibrary.csproj
```