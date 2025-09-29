# Como não criar um site usando o Apache2 🫠
Primeiro iremos baixar o ubuntu ou qualquer outra distribuição linux para usar no virtual box. Irei usar o debian.
Depois de instalar o sistema, vamnos abrir o terminal usando as teclas CTRL + ALT + T.
Agora vamos atualizar o catalaogo digitando o seguinte comando: sudo apt update && sudo apt upgrade -y.
Depois instale o apache2 digitando o seguinte comando: sudo apt install apache2 -y.
agora vamos iniciar e habiliatar os serviços digitando primeiro: sudo systemctl start apache2 e depois: sudo systemctl enable apache2.
verifique se está rodando: systemctl status apache2.
Agora vamos verificar qual o IP esta rodando o site. No terminal digite: ip a.
Depois de encontrar o ip local, teste no navegador. irá aparecer um site exemplo. Caso não tenha localizado o seu ip, pode acesar o site digitando http://localhost/.
Agora iremos melhorar o site. vamos localizar o diretorio. no terminal digite: cd /var/www/html/. depois iremos listar, digite: ls.
veja que o site é apenas o index.html. vamos modicar para exemplo de como funciona.
remova o arquivo com o comando: sudo rm -rf index.html. Agora vamos criar outro arquivo com o mesmo nome e iremos modificar. digite: sudo nano index.html.

