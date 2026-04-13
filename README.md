# 📝 TaskMaster - Organizador de Tarefas Diárias

O **TaskMaster** é uma aplicação de lista de tarefas (To-Do List) de alta performance, desenvolvida com foco em simplicidade, eficiência e clareza visual. O objetivo principal é automatizar o fluxo de organização pessoal através de uma interface intuitiva e responsiva.

---

## 🚀 Funcionalidades Principais

* **Entrada Inteligente:** Campo de descrição otimizado para inserção rápida de tarefas.
* **Gestão de Prioridades:** Sistema de classificação por urgência (Alta, Média, Baixa) com feedback visual imediato.
* **Estilização Condicional:** Diferenciação cromática das tarefas baseada no nível de prioridade para facilitar o escaneamento visual.
* **Interatividade Dinâmica:** * Marcação de conclusão com efeito visual de "tachado".
    * Exclusão instantânea de itens.
    * Suporte a atalhos de teclado (Tecla Enter para adicionar).
* **Design Responsivo:** Adaptável a diferentes tamanhos de tela (Desktop e Mobile).

---

## 🛠️ Tecnologias Utilizadas

Para garantir leveza e compatibilidade total sem dependências externas, o projeto utiliza a "Trindade da Web":

1.  **HTML5:** Estruturação semântica e acessível.
2.  **CSS3:** Estilização moderna utilizando variáveis (Custom Properties) e animações de transição.
3.  **JavaScript (Vanilla):** Lógica funcional pura para manipulação eficiente do DOM (Document Object Model).

---

## 📋 Como Executar o Projeto

Como o sistema foi construído sem a necessidade de compiladores ou frameworks pesados, a execução é extremamente simples:

1.  Faça o download ou copie o código do arquivo `index.html`.
2.  Certifique-se de que o código CSS e JS estão integrados ou referenciados corretamente.
3.  Abra o arquivo em qualquer navegador web moderno (Chrome, Firefox, Edge, Safari).

---

## 🧠 Arquitetura do Código (Detalhamento Técnico)

O desenvolvimento seguiu padrões de "Clean Code" (Código Limpo) para facilitar a manutenção:

### 1. Estilização por Prioridades (CSS)
Utilizamos seletores de classe específicos que alteram a propriedade `border-left-color`. Isso permite que o usuário identifique o que é crítico sem precisar ler textos adicionais, economizando carga cognitiva.

### 2. Manipulação do DOM (JavaScript)
A função principal `addTask()` executa os seguintes passos:
- **Validação:** Impede a criação de tarefas vazias.
- **Criação de Elementos:** Utiliza `createElement` em vez de `innerHTML` direto por questões de segurança e performance.
- **Escopo de Eventos:** Os ouvintes de eventos (click) são anexados diretamente aos botões de cada tarefa no momento da criação, garantindo que a ação de excluir ou concluir seja executada exatamente no objeto correto.

### 3. Experiência do Usuário (UX)
- **Animação fadeIn:** Novas tarefas surgem suavemente para indicar sucesso na ação.
- **Foco Automático:** Após adicionar uma tarefa, o cursor retorna automaticamente para o campo de texto, permitindo um fluxo de trabalho contínuo.

---

## ✒️ Autor
Desenvolvido por um especialista em Engenharia de Software como uma solução robusta e elegante para produtividade pessoal.# to-do-app
