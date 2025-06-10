#  Startup Finder Bot

O **Startup Finder Bot** é um projeto em Flask que utiliza o **LangChain** com **OpenAI** para analisar dados gerados aleatoriamente de fundadores de startups. O sistema cria perfis estruturados e atribui uma pontuação baseada em heurísticas simples. Ideal para testar ideias de scoring de empreendedores ou como base para sistemas de recomendação de investimentos.

---

##  Tecnologias Utilizadas

- **Flask** — Para a interface web.
- **LangChain + OpenAI** — Para análise automatizada do perfil do fundador.
- **Faker** — Para gerar dados simulados realistas.
- **Python** — Para toda a lógica backend.
- **Heurísticas personalizadas** — Para pontuação dos fundadores.

---

## ▶️ Como Rodar Localmente

```bash
1. Clone o repositório
git clone https://github.com/seuusuario/startup-finder-bot.git
cd startup-finder-bot

2. Instale as dependências

pip install -r requirements.txt
3. Configure a chave da API da OpenAI
Crie uma chave gratuita ou paga em: https://platform.openai.com/account/api-keys

Depois, defina a variável de ambiente:

Linux/MacOS


export OPENAI_API_KEY=sua-chave-aqui
Windows (cmd)


set OPENAI_API_KEY=sua-chave-aqui
Ou crie um arquivo .env com o conteúdo:


OPENAI_API_KEY=sua-chave-aqui
E use python-dotenv para carregar automaticamente se desejar.

4. Rode o projeto

python app.py
Abra seu navegador e acesse: http://localhost:5000

💡 Como Funciona
A cada acesso:

5 fundadores são gerados aleatoriamente com nome, idade, experiência, formação e visão.

O LangChain faz uma análise textual com base nos dados simulados.

Uma heurística pontua o potencial do fundador (máximo 100).

Os resultados são exibidos com pontuação e análise da IA.

🛠️ Personalizações Possíveis
Adicionar mais heurísticas com base em networking, capital inicial ou tração.

Persistir os dados em um banco de dados.

Integrar com APIs externas como Crunchbase.

Alterar para Streamlit se desejar interface mais visual.

📄 Licença
Este projeto está licenciado sob a licença MIT.

Desenvolvido por Vitor Santos 🚀 - vkcs.dev

