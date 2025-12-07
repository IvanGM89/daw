Instalacion del servidor FTP

1º Instalacion de vsftpd

- Actualizar paquetes con sudo apt update && sudo apt upgrade
- Instalar el servidor FTP vsftpd con sudo apt install vsftpd
- comprobar el estado del servicio con sudo systemctl status vsftpd

2º Configuracion basica de vsftpd

- Crear una copia de seguridad de /etc/vsftpd.conf
- Editar dicho archivo con los patrones adecuados dicho en los apuntes
- Reiniciar el servicio con sudo systemctl restart vsftpd

3º Creacion del usuario FTP

- Crear el usuario con sudo useradd -m y asignarle una contraseña con sudo passwd

4º Conexion desde el cliente Filezilla

- instalar o abrir filezilla si ya lo tienes instalado
- Rellenar los campos adecuados para ejercer conexion en este caso ip, usuario, contraseña y puerto
- Una vez se ha establecido la conexion crear una carpeta y subir un archivo desde el ordenador anfitrion.
