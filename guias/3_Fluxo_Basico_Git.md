# 3. O Fluxo de Trabalho Básico do Git

Este guia cobre o ciclo de vida de um projeto Git, desde a criação até o envio para o GitHub.

## 1. Iniciando um Repositório

### Cenário A: Criar um novo projeto localmente

1.  **Crie a pasta do projeto e entre nela:**
    ```bash
    mkdir meu-novo-projeto
    cd meu-novo-projeto
    ```
2.  **Inicialize o Git:**
    ```bash
    git init
    ```
    *Resultado: Cria a pasta oculta `.git`, transformando a pasta em um repositório Git.*

### Cenário B: Baixar um projeto do GitHub

1.  **Clone o repositório:** Use o link HTTPS do GitHub.
    ```bash
    git clone [URL do Repositório]
    ```
    *Resultado: Baixa o projeto e já o inicializa como um repositório Git.*

## 2. O Ciclo de Commit (Adicionar e Salvar)

O Git trabalha com três áreas: **Diretório de Trabalho**, **Staging Area** e **Repositório Local**.

### 2.1. Adicionar Arquivos (`git add`)

Após criar ou modificar arquivos, você precisa adicioná-los à **Staging Area** (área de preparação).

```bash
# Adiciona um arquivo específico
git add nome-do-arquivo.html

# Adiciona todos os arquivos modificados/novos
git add .
```

### 2.2. Salvar as Alterações (`git commit`)

O *commit* salva as alterações da Staging Area no seu **Repositório Local**.

```bash
git commit -m "Mensagem clara sobre o que foi alterado"
```
*   **Dica:** Use mensagens de *commit* claras e concisas. Ex: `feat: Adiciona funcionalidade de login` ou `fix: Corrige erro de cálculo no carrinho`.

### 2.3. Verificar o Status (`git status`)

Use este comando frequentemente para ver quais arquivos foram modificados, quais estão na Staging Area e se há algo para enviar.

```bash
git status
```

## 3. Sincronizando com o GitHub (Remoto)

### 3.1. Enviar para o GitHub (`git push`)

Após o *commit*, você envia suas alterações para o repositório remoto (GitHub).

```bash
git push origin main
# 'origin' é o nome padrão do seu repositório remoto.
# 'main' é o nome do seu branch principal.
```

### 3.2. Baixar do GitHub (`git pull`)

Se outra pessoa (ou você mesmo em outro computador) fez alterações no GitHub, use o `pull` para baixá-las.

```bash
git pull origin main
```

## 4. Próximo Passo

Você dominou o fluxo básico! Agora, vamos aprender a trabalhar com branches, que é essencial para o trabalho em equipe. Vá para o **Guia 4: Trabalhando com Branches e Mesclagem**.
