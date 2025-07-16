# 📋 Padrões de Commits e Branches

## 🎯 Objetivo do Projeto

Este repositório tem como objetivo fornecer um guia completo e prático para padronização de commits e branches em projetos de desenvolvimento de software. O projeto visa:

- **Padronizar** mensagens de commit de forma consistente e legível
- **Facilitar** a navegação no histórico de mudanças
- **Melhorar** a colaboração entre desenvolvedores
- **Automatizar** processos de release e changelog
- **Aumentar** a qualidade e rastreabilidade do código

## 📖 Sobre este Guia

Este documento serve como guia de referência para manter a consistência nos commits e branches do projeto, seguindo as melhores práticas da comunidade de desenvolvimento.

## 🌿 Padrões de Branches

### Estrutura de Naming

#### Branch Principal
- **`main`** - Branch de produção, sempre estável

#### Branches de Desenvolvimento
- **`develop`** - Branch de desenvolvimento principal
- **`feature/[nome-da-feature]`** - Para novas funcionalidades
- **`bugfix/[nome-do-bug]`** - Para correções de bugs
- **`hotfix/[nome-do-hotfix]`** - Para correções urgentes em produção
- **`release/[versao]`** - Para preparação de releases

#### Exemplos de Nomes de Branches
```
feature/user-authentication
feature/payment-integration
bugfix/login-validation-error
hotfix/security-patch
release/v1.2.0
```

### Fluxo de Trabalho

1. **Criar branch** a partir de `develop`
2. **Desenvolver** a funcionalidade
3. **Commit** seguindo os padrões
4. **Push** para o repositório remoto
5. **Pull Request** para `develop`
6. **Code Review** e merge

## 📝 Padrões de Commits

### Formato do Commit

```
<tipo>(<escopo>): <descrição>

<corpo do commit (opcional)>

<rodapé (opcional)>
```

### Tipos de Commit

| Tipo | Descrição |
|------|-----------|
| `feat` | Nova funcionalidade |
| `fix` | Correção de bug |
| `docs` | Documentação |
| `style` | Formatação, ponto e vírgula, etc (sem mudança de código) |
| `refactor` | Refatoração de código |
| `test` | Adição ou correção de testes |
| `chore` | Tarefas de manutenção (build, dependências, etc) |
| `perf` | Melhoria de performance |
| `ci` | Mudanças na integração contínua |
| `build` | Mudanças no sistema de build |
| `revert` | Reversão de commit anterior |

### Regras para Commits

#### Cabeçalho (Header)
- **Máximo 50 caracteres**
- **Presente do imperativo** (ex: "adiciona" não "adicionado")
- **Primeira letra minúscula**
- **Sem ponto final**

#### Corpo (Body)
- **Máximo 72 caracteres por linha**
- **Explique o QUE e PORQUÊ**, não o COMO
- **Use presente do imperativo**

#### Rodapé (Footer)
- **Breaking changes**: `BREAKING CHANGE: <descrição>`
- **Issues**: `Closes #123` ou `Fixes #456`

### Exemplos de Commits

#### Commit Simples
```
feat(auth): adiciona sistema de login com JWT
```

#### Commit com Corpo
```
fix(api): corrige erro de validação no endpoint de usuários

O campo email não estava sendo validado corretamente,
permitindo emails inválidos no banco de dados.
```

#### Commit com Breaking Change
```
feat(api): atualiza estrutura da resposta da API

BREAKING CHANGE: A resposta da API agora retorna dados em formato diferente.
Clientes precisam atualizar para a nova estrutura.
```

#### Commit com Issue
```
fix(frontend): resolve problema de loading infinito

Fixes #142
```

### Escopos Sugeridos

- `auth` - Autenticação e autorização
- `api` - API e endpoints
- `frontend` - Interface do usuário
- `backend` - Lógica do servidor
- `database` - Banco de dados
- `config` - Configurações
- `security` - Segurança
- `performance` - Performance
- `ui` - Interface do usuário
- `ux` - Experiência do usuário

## 🔧 Comandos Úteis

### Configuração do Git

```bash
# Configurar nome e email
git config --global user.name "Seu Nome"
git config --global user.email "seu.email@example.com"

# Configurar editor padrão
git config --global core.editor "code --wait"
```

### Workflow Básico

```bash
# Criar nova branch
git checkout -b feature/nova-funcionalidade

# Adicionar mudanças
git add .

# Commit com mensagem
git commit -m "feat(auth): adiciona sistema de login"

# Push para repositório remoto
git push origin feature/nova-funcionalidade

# Voltar para develop
git checkout develop

# Atualizar develop
git pull origin develop

# Deletar branch local após merge
git branch -d feature/nova-funcionalidade
```

### Comandos Avançados

```bash
# Ver histórico de commits
git log --oneline --graph

# Alterar último commit
git commit --amend -m "nova mensagem"

# Fazer rebase interativo
git rebase -i HEAD~3

# Resetar último commit (mantém mudanças)
git reset --soft HEAD~1

# Stash (guardar mudanças temporariamente)
git stash
git stash pop
```

## ✅ Checklist antes do Commit

- [ ] Código está funcionando corretamente?
- [ ] Testes estão passando?
- [ ] Commit message segue o padrão?
- [ ] Não há arquivos desnecessários (logs, node_modules, etc)?
- [ ] Não há informações sensíveis (senhas, tokens)?
- [ ] Mudanças estão em uma branch adequada?

## 🚫 O que NÃO fazer

- ❌ Commits muito grandes com muitas mudanças
- ❌ Mensagens vagas como "fix bug" ou "update code"
- ❌ Commits direto na main/master
- ❌ Não testar antes do commit
- ❌ Incluir arquivos temporários ou de configuração local
- ❌ Misturar diferentes tipos de mudanças em um commit

## 💡 Vantagens dos Padrões de Commit

### 🔍 Rastreabilidade
- **Histórico claro**: Facilita a compreensão do que foi alterado e quando
- **Busca eficiente**: Permite encontrar mudanças específicas rapidamente
- **Debugging**: Ajuda a identificar a origem de bugs e problemas

### 🤝 Colaboração
- **Comunicação**: Mensagens padronizadas facilitam o entendimento entre a equipe
- **Code Review**: Revisores conseguem entender o contexto das mudanças
- **Onboarding**: Novos membros da equipe se adaptam mais rapidamente

### 🤖 Automação
- **Changelog**: Geração automática de logs de mudanças
- **Versionamento**: Automação de bumps de versão baseados no tipo de commit
- **CI/CD**: Triggers automáticos para diferentes tipos de mudanças

### 📊 Métricas
- **Análise**: Possibilita análise de tipos de mudanças mais frequentes
- **Produtividade**: Métricas sobre entrega e qualidade do código
- **Tendências**: Identificação de padrões no desenvolvimento

## 📚 Referências

- [Conventional Commits](https://www.conventionalcommits.org/)
- [Git Flow](https://nvie.com/posts/a-successful-git-branching-model/)
- [How to Write a Git Commit Message](https://chris.beams.io/posts/git-commit/)

---
