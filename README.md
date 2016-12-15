deployment-images

Repository contains docker images for SFTP/FTP/FTPS services.

It provides a SFTP server:
 * Host: localhost
 * Port: 2022
 * Username: jetbrains
 * Password: jetbrains
 * Folder mapping: `/tmp:/home/jetbrains/upload`
 
Please adjust line: `~/.ssh/id_rsa.pub:/home/jetbrains/.ssh/keys/id_rsa.pub:ro` such that the first part is point to your pub key. 
That will allow you to login using your key.

FTP server:
 * Host: localhost
 * Port: 21
 * Username: jetbrains
 * Password: jetbrains
 * Folder mapping: `/tmp:/home/virtual/jetbrains/share`
 
Please adjust `PASV_ADDRESS` to be your local ip address. 

FTPS server:
 * Host: localhost
 * Port: 23
 * Username: jetbrains
 * Password: jetbrains
 * Authentification: explicit
 * Folder mapping: `/tmp:/home/virtual/jetbrains/share`
 
Please adjust `PASV_ADDRESS` to be your local ip address.
