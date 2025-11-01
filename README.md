# YouTubeDownloader
Downloader
# 1) Permisos, actualizar e instalar herramientas básicas
termux-setup-storage             # concede acceso a /sdcard (acepta la ventana en Android)
pkg update -y && pkg upgrade -y
pkg install git python ffmpeg -y

# 2) Usar pip3 (asegúrate que pip apunte a Python3)
pip3 install --upgrade pip

# 3) Instalar las dependencias Python requeridas por el repo
pip3 install yt-dlp colorama

# 4) Clonar el repositorio (cámbialo si ya lo descargaste)
git clone https://github.com/imraj569/YouTube_Downloader.git
cd YouTube_Downloader

# 5) Verifica los archivos y abre playlist.py para ver opciones (útil para saber argumentos)
ls -la
sed -n '1,200p' playlist.py    # muestra las primeras 200 líneas (lee la ayuda/instrucciones del script)
# o
python3 playlist.py --help     # algunos scripts muestran ayuda con --help
