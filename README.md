# 🤖 PAI AI Coder - Assistente Especializado em Python

Uma aplicação web interativa desenvolvida para auxiliar estudantes e desenvolvedores no aprendizado de Python, utilizando um Large Language Model (LLM) via API da Groq.

## 🚀 Sobre o Projeto
O **PAI AI Coder** não é um chatbot genérico. Ele foi projetado com **Engenharia de Prompt (Prompt Engineering)** avançada para atuar como um tutor técnico rigoroso. O modelo é instruído a seguir uma estrutura pedagógica fixa em todas as respostas: *Conceito → Código Comentado → Análise Detalhada → Documentação Oficial*. 

Este projeto foi desenvolvido como parte da minha transição profissional para Inteligência Artificial e Desenvolvimento de Software, aplicando meus 25+ anos de experiência em infraestrutura, lógica e educação técnica.

## ✨ Destaques Técnicos (Foco em AI Training)
- **System Prompting Estruturado:** Controle rigoroso do comportamento do LLM, evitando alucinações e garantindo que o foco permaneça estritamente em programação.
- **Prontidão para RLHF:** A saída padronizada facilita a avaliação humana da qualidade da resposta, simulando fluxos de trabalho reais de treinamento de IA.
- **Gerenciamento de Estado:** Uso de `st.session_state` para manter o contexto da conversa de forma fluida.
- **Tratamento de Erros Robusto:** Blocos `try/except` para falhas de API, garantindo que a aplicação não quebre e oriente o usuário corretamente.
- **Segurança:** A chave de API é inserida dinamicamente via interface ou variáveis de ambiente (`.env`), nunca hardcoded no repositório.

## 🛠️ Stack Tecnológica
- **Linguagem:** Python 3.13
- **Framework Web:** Streamlit
- **Inferência de LLM:** Groq API (Modelo de alta velocidade e baixa latência)
- **Gerenciamento de Ambiente:** Micromamba

---

## ⚙️ Instalação e Uso Local

Siga os passos abaixo para rodar o projeto em sua máquina. Recomenda-se o uso do `micromamba` para um ambiente leve e isolado.

**1. Navegue até a pasta do projeto:**
```bash
cd ~/Pai_Explica/pai_ai_coder
```

**2. Crie e ative o ambiente virtual:**
```bash
micromamba create --name paiec1 python=3.13 -y
micromamba activate paiec1
```

**3. Instale as dependências:**
```bash
pip install -r requirements.txt
```

**4. Execute a aplicação:**
```bash
streamlit run pai.py
```
*(Nota: Insira sua chave de API da Groq no campo dedicado na barra lateral ao abrir o app, ou configure um arquivo `.env` localmente).*

---

## 💬 Exemplo Real de Interação

Veja como o **PAI AI Coder** responde a uma pergunta, seguindo rigorosamente as diretrizes de formatação definidas no *System Prompt*:

> **Usuário:** "O que são variáveis booleanas em Python?"
> 
> **PAI AI Coder:**
> **Explicação Clara**  
> Variáveis booleanas são variáveis que armazenam apenas dois valores possíveis: True (verdadeiro) ou False (falso). Elas são usadas para representar condições lógicas, controlar fluxos de decisão (if, while, etc.) e armazenar resultados de comparações. Em Python, os valores booleanos são objetos da classe `bool`, subclasse de `int`.
> 
> **Exemplo de Código**  
> ```python
> # Exemplo: resultado de comparações
> idade = 20
> maior_de_idade = idade >= 18   # True, porque 20 >= 18
> 
> # Exemplo: operações lógicas
> pode_viajar = possui_carteira and possui_passaporte
> ```
> 
> **Detalhes do Código**  
> - O operador `>=` compara a idade com 18, retornando um booleano.  
> - O operador `and` retorna True somente se ambas as expressões forem True.  
> 
> **📚 Documentação de Referência**  
> - [Booleans e operadores lógicos](https://docs.python.org/3/library/stdtypes.html#boolean-values)  
> - [Estruturas de controle (if)](https://docs.python.org/3/tutorial/controlflow.html#if-statements)

---

## 👨‍💻 Autor
**Rafael Halav**  
Technology Professional | Telecommunications | IT | Python | AI | Data  
🔗 [LinkedIn](https://www.linkedin.com/in/rafael-halav) | ✉️ [Contato](mailto:rafael.halav.tech@gmail.com)

*Desenvolvido com foco em aprendizado contínuo e aplicação prática de Inteligência Artificial.*
```
