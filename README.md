# 🧠 Práxis Mediadora AI

Um motor histórico-cultural de intervenção pedagógica focado em transformar o planejamento de aulas de professores da escola pública. A aplicação une a **Teoria da Modificabilidade Cognitiva Estrutural** de Reuven Feuerstein e o conceito de **Zona de Desenvolvimento Proximal (ZDP)** de Lev Vigotski para gerar "andaimes" educacionais cirúrgicos e de alto nível.

---

## 🎯 Objetivo do Projeto

A ferramenta foi criada para combater o determinismo biológico e o "facilitacionismo" pedagógico, que frequentemente se manifesta em Planos Educacionais Individualizados (PEIs) genéricos e burocráticos. 

O aplicativo permite que o professor mapeie o contexto material e a **falha cognitiva estrutural** do estudante (ex: impulsividade na entrada de dados, dificuldade de comparar na elaboração ou bloqueio na saída). A IA então atua como um mediador, gerando um planejamento em três partes rigorosas:
1. **Plano de Aula Oficial:** Um roteiro literal (script de fala) de como o professor deve intervir para "bloquear" o erro cognitivo.
2. **Andaime Textual do Aluno:** O material/atividade estruturado com paradas de pensamento para ser entregue ao aluno.
3. **Relatório de Avaliação Dinâmica:** Uma rubrica rápida para provar à gestão escolar o avanço cognitivo real do estudante, focado no processo intelectual e não apenas na socialização.

## 🛠️ Tech Stack & Arquitetura

O projeto foi construído seguindo a filosofia *Vibe Coding*, focado em estética premium (Glassmorphism, Dark Mode dinâmico), velocidade e execução zero-config.

- **Frontend Core:** HTML5, JavaScript (Vanilla), TailwindCSS v3 (via CDN).
- **Tipografia & Ícones:** Google Fonts (Inter) e FontAwesome 6.
- **Integração de IA:** Google Gemini API (`generativelanguage.googleapis.com`) via `fetch` direto do client.
- **Recursos Nativos Avançados:** 
  - **Web Speech API:** Reconhecimento de voz para o professor "ditar" o contexto da turma (Desabafo em Áudio).
- **Bibliotecas Auxiliares:**
  - `html2pdf.js`: Para exportar a tela diretamente para um documento PDF A4 formatado.
  - `marked.js`: Para renderizar a sintaxe Markdown retornada pelas IAs.

## 🚀 Setup e Instruções de Uso

Esta é uma aplicação "Single File", o que significa que não há processos de build de Node.js complicados. Ela roda 100% no seu navegador.

1. **Clonar ou Baixar:**
   Baixe o arquivo `pr_xis_mediadora_ai.html` para sua máquina.
2. **Executar:**
   Basta dar um duplo clique no arquivo `pr_xis_mediadora_ai.html` para abri-lo no Google Chrome, Firefox ou Edge.
3. **Fluxo de Uso:**
   - Preencha o formulário à esquerda, usando o microfone se desejar ditar o texto.
   - Você tem duas opções de processamento:
     - **Motor IA Avançado (API Key):** Insira sua chave gratuita do Google AI Studio no menu esquerdo e clique em "Gerar Roteiro Aqui" para o resultado aparecer diretamente na tela.
     - **Modo Gratuito (Copiar/Colar):** Clique em "Gerar Super Prompt para Copiar" e cole o texto formatado no ChatGPT, Claude ou Gemini.
4. **Exportar:**
   Uma vez gerado na tela, clique no botão roxo "Exportar PDF Oficial" no topo superior direito para baixar o arquivo pronto para impressão ou WhatsApp.

## 🔗 Deployment URL

*(Pendente. Sugestão de hospedagem estática: Cloudflare Pages, Surge.sh, Netlify ou Vercel)*

## 📜 Histórico de Modificações (Changelog)

- **v1.1.0** (Atual):
  - **Reconhecimento de Voz:** Implementação do ícone de microfone (Web Speech API) no campo "Realidade Material do Aluno".
  - **Prompt 3 em 1:** Expansão da engenharia de prompt para forçar a IA a devolver o Script, o Andaime Textual e o Relatório de Avaliação Dinâmica.
  - **PDF Export:** Integração com a lib `html2pdf.js` para download oficial do relatório gerado.
  - **UI/UX Refatorada (Toasts):** Fim dos `alerts()` nativos do navegador, substituídos por um sistema elegante de notificações Toast deslizantes (Tailwind).
  - **Dicas Visuais na ZDP:** Exemplos explícitos integrados sob as perguntas do "Ponto de Partida" e "Linha de Chegada", facilitando o entendimento do professor de forma permanente.
  - **Comparativo PEI:** Adição de sessão teórica extensa explicando como a Práxis Mediadora não substitui o PEI juridicamente, mas preenche o vazio metodológico de "como" aplicá-lo em sala.
- **v1.0.0**: 
  - Lançamento inicial da estrutura Vygotsky/Feuerstein e conexão com Gemini API.
