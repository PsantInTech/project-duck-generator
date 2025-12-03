
## 🔹 Pré-requisitos

No Mac, você precisa ter instalado:

- [Python 3.10+](https://www.python.org/downloads/)
- [Node.js 18+ e npm](https://nodejs.org/)
- Git (geralmente já vem no Mac)
- Terminal (Terminal.app ou iTerm2)

---

## 🔹 Clonando o projeto

1. Abra o Terminal.
2. Escolha uma pasta para clonar o projeto:
```bash
cd ~/Documents
Clone o repositório:

bash
Copiar código
git clone https://github.com/SEU_USUARIO/duck-generator.git
Entre na pasta do projeto:

bash
Copiar código
cd duck-generator
🔹 Configurando o backend (Python + Flask)
Entre na pasta do backend:

bash
Copiar código
cd backend
Criar um ambiente virtual (recomendado):

bash
Copiar código
python3 -m venv venv
Ativar o ambiente virtual:

bash
Copiar código
source venv/bin/activate
Instalar as dependências:

bash
Copiar código
pip install -r requirements.txt
Se não existir requirements.txt, instale manualmente:

bash
Copiar código
pip install flask flask-cors pillow
Rodar o servidor:

bash
Copiar código
python duck_agent.py
O backend estará disponível em: http://localhost:8081

Health check: http://localhost:8081/health

🔹 Configurando o frontend (React + Vite)
Abra outro Terminal e vá para a pasta do frontend:

bash
Copiar código
cd ~/Documents/duck-generator/frontend
Instale as dependências:

bash
Copiar código
npm install
Rodar o frontend:

bash
Copiar código
npm run dev
O frontend será iniciado em algo como http://localhost:5173

Abra no navegador e teste a geração de patos.

🔹 Testando a API
Você pode testar rapidamente no Terminal usando curl:

bash
Copiar código
curl -X POST http://localhost:8081/api/duck/generate \
-H "Content-Type: application/json" \
-d '{"description": "um duck azul com óculos"}'
Ou usando o frontend e digitando a descrição com a palavra "duck".

🔹 Estrutura do projeto
css
Copiar código
duck-generator/
├─ backend/
│  ├─ duck_agent.py
│  ├─ fallback_ducks/
│  └─ venv/
├─ frontend/
│  ├─ src/
│  │  ├─ App.jsx
│  │  ├─ main.jsx
│  │  └─ styles.css
│  ├─ index.html
│  └─ package.json
└─ README.md
✅ You have a screenshot of your custom duck!

Now generate your dream duck and take it home! 🦆✨
