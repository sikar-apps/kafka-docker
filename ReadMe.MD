# Generate a keyfile for MongoDB using
```bash
openssl rand -base64 756 > keyfile && chmod 400 keyfile
```
# Set the below environment variables:
```bash
export KEYFILE_PATH=$(pwd)/keyfile
```
# Run the below command to start the kafka cluster:
```bash
docker-compose up -d --build
```