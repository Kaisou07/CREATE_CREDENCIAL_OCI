# 🚀 Criando uma Credencial na OCI para Acessar um Bucket

Este guia fornece um passo a passo para criar uma credencial na **Oracle Cloud Infrastructure (OCI)** para acessar um bucket e utilizá-lo com o `DBMS_CLOUD`.

---

## 📌 Passos

### 🏗️ 1. Criar um Bucket
- Acesse sua conta na **OCI**.
- Navegue até a seção **Buckets** e **crie um novo bucket**.

### 🗄️ 2. Acessar o Autonomous Database
- Vá até seu **Autonomous Database**.
- Abra a opção **Carga de Dados**.
- Isso abrirá a página do **Database Action Developer Web**.

### 🔗 3. Criar uma Conexão para o Cloud Store
- Vá até a aba **Conexões**.
- Clique em **Criar** e selecione **Novo Local do Cloud Store**.
- No meio do formulário, clique no botão **Criar Credencial**.

### 📝 4. Preencher Informações da Credencial
- Preencha os campos necessários.
- **Copie o script gerado**.
- Clique no botão para abrir o **Cloud Shell**.

### 💻 5. Executar o Script no Cloud Shell
- Aguarde a abertura do **Cloud Shell**.
- **Cole o script copiado**.
- Substitua `admin` pelo seu **schema** no comando.
- **Execute o script**.

### ⚙️ 6. Responder às Solicitações do Terminal
- O terminal solicitará a criação de uma **Key** e **Fingerprint**.
- **Aceite todas as solicitações digitando `y`**.
- Complete o processo preenchendo as informações necessárias.
- Caso não tenha uma **wallet**, **crie uma aceitando com `y`**.
- **Insira a senha do seu schema quando solicitado**.

### ▶️ 7. Executar o Comando Gerado
- Após o processo, o shell retornará um comando `cat`.
- **Copie e execute esse comando**.
- O terminal retornará um código **PL/SQL**.
- **Copie e execute esse código dentro do seu schema no banco de dados**.

### 🔍 8. Verificar Permissões
- Caso o comando **PL/SQL** não rode corretamente, pode ser que esteja faltando a permissão necessária.
- **Entre no schema `admin` e conceda a permissão `GRANT` para `DBMS_CLOUD` ao seu schema**.

---

## 🎯 Conclusão
✅ Após seguir esses passos, sua credencial estará **configurada e pronta para uso** com `DBMS_CLOUD`. Agora você pode **carregar arquivos** no seu **bucket da Oracle, S3 ou outro serviço de armazenamento compatível**. 🚀

