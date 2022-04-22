# Apka pogodowa Usługi i platformy deweloperskie

Do wykonania apki użyłem HTML5, CSS oraz JavaScript, mamy możliwość sprawdzenia pogody w dowolnym mieście, wystarczy wprowadzić nazwe miasta do search bara i wcisnąć przycisk wyszukaj. Do upiększenia użyłem baze darmowych zdjęć z unsplash.  
![image](https://i.imgur.com/3tbXdAY.png)

## Api
W celu utworzenia apki pogodowej wykożystałem API openweathermap, feczuje z API potrzebne informacje a następnie je wyświetlam
## Lokalne środowisko
 - [Visual Studio Code](https://code.visualstudio.com/)🔥
 - [VMWare Workstation](https://www.vmware.com/products/workstation-player/workstation-player-evaluation.html)🖥
 - [Docker](https://www.docker.com/) 🐋
 - Linux- twój preferowany 🎉 
## Komendy
![image](https://i.imgur.com/yxUmfjG.png)
```bash
az login --use-device-code // używam wirtualnej maszyny
```
```bash
az group create -n projekt -l westeurope
```
![image](https://i.imgur.com/1LXH4ZZ.png)
```bash
az vm create --resource-group projekt --name virtualmachine --size "Standard_B1ls" --image "Canonical:0001-com-ubuntu-server-focal:20_04-lts-gen2:latest" --public-ip-sku Standard --admin-username ubuntu
```
![image](https://i.imgur.com/nsXcugt.png)
```bash
sshubuntu@20.23.40.95 
```
```bash
sudo apt-get update
```
#instalacja dockera i nginx na virtualce 
```bash
sudo apt-get install docker.io
sudo docker pull nginx
```
![image](https://i.imgur.com/1bcSIih.png)
```bash
docker build -t html-server-image:v1 .
docker tag html-server-image:v1 nimranos/html-server-image
```
![image](https://i.imgur.com/6wjroEP.png)
```bash
sudo docker run -d -p 5000:5000 nimranos/html-server-image:latest nginx
```
![image](https://i.imgur.com/3OD8yKb.png)

## ⭐️More⭐️
 - [Deploy NGINX z Dockerem](https://www.nginx.com/blog/deploying-nginx-nginx-plus-docker/)
 - [API](https://openweathermap.org/)
 - [Dokumentacja Dockera](https://docs.docker.com/) 
 - [Dokumentacja Nginx](http://nginx.org/en/docs/)
 - [Azure](https://portal.azure.com/)
 - [Fetch API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API)
 - [Git Cheatsheet](https://education.github.com/git-cheat-sheet-education.pdf) 