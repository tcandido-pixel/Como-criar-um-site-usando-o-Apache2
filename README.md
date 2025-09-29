# Como criar um site usando o Apache2 
Primeiro iremos baixar o ubuntu ou qualquer outra distribuição linux para usar no virtual box. Irei usar o debian.
Depois de instalar o sistema, vamnos abrir o terminal usando as teclas CTRL + ALT + T.
Agora vamos atualizar o catalaogo digitando o seguinte comando: sudo apt update && sudo apt upgrade -y.
Depois instale o apache2 digitando o seguinte comando: sudo apt install apache2 -y.
agora vamos iniciar e habiliatar os serviços digitando primeiro: sudo systemctl start apache2 e depois: sudo systemctl enable apache2.
verifique se está rodando: systemctl status apache2.
Agora vamos verificar qual o IP esta rodando o site. No terminal digite: ip a.
Depois de encontrar o ip local, teste no navegador. irá aparecer um site exemplo. Caso não tenha localizado o seu ip, pode acesar o site digitando http://localhost/.
Agora iremos fazer alguns exemplos. vamos localizar o diretorio. no terminal digite: cd /var/www/html/. depois iremos listar, digite: ls.
veja que o site é apenas o index.html. vamos modificar para exemplo de como funciona.
remova o arquivo com o comando: sudo rm -rf index.html. Agora vamos criar outro arquivo com o mesmo nome e iremos modificar. digite: sudo nano index.html.
Digite o mesmo codigo simples HTML para teste. depois saia do nano CTRL + X e enter para confirmar e CTRL + O para salvar.
Atualize a pagina e veja como ficou. 
Agora iremos melhorar o site com alguns exemplos disponiveis na internet. escolhi o site pronto do matheus.(https://github.com/matheusmanuel/site-simples-com-html-e-css-)
Para instalar, iremos fazer a clonagem dos arquivos. mas antes vamos instalar o github com o seguinte comando: sudo apt install git -y.
