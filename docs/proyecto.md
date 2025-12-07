## Instalacion del servidor FTP

1. Instalacion de vsftpd

   - Actualizar paquetes con sudo apt update && sudo apt upgrade
   - Instalar el servidor FTP vsftpd con sudo apt install vsftpd
   - comprobar el estado del servicio con sudo systemctl status vsftpd

2. Configuracion basica de vsftpd

   - Crear una copia de seguridad de /etc/vsftpd.conf
   - Editar dicho archivo con los patrones adecuados dicho en los apuntes
   - Reiniciar el servicio con sudo systemctl restart vsftpd

3. Creacion del usuario FTP

   - Crear el usuario con sudo useradd -m y asignarle una contraseña con sudo passwd

4. Conexion desde el cliente Filezilla

   - instalar o abrir filezilla si ya lo tienes instalado
   - Rellenar los campos adecuados para ejercer conexion en este caso ip, usuario, contraseña y puerto
   - Una vez se ha establecido la conexion crear una carpeta y subir un archivo desde el ordenador anfitrion.


## Plan de despliegue

Para desplegar el servidor FTP se siguen los siguientes pasos:

1. Actualizar el sistema:
   - sudo apt update && sudo apt upgrade

2. Instalar el servidor FTP vsftpd:
   - sudo apt install vsftpd

3. Comprobar el estado del servicio:
   - sudo systemctl status vsftpd

4. Crear una copia de seguridad de la configuración:
   - sudo cp /etc/vsftpd.conf /etc/vsftpd.conf.bak

5. Editar el archivo de configuración /etc/vsftpd.conf
   con los parámetros indicados en los apuntes.

6. Reiniciar el servicio:
   - sudo systemctl restart vsftpd

7. Crear usuario FTP:
   - sudo useradd -m ftp_user
   - sudo passwd ftp_user

8. Conectarse desde FileZilla usando:
   - IP del servidor
   - Usuario FTP
   - Contraseña
   - Puerto 21
