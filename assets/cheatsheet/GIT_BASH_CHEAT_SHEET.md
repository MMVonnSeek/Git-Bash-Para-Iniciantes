# Git Bash Cheat Sheet: Comandos Essenciais

Mantenha esta "cola" aberta para referência rápida enquanto você pratica no Git Bash!

## 1. Comandos Básicos do Terminal (Bash)

| Comando | Descrição | Exemplo |
| :--- | :--- | :--- |
| `pwd` | Mostra o diretório atual. | `pwd` |
| `ls` | Lista o conteúdo do diretório. | `ls -l` |
| `cd [pasta]` | Navega para a pasta. | `cd meu-projeto` |
| `cd ..` | Sobe um nível. | `cd ..` |
| `mkdir [nome]` | Cria uma nova pasta. | `mkdir nova-pasta` |
| `touch [arquivo]` | Cria um novo arquivo vazio. | `touch index.html` |
| `clear` | Limpa a tela do terminal. | `clear` |

## 2. Configuração Inicial

| Comando | Descrição | Exemplo |
| :--- | :--- | :--- |
| `git config --global user.name` | Define seu nome de usuário globalmente. | `git config --global user.name "Seu Nome"` |
| `git config --global user.email` | Define seu e-mail globalmente. | `git config --global user.email "seu@email.com"` |
| `git config --list` | Exibe todas as configurações. | `git config --list` |

## 3. Fluxo de Trabalho Principal

| Comando | Descrição | Exemplo |
| :--- | :--- | :--- |
| `git init` | Inicializa um novo repositório Git local. | `git init` |
| `git clone [url]` | Baixa um repositório remoto. | `git clone https://...` |
| `git status` | Mostra o estado dos arquivos (modificados, staged). | `git status` |
| `git add [arquivo]` | Adiciona um arquivo à Staging Area. | `git add index.html` |
| `git add .` | Adiciona todos os arquivos modificados à Staging Area. | `git add .` |
| `git commit -m "[msg]"` | Salva as alterações no repositório local. | `git commit -m "feat: Adiciona botão"` |
| `git push origin [branch]` | Envia commits locais para o repositório remoto. | `git push origin main` |
| `git pull origin [branch]` | Baixa e mescla alterações do repositório remoto. | `git pull origin main` |

## 4. Histórico e Desfazer

| Comando | Descrição | Exemplo |
| :--- | :--- | :--- |
| `git log` | Exibe o histórico de commits. | `git log --oneline` |
| `git reset [arquivo]` | Remove um arquivo da Staging Area (mantém as alterações). | `git reset index.html` |
| `git checkout -- [arquivo]` | Descarta as alterações locais não comitadas em um arquivo. | `git checkout -- index.html` |

## 5. Branches

| Comando | Descrição | Exemplo |
| :--- | :--- | :--- |
| `git branch` | Lista as branches. | `git branch` |
| `git branch [nome]` | Cria uma nova branch. | `git branch nova-feature` |
| `git checkout [nome]` | Alterna para a branch. | `git checkout nova-feature` |
| `git checkout -b [nome]` | Cria e alterna (atalho). | `git checkout -b nova-feature` |
| `git merge [branch]` | Mescla a branch especificada na branch atual. | `git merge nova-feature` |
| `git branch -d [nome]` | Exclui a branch local (após mesclagem). | `git branch -d nova-feature` |
