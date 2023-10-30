Bioformats 7.0.1 (https://www.openmicroscopy.org/bio-formats/) Built with IKVM Maven SDK for .NET6.

#Installation
To add the bioformats_package using IKVM.Maven add the following to your project file.
```
<PropertyGroup>
  <MavenAdditionalRepositories>ome=https://artifacts.openmicroscopy.org/artifactory/maven/;edu.ucar=https://maven.scijava.org/content/repositories/public/;</MavenAdditionalRepositories>
</PropertyGroup> 
<ItemGroup>
    <MavenReference Include="bioformats_package">
      <GroupId>ome</GroupId>
      <ArtifactId>bioformats_package</ArtifactId>
      <Version>7.0.1</Version>
    </MavenReference>
    <MavenReference Include="cdm-core">
      <GroupId>edu.ucar</GroupId>
      <ArtifactId>cdm-core</ArtifactId>
      <Version>5.3.3</Version>
    </MavenReference>
</ItemGroup>
<Target Name="FixIkvmReference" AfterTargets="_GetMavenIkvmReferenceItems">
    <Message Importance="high" Text="$(IkvmMavenSdkDir)" />
    <ItemGroup>
        <IkvmReferenceItem Condition="'%(Identity)'=='maven$org.json:json:20230227'">
            <AssemblyVersion>1.0.0.0</AssemblyVersion>
        </IkvmReferenceItem>
    </ItemGroup>
</Target>
```