# 🚀 Como criar um site usando o Apache2

Este guia explica como instalar e configurar o Apache2 em uma máquina virtual Linux e publicar um site simples.

---

# 1️⃣ Preparação do ambiente

Baixe e instale uma distribuição Linux no VirtualBox (ex.: Ubuntu ou Debian).

Após a instalação, abra o terminal com:
- CTRL + ALT + T

---

# 2️⃣ Atualizar pacotes

Digite o comando abaixo para atualizar o sistema:

- sudo apt update && sudo apt upgrade -y

---

# 3️⃣ Instalar e habilitar o Apache2

Instale o Apache2:

- sudo apt install apache2 -y


Inicie e habilite o serviço:

- sudo systemctl start apache2
  
- sudo systemctl enable apache2


Verifique se está em execução:

- systemctl status apache2

---

# 4️⃣ Testar o servidor

Para saber o IP local da máquina:

- ip a


Agora, abra o navegador e acesse:

- http://seu-ip-local
  
ou

- http://localhost/

Você verá a página padrão do Apache2. ✅

---
