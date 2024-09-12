# Buildroot SBOM Action
This github action generates the `legal-info` and generates the Cyclone DX SBOM
for a given buildroot output directory. 

The action expects to be given a buildroot output folder, and will call
`make legal-info` and `make show-info` to complete its task.

The action publishes the tarball of all legal info and the software SBOM to the 
pipeline's artefacts. 