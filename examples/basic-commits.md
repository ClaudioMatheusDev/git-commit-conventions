# 📝 Exemplos Básicos de Commits

## ✨ Novas Funcionalidades (feat)

```bash
# Funcionalidade simples
git commit -m "feat: adiciona botão de logout"

# Com escopo
git commit -m "feat(auth): adiciona autenticação via Google"

# Com emoji
git commit -m "✨ feat(user): adiciona perfil de usuário"
```

## 🐛 Correção de Bugs (fix)

```bash
# Bug simples
git commit -m "fix: corrige erro de validação de email"

# Com escopo
git commit -m "fix(api): resolve problema de timeout"

# Com emoji
git commit -m "🐛 fix(frontend): corrige layout mobile"
```

## 📚 Documentação (docs)

```bash
# Documentação geral
git commit -m "docs: atualiza README com instruções de instalação"

# Documentação de API
git commit -m "docs(api): adiciona documentação dos endpoints"

# Com emoji
git commit -m "📚 docs(contributing): adiciona guia de contribuição"
```

## 🎨 Melhorias de Estilo (style)

```bash
# Formatação de código
git commit -m "style: aplica formatação ESLint"

# CSS/Design
git commit -m "style(frontend): melhora espaçamento dos componentes"

# Com emoji
git commit -m "🎨 style: remove espaços em branco desnecessários"
```

## ♻️ Refatoração (refactor)

```bash
# Refatoração simples
git commit -m "refactor: simplifica função de validação"

# Com escopo
git commit -m "refactor(auth): extrai lógica de token para service"

# Com emoji
git commit -m "♻️ refactor(utils): otimiza função de formatação de data"
```

## 🧪 Testes (test)

```bash
# Novos testes
git commit -m "test: adiciona testes para função de login"

# Correção de testes
git commit -m "test(api): corrige testes de integração"

# Com emoji
git commit -m "🧪 test(user): adiciona testes unitários para UserService"
```

## 🔧 Tarefas de Manutenção (chore)

```bash
# Dependências
git commit -m "chore: atualiza dependências do projeto"

# Configuração
git commit -m "chore(config): adiciona configuração do Docker"

# Com emoji
git commit -m "🔧 chore: configura pipeline de CI/CD"
```

## ⚡ Melhorias de Performance (perf)

```bash
# Performance geral
git commit -m "perf: otimiza consulta do banco de dados"

# Com escopo
git commit -m "perf(frontend): reduz tamanho do bundle"

# Com emoji
git commit -m "⚡ perf(api): implementa cache para endpoints"
```

## 🔄 Integração Contínua (ci)

```bash
# Configuração de CI
git commit -m "ci: adiciona workflow do GitHub Actions"

# Correção de pipeline
git commit -m "ci(deploy): corrige configuração de deployment"

# Com emoji
git commit -m "🔄 ci: adiciona steps de teste automatizado"
```

## 🏗️ Sistema de Build (build)

```bash
# Configuração de build
git commit -m "build: adiciona configuração do Webpack"

# Scripts
git commit -m "build(scripts): adiciona script de build para produção"

# Com emoji
git commit -m "🏗️ build: otimiza processo de build"
```

## ⏪ Reversão (revert)

```bash
# Reversão simples
git commit -m "revert: desfaz mudanças no sistema de autenticação"

# Com referência
git commit -m "revert: reverte commit abc123 - feat(auth): adiciona Google OAuth"

# Com emoji
git commit -m "⏪ revert: remove funcionalidade de notificações push"
```

## 📱 Exemplos por Contexto

### Frontend (React/Vue/Angular)
```bash
feat(components): adiciona componente de loading
fix(styles): corrige responsividade do header
style(layout): melhora espaçamento entre seções
```

### Backend (API/Services)
```bash
feat(api): adiciona endpoint de upload de arquivos
fix(database): corrige conexão com MongoDB
perf(queries): otimiza consultas de usuários
```

### Mobile (React Native/Flutter)
```bash
feat(navigation): adiciona navegação por tabs
fix(permissions): corrige solicitação de permissões
style(ui): melhora interface do login
```

### DevOps
```bash
chore(docker): adiciona Dockerfile para produção
ci(github): configura actions para deploy automático
build(scripts): adiciona script de backup do banco
```

## 🎯 Dicas Importantes

1. **Seja específico**: Prefira "fix(login): corrige validação de senha" a "fix: bug"
2. **Use presente**: "adiciona" não "adicionado" ou "adicionando"
3. **Seja conciso**: Máximo 50 caracteres no título
4. **Use escopo**: Ajuda a identificar a área afetada
5. **Seja consistente**: Mantenha o mesmo padrão em todo o projeto