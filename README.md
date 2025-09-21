# Como não criar um site usando o Apache2 🫠
Primeiro iremos baixar o ubuntu ou qualquer outra distribuição linux para usar no virtual box.
Depois de instalar o sistema, vamnos abrir o terminal usando as teclas CTRL + ALT + T
Agora vamos atualizar o catalaogo digitando o seguinte comando: sudo apt update && sudo apt upgrade -y
Depois instale o apache2 digitando o seguinte comando: sudo apt install apache2 -y
agora vamos iniciar e habiliatar os serviços digitando primeiro sudo systemctl start apache2 e depois sudo systemctl enable apache2
verifique se está rodando: systemctl status apache2

