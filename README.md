# WebJobV3

- Documentation to build this **WebJob** -> [WebJob Documentation](https://learn.microsoft.com/en-us/azure/app-service/webjobs-sdk-get-started)

## The necessary packages for running WebJobs SDK V3 (.NET Core)
- _Note: WebJobs SDK Version 1 is .NET Framework_

### Packages:
- Notes: `<ImplicitUsings>disable</ImplicitUsings>` is for ensuring direct correlations to the to **namespaces** and **Modules**/**NuGet Packages**

``` xml
<Project Sdk="Microsoft.NET.Sdk">

  <PropertyGroup>
    <OutputType>Exe</OutputType>
    <TargetFramework>net6.0</TargetFramework>
    <ImplicitUsings>disable</ImplicitUsings>
    <Nullable>enable</Nullable>
  </PropertyGroup>

  <ItemGroup>
    <PackageReference Include="Microsoft.Azure.WebJobs.Extensions" Version="4.0.1" />
    <PackageReference Include="Microsoft.Azure.WebJobs.Extensions.Storage" Version="5.2.2" />
    <PackageReference Include="Microsoft.Extensions.Logging.Console" Version="6.0.0" />
  </ItemGroup>

  <ItemGroup>
    <None Update="appsettings.json">
      <CopyToOutputDirectory>Always</CopyToOutputDirectory>
    </None>
  </ItemGroup>

</Project>
```
