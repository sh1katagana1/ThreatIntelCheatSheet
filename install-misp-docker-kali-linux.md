# Install MISP on Kali Linux

The best way is the production ready docker version at https://github.com/MISP/misp-docker. Kali can install Docker with no issue, so run this:
```
apt update
apt install -y docker.io
systemctl enable docker --now
```

The MISP one needs Docker Compose, which Kali does not have a repository for, so you would want to manually install it. Run this Bash script to do it and it will make it as a Docker plugin inside of the .docker folder of Root:

```
echo "deb [arch=amd64 signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/debian bookworm stable" | tee /etc/apt/sources.list.d/docker.list
curl -fsSL https://download.docker.com/linux/debian/gpg | gpg --dearmor -o /etc/apt/keyrings/docker.gpg
apt update
apt install -y docker-ce docker-ce-cli containerd.io
```
Now clone the MISP docker GitHub, cd to it and do:
```
docker compose pull
```
This will grab all necessary files. Now to get it running so you can go to it in a browser locally:
```
docker compose up
```
This takes a bit of time, you will know when its done when nothing else is being installed. You then open up a browser and go to https://localhost. The default credentials are:
```
User: admin@admin.test
Password: admin
```
Troubleshooting:
When I tried this initially on my Kali Linux, I got this error when I did docker compose up: dependency failed to start: container misp-docker-misp-modules-1 is unhealthy

It seemed to fix it when i ran:
```
docker logs misp-docker-misp-modules-1
```
I think this started the service, but it continued with the MISP initiation. 










