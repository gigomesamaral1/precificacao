# 🛍️ Plataforma de Precificação Inteligente

🚀 **Projeto de TCC: Desenvolvimento de uma Plataforma Web para Precificação Inteligente no Setor Varejista**

## 📌 Sobre o Projeto
Este projeto visa automatizar o monitoramento de preços da concorrência utilizando **n8n para Web Scraping, automação de processos e backend**, **AWS para infraestrutura** e **Machine Learning (SageMaker)** para sugerir ajustes dinâmicos de preços. A plataforma auxilia pequenos e médios varejistas a manterem preços competitivos de forma eficiente.

---

## 🏗️ Arquitetura do Sistema

| **Camada**       | **Tecnologia Utilizada**         | **Responsabilidade** |
|-----------------|--------------------------------|----------------------|
| **Frontend**    | React.js (AWS Amplify)         | Interface gráfica para os lojistas |
| **Backend**     | n8n (Self-hosted ou Cloud)     | Processamento dos dados e aplicação de regras de precificação |
| **Banco de Dados** | Amazon RDS (PostgreSQL)    | Armazena preços coletados e históricos |
| **Web Scraping** | n8n (com Puppeteer/HTTP Request) | Captura os preços da concorrência automaticamente |
| **Machine Learning** | Amazon SageMaker          | Analisa padrões e sugere ajustes de preços |
| **Automação**   | n8n                            | Orquestra Web Scraping, integração de dados e notificações |
| **API Gateway** | AWS API Gateway               | Comunicação segura entre frontend e backend |

---

## ⚙️ Tecnologias Utilizadas
- **n8n** para Web Scraping, Backend e automação de processos 🔄
- **React.js** para o frontend 🎨
- **AWS (Amplify, RDS, API Gateway, SageMaker, Lambda)** ☁️
- **PostgreSQL** como banco de dados 📊
- **Docker** para containerização 🐳
- **Puppeteer** para extração de dados de sites 🕵️‍♂️
- **Axios** para consumo de APIs 🔗

---

## 🛠️ Como Rodar o Projeto

### 📌 1️⃣ Configurar e Rodar o Backend no n8n
```sh
# Instalar o n8n
tnpm install -g n8n

# Iniciar o n8n
n8n start

# Acesse o painel de automação
http://localhost:5678
```
⚠️ **Certifique-se de configurar os fluxos de backend, scraping e integração com o banco no n8n!**

---

### 📌 2️⃣ Rodar o Frontend (React.js)
```sh
cd frontend
npm install
npm start
```
O frontend estará disponível em: **http://localhost:3000**

---

## 📊 Fluxo de Funcionamento

1️⃣ **Web Scraping com n8n** → Coleta preços automaticamente e envia para o RDS 📊  
2️⃣ **n8n Processa os Dados** → Armazena, analisa e disponibiliza via API ⚡  
3️⃣ **Machine Learning (SageMaker)** → Sugere ajustes dinâmicos nos preços 🔍  
4️⃣ **n8n Notifica Lojistas** → Alerta sobre variações de preço 📩  
5️⃣ **Frontend Exibe os Dados** → Dashboard interativo no React.js 🎨  

---

## 📈 Próximos Passos
✅ Finalizar integração do backend com o n8n  
✅ Implementar ajustes automáticos de preços via API  
✅ Melhorar visualização dos dados no frontend  

---

## 📄 Licença
Este projeto é de código aberto e está licenciado sob a **MIT License**.

📢 **Dúvidas ou Sugestões?** Abra uma issue ou contribua com o projeto! 🚀
