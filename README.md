# docker-registry-cloner
A tool to migrate Docker images from one registry to another

## Command line reference
````
Usage: docker-registry-cloner [options]

  Options:

    -h, --help                        output usage information
    -V, --version                     output the version number
    -s, --source <required>           Source registry url (e.g. registry.org)
    -t, --target <required>           Target registry url (e.g. registry.org)
    -a, --source-credentials <items>  Credentials for source registry (e.g. username,password)
    -b, --target-credentials <items>  Credentials for target registry (e.g. username,password)
    -i, --include-images <items>      Include image names (e.g. image1,image2)
    -e, --exclude-images <items>      Exclude image names (e.g. image1,image2)
````
## Example usage
````
./docker-registry-cloner -i image1 -s https://registry:5000 -t https://registry2:5000 --source-credentials username,pass --target-credentials username,pass
````
