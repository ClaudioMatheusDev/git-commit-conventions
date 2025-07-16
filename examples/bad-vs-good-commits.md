# ❌ ✅ Commits Ruins vs Bons

## 🎯 Mensagens de Commit

### ❌ Ruins
```bash
# Muito vago
git commit -m "fix bug"
git commit -m "update code"
git commit -m "changes"
git commit -m "stuff"

# Sem contexto
git commit -m "fix"
git commit -m "update"
git commit -m "new feature"
git commit -m "improvements"

# Tempo verbal errado
git commit -m "fixed login bug"
git commit -m "adding new button"
git commit -m "updated dependencies"
git commit -m "will fix later"
```

### ✅ Bons
```bash
# Específico e claro
git commit -m "fix(auth): corrige validação de senha vazia"
git commit -m "feat(user): adiciona avatar personalizado"
git commit -m "docs(readme): atualiza instruções de instalação"
git commit -m "perf(api): otimiza consulta de usuários"

# Com contexto adequado
git commit -m "fix(payment): resolve timeout na integração com gateway"
git commit -m "feat(search): implementa busca com filtros avançados"
git commit -m "refactor(database): extrai queries para repository pattern"
git commit -m "test(auth): adiciona testes para fluxo de recuperação de senha"
```

## 🔍 Especificidade

### ❌ Ruins
```bash
# Muito genérico
git commit -m "fix frontend"
git commit -m "update API"
git commit -m "improve performance"
git commit -m "fix styles"

# Sem escopo
git commit -m "add validation"
git commit -m "remove unused code"
git commit -m "update configuration"
git commit -m "fix error handling"
```

### ✅ Bons
```bash
# Específico com escopo
git commit -m "fix(login): corrige validação de email inválido"
git commit -m "feat(dashboard): adiciona gráfico de vendas mensais"
git commit -m "perf(search): implementa debounce na busca em tempo real"
git commit -m "style(header): ajusta responsividade em mobile"

# Contexto claro
git commit -m "feat(notification): adiciona notificações push para pedidos"
git commit -m "fix(checkout): resolve erro de cálculo de frete"
git commit -m "refactor(auth): centraliza lógica de token em AuthService"
git commit -m "test(payment): adiciona testes de integração com Stripe"
```

## 📏 Tamanho da Mensagem

### ❌ Ruins
```bash
# Muito longo (>50 caracteres)
git commit -m "feat(user): adiciona funcionalidade completa de gerenciamento de perfil de usuário incluindo upload de avatar, edição de informações pessoais e configurações de privacidade"

# Muito curto
git commit -m "fix"
git commit -m "update"
git commit -m "new"
git commit -m "change"
```

### ✅ Bons
```bash
# Tamanho ideal (~50 caracteres)
git commit -m "feat(user): adiciona upload de avatar"
git commit -m "fix(api): corrige timeout na consulta"
git commit -m "docs: atualiza guia de instalação"
git commit -m "perf(db): otimiza query de produtos"
```

## 🎨 Formato e Estrutura

### ❌ Ruins
```bash
# Sem padrão
git commit -m "Fix bug in login page"
git commit -m "ADD: new user feature"
git commit -m "Updated the database schema"
git commit -m "bugfix: authentication issues"

# Pontuação incorreta
git commit -m "feat(auth): adiciona login."
git commit -m "Fix(API): corrige erro!!!"
git commit -m "docs: atualiza README..."
git commit -m "feat(user): adiciona perfil?"
```

### ✅ Bons
```bash
# Formato consistente
git commit -m "feat(auth): adiciona login com Google"
git commit -m "fix(api): corrige erro de validação"
git commit -m "docs(readme): atualiza instruções"
git commit -m "style(ui): melhora layout do header"

# Sem pontuação final
git commit -m "feat(user): adiciona edição de perfil"
git commit -m "fix(payment): resolve erro de processamento"
git commit -m "test(auth): adiciona testes de login"
git commit -m "chore(deps): atualiza dependências"
```

## 💬 Comunicação

### ❌ Ruins
```bash
# Linguagem misturada
git commit -m "fix(auth): corrige login bug"
git commit -m "feat(user): add new profile feature"
git commit -m "docs: update README file"
git commit -m "perf(api): improve performance da API"

# Informações irrelevantes
git commit -m "feat(user): adiciona perfil (finalmente!!!)"
git commit -m "fix(bug): corrige erro (que saco)"
git commit -m "update: mudanças que o chefe pediu"
git commit -m "hotfix: bug crítico - trabalhei até 2h da manhã"
```

### ✅ Bons
```bash
# Linguagem consistente (português)
git commit -m "feat(auth): adiciona login com Google"
git commit -m "fix(user): corrige validação de email"
git commit -m "docs(readme): atualiza guia de instalação"
git commit -m "perf(api): otimiza consulta de usuários"

# Profissional e objetivo
git commit -m "feat(notification): implementa notificações push"
git commit -m "fix(payment): resolve timeout no gateway"
git commit -m "test(auth): adiciona testes de integração"
git commit -m "chore(ci): configura pipeline de deploy"
```

## 🔄 Commits Múltiplos

### ❌ Ruins
```bash
# Commits muito grandes
git commit -m "feat: adiciona sistema completo de usuários, autenticação, perfis, notificações e dashboard"

# Commits muito pequenos
git commit -m "fix: remove console.log"
git commit -m "fix: adiciona ponto e vírgula"
git commit -m "fix: corrige indentação"
git commit -m "fix: remove comentário"
```

### ✅ Bons
```bash
# Commits com escopo apropriado
git commit -m "feat(auth): adiciona sistema de autenticação"
git commit -m "feat(user): implementa perfil de usuário"
git commit -m "feat(dashboard): adiciona dashboard principal"
git commit -m "feat(notification): implementa notificações"

# Agrupamento lógico
git commit -m "style(auth): corrige formatação e remove logs"
git commit -m "refactor(utils): extrai funções comuns"
git commit -m "test(auth): adiciona testes unitários"
```

## 📚 Contexto e Documentação

### ❌ Ruins
```bash
# Sem contexto no corpo
git commit -m "feat(api): adiciona endpoint de usuários

endpoint novo"

# Informações desnecessárias
git commit -m "fix(auth): corrige bug

Bug que estava me irritando há semanas
Finalmente consegui resolver
Testei em vários cenários
Espero que funcione agora"
```

### ✅ Bons
```bash
# Contexto útil
git commit -m "feat(api): adiciona endpoint de usuários

Implementa CRUD completo para gerenciamento de usuários
incluindo validação, paginação e filtros.

- GET /users (lista com paginação)
- POST /users (criação com validação)
- PUT /users/:id (atualização)
- DELETE /users/:id (remoção)

Closes #123"

# Explicação clara do problema
git commit -m "fix(auth): corrige validação de token expirado

O middleware de autenticação não estava verificando
corretamente tokens expirados, permitindo acesso
não autorizado. Adiciona validação de timestamp
e retorna erro 401 para tokens inválidos.

Fixes #456"
```

## 🎯 Referências e Issues

### ❌ Ruins
```bash
# Referências incorretas
git commit -m "fix(auth): corrige login - issue 123"
git commit -m "feat(user): adiciona perfil (veja PR #456)"
git commit -m "update: mudanças relacionadas ao ticket XYZ"
git commit -m "fix: resolve problema mencionado na reunião"
```

### ✅ Bons
```bash
# Referências corretas
git commit -m "fix(auth): corrige timeout na validação

Aumenta timeout de validação de 5s para 30s para
evitar falhas em redes lentas.

Fixes #123"

git commit -m "feat(user): adiciona edição de perfil

Implementa interface para usuários editarem
informações pessoais e configurações.

Closes #456
Relates to #789"
```

## 🔧 Tipos de Commit

### ❌ Ruins
```bash
# Tipos incorretos
git commit -m "update(auth): adiciona nova funcionalidade"
git commit -m "change(api): corrige bug na validação"
git commit -m "new(user): adiciona sistema de perfil"
git commit -m "improve(perf): otimiza consulta"
```

### ✅ Bons
```bash
# Tipos corretos
git commit -m "feat(auth): adiciona login com redes sociais"
git commit -m "fix(api): corrige validação de dados"
git commit -m "feat(user): implementa sistema de perfil"
git commit -m "perf(db): otimiza consulta de produtos"
```

## 📊 Resumo das Boas Práticas

### ✅ Checklist de Commit Perfeito
- [ ] Usa formato padronizado: `<tipo>(<escopo>): <descrição>`
- [ ] Tipo correto (feat, fix, docs, etc.)
- [ ] Escopo apropriado quando necessário
- [ ] Descrição clara e específica
- [ ] Máximo 50 caracteres no título
- [ ] Presente do imperativo
- [ ] Primeira letra minúscula
- [ ] Sem ponto final
- [ ] Linguagem consistente
- [ ] Contexto no corpo quando necessário
- [ ] Referências corretas a issues
- [ ] Breaking changes documentadas

### ❌ Sinais de Alerta
- Mensagens vagas ou genéricas
- Commits muito grandes ou muito pequenos
- Mistura de tipos de mudança
- Linguagem inconsistente
- Informações irrelevantes
- Falta de contexto quando necessário
- Referências incorretas
- Formatação inconsistente