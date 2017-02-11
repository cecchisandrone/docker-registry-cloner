# docker-registry-cloner
A tool to migrate Docker images from one registry to another

## Example usage
````
./docker-registry-cloner -i image1 -s https://registry:5000 -t https://registry2:5000 --source-credentials username,pass --target-credentials username,pass
````