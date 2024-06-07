Installation Jenkins with packages

Jenkins packages installation 

```jsx
sudo wget -O /usr/share/keyrings/jenkins-keyring.asc \
  https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key
echo "deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc]" \
  https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
sudo apt-get update
sudo apt-get install jenkins
```

Java JRE installation

```bash
sudo apt update
sudo apt install fontconfig openjdk-17-jre
```

User modify 

```bash
useradd Jenkins
usermod -aG docker Jenkins
ls -dl /var/run/docker.sock
sudo systemctl restart docker
```