% Utviklingsmiljøer 
% docker og fig
% Sigurd Fosseng, Sopra Steria

# "Tradisjonelt"

## Slik installerer ..

- mongodb
- mysql
- python
- node + grunt + bower +++
- django
- jdk 8

osv..

## I alle OS

- Windows
- Linux
- OS X

## Dying Wiki
    
![Development Environment](img/devenv.png)

## Prod?

![](img/notdevops.png)

## Løsninger

Vagrant, VM, installasjons-script

.

eller **fig**, som bruker **docker**.


# ![](img/docker.png)


## ![](img/devops.png)

## Hva

- Lettvekts virtualisering
- enkel deploy til alle systemer som kjører Docker
- shipping-container for ditt program.
- pack, ship, run programmet i isolert miljø, enkelt.

## Hva

- skrevet i golang
- Kjernestøtte i linux
- virtualiserings overhead er veldig lavt. (0 kost vs native prosess)
- isolert miljø

## ![](img/docker-filesystems-multilayer.png)

## ![](img/notdevops.png)

## 

```
FROM php:5.6-cli
COPY . /usr/src/myapp
WORKDIR /usr/src/myapp
CMD [ "php", "./your-script.php" ]

```
 /Dockerfile

## ![](img/dockerbuild.png)
## Kjapp demo

# [Fig](http://www.fig.sh/)

## forenkler docker
- et verktøy for å håndtere docker
- kan kjøre opp flere containere
- lenke containere sammen
- defineres i en `fig.yml` fil

## demotime

## limits
- fungerer ikke optimalt på windows
- snart utdatert (blir en del av docker)

# ![](img/doge.jpg)

## ikke helt devops
- bare første steg på en lang stige opp til devops-himmelen
