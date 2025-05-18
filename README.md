# Aniversariômetro Inteligente com Gemini AI 🎂✨

Bem-vindo ao Aniversariômetro Inteligente! Este projeto é um assistente pessoal para gerenciar datas de aniversário, alertar sobre os próximos e ajudar você a criar mensagens de parabéns e sugestões de presentes personalizadas utilizando o poder da Inteligência Artificial do Google Gemini (modelo Flash).

## Funcionalidades Principais 🚀

* **Cadastro Detalhado:** Registre aniversariantes com nome, data de nascimento completa, interesses, restrições (alimentares ou outras) e seu tipo de relacionamento com a pessoa.
* **Alertas Inteligentes:** Seja notificado sobre aniversários que são "hoje" ou que ocorrerão nos próximos dias.
* **Mensagens Personalizadas com IA:** Gere mensagens de parabéns criativas e adequadas ao seu relacionamento com o aniversariante, criadas pelo Gemini Flash.
* **Sugestões de Presentes com IA:** Receba ideias de presentes baseadas nos interesses e restrições da pessoa, com sugestões adaptadas pela IA para serem relevantes e atenciosas.
* **Persistência de Dados:** Todos os dados cadastrados são salvos de forma segura no Google Drive do usuário, garantindo que não se percam entre as sessões.
* **Interface Interativa:** Interaja com o programa através de um console amigável diretamente no ambiente Google Colab.

## Tecnologias Utilizadas 🛠️

* Python 3
* Google Colab (ambiente de desenvolvimento e execução)
* Google Gemini API (especificamente o modelo `gemini-1.5-flash-latest`)
* Google Drive API (para armazenamento persistente dos dados dos aniversários)
* JSON (para formato de armazenamento dos dados)

## Como Configurar e Executar no Google Colab 🧑‍💻

Siga estes passos para rodar o Aniversariômetro Inteligente:

**Pré-requisitos:**

1.  Uma conta Google.
2.  Uma API Key do Google Gemini. Você pode obter uma seguindo as instruções em [Google AI Studio](https://aistudio.google.com/app/apikey).

**Passos para Execução:**

1.  **Abrir o Notebook:**
    * Abra o arquivo `.ipynb` deste repositório diretamente no [Google Colab](https://colab.research.google.com/).

2.  **Configurar a API Key do Gemini:**
    * No ambiente do Colab, clique no ícone de **chave (Secrets)** no painel esquerdo.
    * Clique em **"+ ADD A NEW SECRET"**.
    * No campo "Name", digite exatamente: `GEMINI_API_KEY`
    * No campo "Value", cole a sua API Key que você obteve do Google AI Studio.
    * Certifique-se de que a opção **"Notebook access"** (Acesso ao notebook) está ativada para este segredo.

3.  **Executar a Célula 1 (Montagem do Drive e Configurações):**
    * Esta é a primeira célula do notebook. Execute-a clicando no botão de "Play" à esquerda dela ou pressionando `Shift + Enter`.
    * Você será solicitado(a) a **autorizar o acesso ao seu Google Drive**. Siga as instruções na tela (clicar no link, fazer login na sua conta Google, copiar o código de autorização e colá-lo no campo de entrada no Colab).
    * Após a autorização, esta célula criará uma pasta no seu "Meu Drive" (por padrão, chamada `AniversariometroApp_Dados_Final`) onde o arquivo `aniversarios_gdrive_final.json` (contendo os dados dos aniversários) será armazenado.
    * Aguarde a mensagem "🎉 Configuração do Google Drive finalizada com sucesso!" antes de prosseguir.

4.  **Executar a Célula 2 (Aplicação Principal do Aniversariômetro):**
    * Esta é a segunda célula do notebook. Execute-a **somente após a Célula 1 ter sido concluída com sucesso**.
    * O programa Aniversariômetro iniciará, e você poderá começar a cadastrar aniversariantes e receber alertas e sugestões!

## Como Usar o Programa 🤖

Após a execução da Célula 2:

1.  **Cadastro:** O programa perguntará se você deseja cadastrar um novo aniversariante. Siga as instruções, fornecendo nome, data de nascimento (no formato AAAA-MM-DD), interesses, restrições e seu relacionamento.
2.  **Verificação:** Após a etapa de cadastro, o programa verificará automaticamente os aniversários próximos (hoje e nos próximos 7 dias, por padrão).
3.  **Resultados:** Para cada aniversariante próximo, serão exibidas:
    * A data do aniversário e quantos dias faltam.
    * Uma sugestão de mensagem de parabéns gerada pela IA.
    * Ideias de presentes geradas pela IA.


**Autor:** [MARLON GABRIEL]
