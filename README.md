# Template Base - Node.js + Express

Estrutura inicial padrão para projetos Back-end utilizando ES Modules (`import/export`).

## Como usar este template

1. **Instale as dependências** (obrigatório ao clonar o projeto em outra máquina):
   ```bash
   npm install
   ```
   > **Por que isso é necessário?** A pasta `node_modules` é ignorada pelo `.gitignore` para não pesar o repositório no GitHub. Ao rodar `npm install`, o gerenciador de pacotes lê o arquivo `package.json` e baixa todas as bibliotecas necessárias automaticamente.

2. **Configure as variáveis de ambiente**:
   - Copie o arquivo `.env.example`, renomeie a cópia para `.env` e preencha com os valores reais do seu ambiente (como a porta do servidor ou senhas).

3. **Inicie o servidor**:
   - **Modo desenvolvimento** (reinicia sozinho ao salvar alterações):
     ```bash
     npm run dev
     ```
   - **Modo produção**:
     ```bash
     npm start
     ```

## Estrutura de Pastas

- **`public/`**: Arquivos estáticos acessíveis pelo navegador (HTML, CSS, imagens).
- **`src/config/`**: Configurações externas (conexão com banco de dados, variáveis).
- **`src/controllers/`**: Lógica principal e regras de negócio de cada rota.
- **`src/middlewares/`**: Funções intermediárias (validação de dados, autenticação).
- **`src/routes/`**: Definição dos endereços (endpoints) da API.
- **`src/app.js`**: Configuração central do Express.
- **`src/server.js`**: Inicialização do servidor.
