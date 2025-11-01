# YouTubeDownloader
Downloader
# Permitir acceso a almacenamiento
termux-setup-storage

# Actualizar Termux
pkg update -y && pkg upgrade -y

# Instalar dependencias necesarias
pkg install git python ffmpeg -y

# Actualizar pip
pip3 install --upgrade pip

# Clonar el repositorio correcto
git clone https://github.com/ralvarado9/YouTubeDownloader.git
cd YouTubeDownloader

# Instalar librerías Python necesarias
pip3 install yt-dlp colorama

# Crear carpeta para guardar descargas (opcional)
mkdir -p /sdcard/Download/YT

# Ejecutar el programa
python3 playlist.py
