# owncloud
Primer tens que actualitzar les llistes de paquets i actualitzar tots els paquets existents al vostre sistema.
###### sudo apt install software-properties-common -y
Ara instal·les les eines necessàries per treballar amb els arxius de paquets personals (PPA).
###### LC_ALL=C.UTF-8 sudo add-apt-repository ppa:ondrej/php -y
Una vegada ja has instal·lat les eines, actualitza els repositoris:
###### sudo apt update
Ara toca Instalar les llibreries de PHP de la versió 7.4 utilitzant els codigs següents:
###### sudo apt install php7.4 -y
###### sudo apt install -y php libapache2-mod-php7.4
###### sudo apt install -y php7.4-fpm php7.4-common php7.4-mbstring php7.4-xmlrpc php7.4-soap php7.4-gd php7.4-xml php7.4-intl php7.4-mysql php7.4-cli php7.4-ldap php7.4-zip php7.4-curl
Seleccioneu la versió de PHP que voleu:
###### sudo update-alternatives --config php
Activa els mòduls d'apache2 necessaris:
###### sudo a2enmod proxy_fcgi setenvif
###### sudo a2enconf php7.4-fpm
Reinicieu l'apache2:
###### sudo service apache2 restart
