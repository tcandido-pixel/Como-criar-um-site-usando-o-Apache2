# Como criar um site usando o Apache2

Este guia explica como instalar e configurar o Apache2 em uma máquina virtual Linux e publicar um site simples.

---------------------------------------------------------------------------------------------------------------

# 1️⃣ Preparação do ambiente

Baixe e instale uma distribuição Linux no VirtualBox (ex.: Ubuntu ou Debian).

Após a instalação, abra o terminal com:

- ```CTRL + ALT + T```

---

# 2️⃣ Atualizar pacotes

Digite o comando abaixo para atualizar o sistema:

- ```sudo apt update && sudo apt upgrade -y```

---

# 3️⃣ Instalar e habilitar o Apache2

Instale o Apache2:

- ```sudo apt install apache2 -y```


Inicie e habilite o serviço:

- ```sudo systemctl start apache2```
  
- ```sudo systemctl enable apache2```


Verifique se está em execução:

- ```systemctl status apache2```

---

# 4️⃣ Testar o servidor

Para saber o IP local da máquina:

- ```ip a```


Agora, abra o navegador e acesse:

- ```http://seu-ip-local```
  
ou

- ```http://localhost/```

Você verá a página padrão do Apache2. ✅

---

# 5️⃣ Editar arquivos do site

Entre no diretório do site:

- ```cd /var/www/html/```
  
- ```ls```

Remova o arquivo padrão:

- ```sudo rm -rf index.html```

Crie um novo arquivo index.html:

- ```sudo nano index.html```

Digite um exemplo simples em HTML:
```
<html>
<head><tittle>titulo</tittle>
</head>
<body>
<h1>Bem vindo a minha primeira pagina HTML</h1>
</body>
</html>
```
Salve (CTRL + O + ENTER) e saia (CTRL + X).
Atualize a página no navegador para ver o resultado.

---

# 6️⃣ Usar um site pronto do GitHub

Antes de clonar, instale o Git:

- ```sudo apt install git -y```

Clone um site pronto (exemplo do Matheus):

- ```sudo git clone https://github.com/matheusmanuel/site-simples-com-html-e-css-.git```

Acesse a pasta clonada:

- ```cd site-simples-com-html-e-css-```
- ```ls```

Volte para a pasta anterior: 

- ```cd ..```
  
Apague o arquivo index.html:

- ```sudo rm -rf index.html```
  
Copie os seguintes arquivos:

- ```sudo cp site-simples-com-html-e-css-/index.html```

- ```sudo cp site-simples-com-html-e-css-/style.css```

- ```sudo cp site-simples-com-html-e-css-/background.jpg```

- ```sudo cp site-simples-com-html-e-css-/Como-Criar-um-SITE-Com-HTML-e-CSS-na-pràtica.png```

Remova o arquivo baixado:

- ```sudo rm -rf site-simples-com-html-e-css-/```
  
Copie os arquivos para /var/www/html/ e recarregue a página no navegador.
