# 🚀 Exemplos Avançados de Commits

## 📋 Commits com Corpo (Body)

### Exemplo 1: Funcionalidade Complexa
```
feat(auth): adiciona sistema de autenticação de dois fatores

Implementa 2FA usando TOTP (Time-based One-Time Password) para
aumentar a segurança das contas de usuário. O sistema suporta
aplicativos como Google Authenticator e Authy.

- Adiciona geração de QR code para configuração
- Implementa validação de tokens TOTP
- Adiciona backup codes para recuperação
```

### Exemplo 2: Bug Crítico
```
fix(payment): corrige falha na validação de cartão de crédito

O sistema estava aceitando cartões inválidos devido a um erro
na regex de validação. Isso causava falhas no processamento
de pagamentos e chargebacks.

- Atualiza regex para validar formato correto
- Adiciona validação de dígito verificador
- Implementa testes para casos extremos
```

### Exemplo 3: Refatoração Importante
```
refactor(database): migra ORM de Sequelize para Prisma

A mudança visa melhorar performance e developer experience.
O Prisma oferece melhor type safety e queries mais eficientes.

- Converte todos os models para schema Prisma
- Atualiza queries em todos os services
- Mantém compatibilidade com dados existentes
- Adiciona migrations para transição suave
```

## 🔄 Commits com Rodapé (Footer)

### Exemplo 1: Breaking Change
```
feat(api): atualiza estrutura de resposta da API

Padroniza todas as respostas da API para seguir o formato
JSON:API specification, melhorando consistência e usabilidade.

BREAKING CHANGE: Todas as respostas agora seguem formato padrão.
Clientes devem atualizar para processar novo formato de resposta.
Ver migração em docs/api-migration.md
```

### Exemplo 2: Issue Reference
```
fix(upload): resolve problema de upload de arquivos grandes

Aumenta limite de upload para 50MB e melhora handling de timeout
para arquivos grandes. Também adiciona progress indicator.

- Atualiza configuração do multer
- Implementa chunked upload para arquivos > 10MB
- Adiciona retry automático em caso de falha

Closes #456
Fixes #789
```

### Exemplo 3: Múltiplas Referências
```
feat(notifications): adiciona sistema de notificações push

Implementa notificações push usando Firebase Cloud Messaging
para web e mobile. Suporta notificações personalizadas e
agendamento.

- Integra Firebase SDK
- Adiciona service worker para web
- Implementa templates de notificação
- Adiciona painel de configuração

Closes #123
Relates to #456
Implements #789
```

## 💥 Breaking Changes

### Exemplo 1: Mudança na API
```
feat(api): implementa versionamento de API

Adiciona suporte para múltiplas versões da API para melhor
compatibilidade com clientes existentes.

BREAKING CHANGE: Endpoints movidos para /v1/. Clientes devem
atualizar URLs para incluir versão. Suporte para URLs antigas
será removido em 6 meses.
```

### Exemplo 2: Mudança no Banco
```
refactor(database): normaliza estrutura de usuários

Separa informações de perfil da tabela users para melhor
organização e performance.

BREAKING CHANGE: Estrutura da tabela users alterada.
Executar migration obrigatória: npm run db:migrate
```

### Exemplo 3: Mudança na Configuração
```
chore(config): atualiza estrutura de configuração

Simplifica configuração do projeto e adiciona validação
automática de variáveis de ambiente.

BREAKING CHANGE: Formato do arquivo .env alterado.
Consultar .env.example para nova estrutura.
```

## 🎯 Commits Completos (Header + Body + Footer)

### Exemplo 1: Feature Completa
```
feat(search): adiciona busca avançada com filtros

Implementa sistema de busca com filtros por categoria, preço,
localização e data. Inclui sugestões em tempo real e 
autocomplete.

- Adiciona índices Elasticsearch para performance
- Implementa filtros dinâmicos no frontend
- Adiciona cache para queries frequentes
- Implementa analytics de busca

Closes #234
Relates to #567
```

### Exemplo 2: Fix Crítico
```
fix(security): corrige vulnerabilidade de XSS no chat

Remove possibilidade de injeção de scripts maliciosos através
de mensagens do chat. Implementa sanitização adequada de HTML.

- Adiciona DOMPurify para sanitização
- Implementa whitelist de tags permitidas
- Adiciona testes de segurança
- Atualiza CSP headers

Fixes #SECURITY-001
BREAKING CHANGE: Mensagens com HTML customizado serão removidas.
```

### Exemplo 3: Performance
```
perf(frontend): otimiza carregamento da página inicial

Reduz tempo de carregamento inicial em 40% através de code
splitting, lazy loading e otimização de imagens.

- Implementa code splitting por rotas
- Adiciona lazy loading para componentes pesados
- Otimiza imagens com WebP e compression
- Implementa service worker para cache
- Adiciona preload para recursos críticos

Closes #345
Improves #456
```

## 📊 Commits de Análise e Métricas

### Exemplo 1: Monitoramento
```
feat(monitoring): adiciona dashboard de métricas

Implementa dashboard em tempo real para monitorar performance
da aplicação e health dos serviços.

- Integra Prometheus para coleta de métricas
- Adiciona Grafana para visualização
- Implementa alertas automáticos
- Adiciona métricas customizadas de negócio

Closes #678
```

### Exemplo 2: Analytics
```
feat(analytics): implementa tracking de eventos de usuário

Adiciona sistema de analytics para entender comportamento
dos usuários e otimizar experiência.

- Integra Google Analytics 4
- Implementa eventos customizados
- Adiciona GDPR compliance
- Cria dashboards de analytics

Closes #789
```

## 🔐 Commits de Segurança

### Exemplo 1: Autenticação
```
feat(security): implementa rate limiting por IP

Adiciona proteção contra ataques de força bruta e DDoS
através de rate limiting configurável.

- Implementa Redis para contagem de requests
- Adiciona middleware de rate limiting
- Configura limites por endpoint
- Adiciona whitelist para IPs confiáveis

Closes #SECURITY-002
```

### Exemplo 2: Auditoria
```
feat(audit): adiciona log de auditoria para ações críticas

Implementa sistema de auditoria para rastrear todas as
ações sensíveis realizadas por usuários.

- Adiciona tabela de audit_logs
- Implementa middleware de auditoria
- Adiciona interface para consulta de logs
- Implementa retenção automática de logs

Closes #AUDIT-001
```

## 🎨 Dicas para Commits Avançados

1. **Corpo detalhado**: Explique o QUE e PORQUÊ, não o COMO
2. **Contexto**: Forneça contexto suficiente para entender a mudança
3. **Impacto**: Descreva o impacto da mudança no sistema
4. **Referências**: Sempre referencie issues relacionadas
5. **Breaking Changes**: Documente mudanças que quebram compatibilidade
6. **Limite de linhas**: Mantenha linhas do corpo com máximo 72 caracteres
7. **Separação**: Use linha em branco entre header, body e footer