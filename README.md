AWS Dynamic DNS Syncronizer
====

This script reads the current external IP where the script is executed from and syncronizes it with the HostedZone ```alfonsimeri.net.``` in AWS

Requirements
---
* Python 2.7
* pip

Usage Instructions
---
You could just install the dependencies:

```
pip install -r requirements.txt
```

and execute the script:

```
./bin/dnssync
```

Docker
---
If you want to use docker just run:

```
docker build -t dnssync .
docker run -e "AWS_ACCESS_KEY_ID=your_key_id" -e "AWS_SECRET_ACCESS_KEY=your_secret_access_key" -it --rm --name dnssync dnssync
```
