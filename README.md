# Crud

# Introdução  

Este projeto é um sistema CRUD (Create, Read, Update, Delete) desenvolvido em PHP e MySQL, utilizando PHPMyAdmin para gerenciar o banco de dados.  

# Funcionalidades  

Criar registros no banco de dados  
Listar registros cadastrados  
Editar registros existentes  
Excluir registros  

# Tecnologias Utilizadas
PHP (https://www.php.net/) (versão 4.4 ou superior)  
MySQL  (https://www.mysql.com/)  
PHPMyAdmin  (https://www.phpmyadmin.net/)  
Acesso a um servidor de alojamento (como o Alojamento-Ratis que foi usado para este projeto) com suporte a PHP e MySQL.
# Estrutura do Projeto  

```bash
├── /css/                     # Pasta que guarda o css  
│     ├── style.css           # Arquivo de css  
├── /imges/                   # Paste onde tem algumas imagens para teste
        ├──food-1.png         # Imagem de teste 1  
        ├──food-2.png         # Imagem de teste 2  
        ├──food-3.png         # Imagem de teste 3  
        ├──food-4.png         # Imagem de teste 4  
        ├──food-5.png         # Imagem de teste 5  
        ├──food-6.png         # Imagem de teste 6
├── /uploaded_img/            # Pasta onde serão colocadas as imagens inseridas na base de dados pelo utilizador  
        ├──food-1.png         # Imagem de teste 1  
        ├──food-2.png         # Imagem de teste 2  
        ├──food-3.png         # Imagem de teste 3
├── /README.md                # Ficheiro que esta a ler onde tera todas as informações sobre o projeto e como pode implementar você mesmo  
├── /admin_page.php           # Ficheiro onde tera o frontend sendo o que se ve do site
├── /admin_update.php         # Ficheiro onde tera o backend sendo a parte funcional como funções
├── /config.php               # Fichiero para ligar a base de dados
├── /produtos.sql             # Ficheiro da base de dados
```
🎯 Requisitos

Servidor Web (Apache recomendado)

PHP 7 ou superior

MySQL

PHPMyAdmin (opcional para gerenciamento visual do banco de dados)

Conta em um serviço de hospedagem gratuita (ex: 000WebHost, InfinityFree)

⚙️ Configuração do Banco de Dados

Acesse o PHPMyAdmin e crie um novo banco de dados.

Execute o script SQL localizado em /database/crud.sql para criar as tabelas necessárias.

Atualize o arquivo /config/config.php com as credenciais do banco de dados:

<?php
$host = 'localhost';
$user = 'seu_usuario';
$pass = 'sua_senha';
$dbname = 'seu_banco_de_dados';
$conn = new mysqli($host, $user, $pass, $dbname);
if ($conn->connect_error) {
    die("Conexão falhou: " . $conn->connect_error);
}
?>

🚀 Hospedagem Gratuita

Caso queira hospedar o projeto gratuitamente, siga estas etapas:

Cadastre-se em 000WebHost ou InfinityFree.

Faça o upload dos arquivos do projeto via FTP ou painel de controle da hospedagem.

Crie um banco de dados MySQL e configure corretamente as credenciais no arquivo config.php.
