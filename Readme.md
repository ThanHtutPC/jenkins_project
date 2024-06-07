Docker installation 

```bash
sudo apt update
sudo apt-get install ca-certificates curl gnupg
sudo install -m 0755 -d /etc/apt/keyrings; curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg; sudo chmod a+r /etc/apt/keyrings/docker.gpg
echo "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu $(. /etc/os-release && echo "$VERSION_CODENAME") stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
cd /etc/apt/sources.list.d/
sudo apt-update
2033  sudo apt-get install docker-ce docker-ce-cli containerd.io docker-compose-plugin
```

Installation jenkins

```bash
	docker network create jenkins
	docekr build -t <name:tags> .
	docker-compose up -d
```

Verify the docker

```bash
docker network lss
docker images 
docker ps 
```

http://<your ip address>:8080

Run the  docker logs jenkins-blueocean copy password and add the “administration password”

Installation with packages