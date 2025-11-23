# 1. Instalação e Configuração Inicial

## 1. O que é o Git Bash?

O **Git Bash** é um aplicativo para sistemas operacionais Windows que fornece uma experiência de linha de comando (terminal) que emula o ambiente Bash do Linux. Ele é a forma mais comum de usar o Git via linha de comando no Windows.

## 2. Instalação (Windows)

1.  **Download:** Acesse o site oficial do Git e baixe o instalador para Windows: [https://git-scm.com/downloads](https://git-scm.com/downloads).
2.  **Execução:** Execute o arquivo baixado.
3.  **Configurações Padrão:** Para iniciantes, é recomendado manter as configurações padrão durante a instalação. Certifique-se de que a opção **"Use Git from the Windows Command Prompt"** ou similar esteja marcada.
4.  **Finalização:** Após a instalação, você pode abrir o Git Bash clicando com o botão direito em qualquer pasta e selecionando **"Git Bash Here"**.

## 3. Configuração da Sua Identidade

Antes de começar a fazer *commits*, você precisa dizer ao Git quem você é. Isso é crucial para que seus *commits* sejam rastreados corretamente no GitHub.

Execute os seguintes comandos no Git Bash, substituindo as informações entre aspas pelos seus dados:

### 3.1. Configurar Nome de Usuário

```bash
git config --global user.name "Seu Nome Completo"
```

### 3.2. Configurar Email

Use o mesmo endereço de e-mail que você usa na sua conta do GitHub.

```bash
git config --global user.email "seu.email@exemplo.com"
```

### 3.3. Verificar a Configuração

Para ter certeza de que tudo foi configurado corretamente, use:

```bash
git config --list
```

Você deve ver seu `user.name` e `user.email` na lista.

## 4. Próximo Passo

Com o Git Bash instalado e configurado, você está pronto para aprender a navegar no terminal. Vá para o **Guia 2: Comandos Básicos do Terminal (Bash)**.
