# serverJellyfin

server Jellyfin
Este es un archivo de Docker Compose, que define un conjunto de contenedores que se despliegan juntos como parte de una aplicación o sistema. Cada servicio en el archivo Compose especifica una imagen de Docker a utilizar, así como otras opciones de configuración.

En este caso, hay cinco servicios definidos:

jellyfin: Este servicio proporciona un servidor multimedia basado en Jellyfin. Está configurado para usar varios volúmenes, incluyendo uno para la configuración, otro para la caché y otros dos para los archivos multimedia. El servicio se expone en el puerto 8096 y se configuró para reiniciarse automáticamente a menos que se detenga explícitamente.

radarr: Este servicio proporciona un gestor de descargas para películas. También está configurado para usar un volumen para la configuración, así como otro volumen para los archivos de películas y descargas. El servicio se expone en el puerto 7878 y se configuró para reiniciarse automáticamente a menos que se detenga explícitamente.

sonarr: Este servicio proporciona un gestor de descargas para programas de televisión. Al igual que los otros servicios, se configura con un volumen para la configuración y otro volumen para los archivos de televisión y descargas. El servicio se expone en el puerto 8989 y se configuró para reiniciarse automáticamente a menos que se detenga explícitamente.

prowlarr: Este servicio proporciona un gestor de descargas para cómics. Está configurado para usar un volumen para la configuración y se expone en el puerto 9696. El servicio se configuró para reiniciarse automáticamente a menos que se detenga explícitamente.

qbittorrent: Este servicio proporciona un cliente de BitTorrent basado en qBittorrent. Está configurado para usar un volumen para la configuración, otro para los archivos descargados y se expone en los puertos 8080 y 6881 (para conexiones de red BitTorrent). El servicio se configuró para reiniciarse automáticamente a menos que se detenga explícitamente.
