Los alias
https://gist.github.com/MiguelAngelRamos/cfb604f23ae02d804cacb1e1d41f2f59
Comandos para crear una llave ssh
Creamos la llave
ssh-keygen -t rsa -b 4096 -C "tu_email@gmail.com"
Comprobamos que existan llaves
ls -al ~/.ssh 
Evaluar el servidor SSH ver si esta funcionando.
eval $(ssh-agent -s)
Agregamos la llave privada a nuestro servidor
ssh-add ~/.ssh/id_rsa
Copiar nuestra llave publica vamos utilizar editor vi
vi ~/.ssh/id_rsa.pub 