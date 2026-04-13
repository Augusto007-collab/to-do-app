# 🌌 TaskMaster Ultra: Workspace Inteligente

O **TaskMaster Ultra** é uma estação de trabalho completa para produtividade, projetada para oferecer uma experiência imersiva de gestão de tarefas. Combinando estética *Glassmorphism* com funcionalidades de monitoramento em tempo real, esta aplicação vai além de uma simples lista, transformando-se em um dashboard de foco pessoal.

---

## 💎 Funcionalidades de Elite

* **Identificação de Acesso:** Camada de transição inicial (Login) que personaliza o ambiente com o nome do usuário.
* **Gestão de Deadlines:** Campo de data e hora (`datetime-local`) para definir prazos precisos, permitindo o gerenciamento de urgências.
* **Monitoramento de Sessão:** Cronômetro dinâmico que contabiliza o tempo de permanência no site, auxiliando no controle de foco.
* **Dashboard de Status:** Relógio e calendário em tempo real integrados ao rodapé da aplicação.
* **Feedback Multissensorial:** * **Visual:** Animações de entrada (`slideUp`) e transições suaves de opacidade.
    * **Auditivo:** Web Audio API para disparar bipes sintetizados em ações de sucesso, erro ou exclusão.
* **Design Glassmorphism:** Interface baseada em transparências, desfoque de fundo (blur) e bordas finas, otimizada para o "Modo Escuro".

---

## 🛠️ Arquitetura Técnica

O projeto foi construído utilizando tecnologias puras (Vanilla), sem dependência de bibliotecas pesadas, garantindo carregamento instantâneo.

### 1. Estrutura e Estilo (HTML5 & CSS3)
- **Flexbox/Grid:** Utilizados para manter a interface responsiva em qualquer dispositivo.
- **Glassmorphism:** Implementado através da propriedade `backdrop-filter: blur()`.
- **Animações `@keyframes`:** Controlam o surgimento fluido dos elementos e a saída animada de tarefas removidas.

### 2. Lógica de Negócio (JavaScript)
- **Session Management:** O cronômetro de sessão utiliza lógica de incremento em segundos com formatação `MM:SS`.
- **DOM Dinâmico:** As tarefas são injetadas no topo da lista (`prepend`) para priorizar as inserções mais recentes.
- **Áudio Sintetizado:** Uso da `AudioContext` para criar frequências sonoras via código, eliminando a necessidade de carregar arquivos de áudio externos.

---

## ⚙️ Como Utilizar

1.  Salve o código fonte em um arquivo chamado `index.html`.
2.  Abra o arquivo em qualquer navegador moderno.
3.  **Acesso:** Digite seu nome na tela inicial para desbloquear o workspace.
4.  **Criação:** Descreva a tarefa, selecione a prioridade e, se necessário, defina um prazo no calendário.
5.  **Interação:** * Clique no ícone de **Check** para concluir (a tarefa ficará translúcida).
    * Clique no ícone de **Lixeira** para remover com efeito de deslize.

---

## 📝 Notas do Desenvolvedor

Esta versão foi desenvolvida com foco em **UX (User Experience)**. A inclusão da data/hora e do tempo de sessão visa criar um senso de presença e urgência, enquanto a tela de identificação inicial estabelece um compromisso psicológico do usuário com suas atividades.

**Versão:** 3.0 Ultra (Current)  
**Status:** Produção / Estável
