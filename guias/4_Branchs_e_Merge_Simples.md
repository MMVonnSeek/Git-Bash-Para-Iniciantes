# 4. Trabalhando com Branches e Mesclagem Simples

Trabalhar com **branches** (ramificações) é o que torna o Git tão poderoso. Ele permite que você e sua equipe trabalhem em diferentes funcionalidades ao mesmo tempo, sem interferir no código principal.

## 1. O Conceito de Branch

Pense no `main` (ou `master`) como a linha do tempo principal do seu projeto. Uma *branch* é uma cópia dessa linha do tempo onde você pode fazer experimentos e desenvolver novas funcionalidades.

## 2. Comandos Essenciais de Branch

| Comando | Função | Exemplo de Uso |
| :--- | :--- | :--- |
| `git branch` | Lista todas as branches locais. A branch atual é marcada com um asterisco (`*`). | `git branch` |
| `git branch [nome]` | Cria uma nova branch. | `git branch nova-feature` |
| `git checkout [nome]` | Alterna para a branch especificada. | `git checkout nova-feature` |
| `git checkout -b [nome]` | Cria e alterna para a nova branch em um único comando. | `git checkout -b nova-feature` |

## 3. O Fluxo de Trabalho com Branches

1.  **Crie uma nova branch** para a sua tarefa:
    ```bash
    git checkout -b minha-tarefa
    ```
2.  **Trabalhe e Comite** normalmente na sua nova branch:
    ```bash
    # Faça suas alterações nos arquivos
    git add .
    git commit -m "feat: Implementa a nova funcionalidade X"
    ```
3.  **Envie a branch para o GitHub:**
    ```bash
    git push origin minha-tarefa
    ```

## 4. Mesclagem (Merge)

Quando sua funcionalidade estiver pronta e testada, você precisa mesclá-la de volta na branch principal (`main`).

1.  **Volte para a branch principal:**
    ```bash
    git checkout main
    ```
2.  **Puxe as últimas alterações** da branch principal do GitHub (para evitar conflitos):
    ```bash
    git pull origin main
    ```
3.  **Mescle sua branch de funcionalidade:**
    ```bash
    git merge minha-tarefa
    ```
    *   Se não houver conflitos, o Git fará a mesclagem automaticamente.
    *   Se houver conflitos, consulte o **Guia 3** para a seção de resolução de conflitos.

4.  **Envie a mesclagem para o GitHub:**
    ```bash
    git push origin main
    ```

## 5. Limpeza

Após a mesclagem, você pode excluir a branch local e remota (se não for mais necessária):

```bash
# Excluir branch local
git branch -d minha-tarefa

# Excluir branch remota
git push origin --delete minha-tarefa
```