Bioformats 7.0.0 (https://www.openmicroscopy.org/bio-formats/) Built with ikvm 8.6.2 for .NET6.
Add nuget package IKVM to your project to use this library.

# Building
Generated with the latest version of bioformats_package.jar with ikvmc.exe. As well as the following dependencies placed in folder "dependencies" in the same folder as ikvmc.exe the dependencies can be downloaded from Maven.
- google-collect.1.0.jar

Then running ikvmc.exe from command line with the following command:

```./ikvmc bioformats_package.jar -target:library -recurse:dependencies *> output.txt```

This will generate the dll bioformats_package.dll.
