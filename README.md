# Banco-De-Dados-Azure

# 🧱 Configuração de uma Instância de Banco de Dados no Azure (Azure SQL Database)
🛠️ Plataforma Usada: Portal do Azure
📌 Serviço Exemplo: Azure SQL Database (modelo PaaS)
🔹 1. Acesse o Portal do Azure
Vá para: https://portal.azure.com

Faça login com sua conta Microsoft/Azure.

## 🔹 2. Criar o Banco de Dados
No menu lateral ou na barra de pesquisa, digite e selecione: "SQL Database"

Clique em “+ Criar”.

## 🔹 3. Aba “Básico” - Configuração Inicial

### Campo                   |	O que preencher
### Assinatura	            |Selecione a sua assinatura
### Grupo de Recursos       |Escolha um existente ou crie um novo
### Nome do banco de dados	|Ex: meuBancoTeste
### Servidor	              |Crie um novo servidor (será sua instância de banco de dados)
### Localização (Região)	  |Escolha a mais próxima do seu cliente/usuário

## 🔹 4. Criar um Servidor SQL
Clique em “Criar novo” e preencha:


### Campo                       |	O que preencher
### Nome do servidor	          |Ex: meuservidor-sql
### Localização	                |Mesma do banco
### Login do administrador	    |Ex: adminsql
### Senha	                      |Defina uma senha forte
### Confirmar senha	            |Redigite a senha

## 🔹 5. Aba “Configuração do Preço”
Selecione o plano conforme o seu uso:

DTU-based (básico, padrão, premium) – Ideal para quem quer simplicidade.

vCore-based – Maior controle sobre CPU e memória.

Para testes, escolha a opção mais barata: Basic ou Standard (S0).

## 🔹 6. Aba “Rede”
Conectividade: Permitir acesso público ou privado (VPN/VNet).

Regras de firewall:

Habilite o acesso ao IP atual do seu computador para conectar.

Você pode configurar isso depois também.

## 🔹 7. Aba “Segurança” (Opcional)
Habilitar Autenticação do Azure AD (opcional).

Ativar Backup geo-redundante, Auditoria e Transparência de dados (conforme necessidade).

## 🔹 8. Revisar e Criar
Clique em "Revisar + Criar".

Após validar as configurações, clique em "Criar".

Aguarde alguns minutos enquanto o recurso é provisionado.

## 🔹 9. Conectar ao Banco de Dados
Após a criação:

Vá até o banco na página inicial do portal.

Clique em "Mostrar cadeia de conexão" (connection string).

Copie a string e configure em sua aplicação ou use um software como:

Azure Data Studio

SQL Server Management Studio (SSMS)

#  ✅ Resumo Final

Etapa	Descrição
1. Criar SQL Database	Nome + grupo de recurso
2. Criar Servidor	Nome + login/senha + região
3. Escolher preço	Plano básico para testes
4. Configurar acesso	IP público, regras de firewall
5. Finalizar e conectar	Usar SSMS ou app web
