# 2i-crud

# Introdução  

Este projeto é um sistema CRUD (Create, Read, Update, Delete) desenvolvido em PHP e MySQL, utilizando PHPMyAdmin para gerenciar o banco de dados.  

# Funcionalidades  

Criar registros no banco de dados  
Listar registros cadastrados  
Editar registros existentes  
Excluir registros  

# Tecnologias Utilizadas
PHP  
MySQL  
PHPMyAdmin  
HTML/CSS  

# Estrutura do Projeto  
/  
|-- /config  # Arquivo de configuração do banco de dados  
|-- /database # Scripts SQL para criação do banco de dados  
|-- /public   # Arquivos públicos como CSS, JS, imagens  
|-- /src      # Código principal do CRUD  
|-- index.php # Página principal do sistema  
|-- README.md # Documentação do projeto  

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
