# ES6-docker-compose
Purpose

If you have multiple servers which have docker installed and you want to make them elasticsearch 6 nodes, you can use this. All that I found online was for nodes that reside on the same server and not with a dedicated machine per node. Hope this will help others.
Nodes are connected via network and they reside in docker containers under different servers/vms.

Prerequisites

1. Docker
2. Docker-compose
3. Git


Instalation

1. Install docker-compose using whatever method you want, I suggest using below command line
curl -L https://github.com/docker/compose/releases/download/1.18.0-rc2/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose
   chmod +x /usr/local/bin/docker-compose

2. git clone https://github.com/ChuckB0ris/ES6-docker-compose.git
3. cd ES6-docker-compose/
4. Start modifying the docker-compose.yml and es6.yml as you need them to be configured(vim docker-compose.yml vim es6.yml)
5. After you are done with that from the ES6-docker-compose folder run "docker-compose up" and you should be good. You might need to run with sudo if not root.
