<h1>N8N Localmente com Docker 🐳</h1>

<p>Automatize seus fluxos de trabalho com facilidade usando o <strong>N8N</strong>, uma poderosa ferramenta de automação baseada em código low-code, executando localmente via Docker.</p>

<hr>

<h2>📦 Pré-requisitos</h2>
<ul>
  <li>Docker instalado (<a href="https://www.docker.com/get-started" target="_blank">Instalar</a>)</li>
  <li>Docker Compose instalado (<a href="https://docs.docker.com/compose/install/" target="_blank">Instalar</a>)</li>
</ul>

<hr>

<h2>⚙️ Como Executar</h2>
<ol>
  <li>Clone este repositório:</li>
  <pre><code>git clone https://github.com/vikthyr/n8n-with-docker.git</code></pre>

  <li>Acesse a pasta do projeto:</li>
  <pre><code>cd sua-pasta</code></pre>

  <li>Copie o arquivo de exemplo e renomeie:</li>
  <pre><code>cp .env-example .env</code></pre>

  <li>Altere as credenciais no arquivo <code>.env</code> conforme necessário (usuário, senha, chave de criptografia etc.).</li>

  <li>Inicie os containers com:</li>
  <pre><code>docker-compose up</code></pre>
</ol>

<h3>🌐 Acesse o N8N através da URL:</h3>
<p><strong><a href="http://localhost:5678" target="_blank">http://localhost:5678</a></strong></p>

<hr>

<h2>💾 Persistência de Dados</h2>
<p>O arquivo <code>docker-compose.yml</code> está configurado para garantir a persistência de dados, incluindo automações e credenciais.</p>

<ul>
  <li>Será criada automaticamente uma pasta chamada <strong>n8n_data</strong> na raiz do projeto.</li>
  <li>Essa pasta deve ser mantida/copiada para qualquer ambiente onde o projeto for executado, garantindo que suas automações continuem funcionando.</li>
</ul>

<hr>

<h2>🔐 Segurança</h2>
<ul>
  <li>O acesso via navegador é protegido por autenticação básica configurada no arquivo <code>.env</code>.</li>
  <li>É altamente recomendado adicionar o arquivo <code>.env</code> ao seu <code>.gitignore</code> para proteger informações sensíveis.</li>
</ul>
