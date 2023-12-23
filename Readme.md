[![NuGet version (BioFormatsNET6)](https://img.shields.io/nuget/v/BioFormats.NET6.svg)](https://www.nuget.org/packages/BioFormats.NET6/7.1.0)
[![NuGet version (BioFormatsNET6)](https://img.shields.io/nuget/dt/BioFormats.NET6?color=g)](https://www.nuget.org/packages/BioFormats.NET6/7.1.0)

Bioformats 7.1.0 (https://www.openmicroscopy.org/bio-formats/) Built with IKVM 8.7.3 Maven SDK for .NET6.
For x64 use the nuget package version of the project by installing it from [![NuGet version (BioFormatsNET6)](https://img.shields.io/nuget/v/BioFormats.NET6.svg)](https://www.nuget.org/packages/BioFormats.NET6/7.1.0.1)
For ARM use the Maven version of the project by installing the latest IKVM Maven SDK and adding this to your project file:
```
<PropertyGroup>
  <MavenAdditionalRepositories>ome=https://artifacts.openmicroscopy.org/artifactory/maven/;edu.ucar=https://maven.scijava.org/content/repositories/public/;</MavenAdditionalRepositories>
</PropertyGroup> 
<ItemGroup>
    <MavenReference Include="bioformats_package">
      <GroupId>ome</GroupId>
      <ArtifactId>bioformats_package</ArtifactId>
      <Version>7.1.0</Version>
    </MavenReference>
    <MavenReference Include="cdm-core">
      <GroupId>edu.ucar</GroupId>
      <ArtifactId>cdm-core</ArtifactId>
      <Version>5.3.3</Version>
    </MavenReference>
    <MavenReference Include="guava-jdk5">
      <GroupId>com.google.guava</GroupId>
      <ArtifactId>guava-jdk5</ArtifactId>
      <Version>13.0</Version>
    </MavenReference>
</ItemGroup>
```
