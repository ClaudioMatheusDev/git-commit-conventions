# 🌍 Cenários Reais de Desenvolvimento

## 🚀 Startup/Produto Novo

### Fase de MVP
```bash
# Criação inicial do projeto
feat: inicializa projeto com estrutura básica

# Funcionalidades essenciais
feat(auth): adiciona sistema de login simples
feat(user): implementa cadastro de usuários
feat(dashboard): adiciona tela principal do app

# Ajustes rápidos
fix(auth): corrige redirecionamento após login
style(ui): melhora layout da página inicial
```

### Crescimento Rápido
```bash
# Novas funcionalidades baseadas em feedback
feat(notifications): adiciona notificações por email
feat(payment): integra gateway de pagamento
feat(search): adiciona busca básica

# Otimizações necessárias
perf(database): adiciona índices para queries lentas
fix(memory): corrige vazamento de memória no upload
```

## 🏢 Empresa Estabelecida

### Manutenção de Sistema Legacy
```bash
# Correções em sistema antigo
fix(legacy): corrige compatibilidade com IE11
refactor(jquery): migra componente para React
chore(deps): atualiza dependências com vulnerabilidades

# Melhorias graduais
feat(api): adiciona novo endpoint mantendo compatibilidade
perf(cache): implementa cache para reduzir carga do banco
```

### Modernização
```bash
# Migração tecnológica
refactor(frontend): migra de jQuery para React
refactor(backend): migra de PHP para Node.js
build(docker): containeriza aplicação

# Atualização de infraestrutura
chore(k8s): migra para Kubernetes
ci(pipeline): implementa GitOps com ArgoCD
```

## 🛒 E-commerce

### Funcionalidades Críticas
```bash
# Carrinho de compras
feat(cart): adiciona funcionalidade de carrinho
feat(checkout): implementa processo de checkout
feat(payment): integra múltiplos meios de pagamento

# Inventário
feat(inventory): adiciona controle de estoque
fix(stock): corrige sincronização de estoque
perf(search): otimiza busca de produtos
```

### Sazonalidade
```bash
# Preparação para Black Friday
perf(infra): escala horizontal para alto tráfego
feat(promo): adiciona sistema de cupons
monitor(alerts): adiciona alertas de performance

# Pós-evento
fix(orders): corrige processamento de pedidos em lote
refactor(cache): otimiza cache após análise de tráfego
```

## 🏥 Sistema de Saúde

### Compliance e Segurança
```bash
# LGPD/GDPR
feat(privacy): implementa consentimento de cookies
feat(data): adiciona exportação de dados pessoais
fix(security): corrige vazamento de dados sensíveis

# Auditoria
feat(audit): adiciona log de todas as ações médicas
feat(backup): implementa backup automático diário
```

### Integração com Sistemas
```bash
# APIs médicas
feat(integration): integra com sistema de laboratório
feat(hl7): implementa padrão HL7 para troca de dados
fix(sync): corrige sincronização com sistema hospitalar
```

## 🏦 Fintech

### Regulamentações
```bash
# Compliance bancário
feat(kyc): implementa processo KYC automático
feat(aml): adiciona detecção de lavagem de dinheiro
fix(pci): corrige conformidade PCI-DSS
```

### Transações
```bash
# Processamento de pagamentos
feat(pix): implementa PIX como meio de pagamento
feat(international): adiciona transferências internacionais
fix(reconciliation): corrige conciliação bancária
```

## 📱 Aplicativo Mobile

### Funcionalidades Mobile
```bash
# Recursos nativos
feat(camera): adiciona captura de fotos
feat(location): implementa geolocalização
feat(push): adiciona notificações push

# Offline
feat(offline): adiciona modo offline
fix(sync): corrige sincronização de dados
```

### Store Deployment
```bash
# Deploy nas lojas
build(ios): prepara build para App Store
build(android): gera APK para Play Store
fix(review): corrige problemas apontados pela Apple
```

## 🎮 Gaming

### Gameplay
```bash
# Mecânicas de jogo
feat(combat): adiciona sistema de combate
feat(inventory): implementa sistema de inventário
fix(physics): corrige colisões entre objetos
```

### Monetização
```bash
# Sistema de compras
feat(shop): adiciona loja in-app
feat(battle-pass): implementa sistema de battle pass
fix(ads): corrige exibição de anúncios
```

## 📊 Sistema de Analytics

### Coleta de Dados
```bash
# Tracking
feat(events): adiciona tracking de eventos customizados
feat(session): implementa tracking de sessão
fix(gdpr): adiciona opt-out para tracking
```

### Processamento
```bash
# Big Data
feat(pipeline): implementa pipeline de ETL
perf(queries): otimiza queries do data warehouse
fix(streaming): corrige processamento em tempo real
```

## 🏗️ Arquitetura de Microsserviços

### Serviços
```bash
# Novos serviços
feat(user-service): cria microsserviço de usuários
feat(notification-service): implementa serviço de notificações
fix(api-gateway): corrige roteamento entre serviços
```

### Comunicação
```bash
# Mensageria
feat(messaging): implementa comunicação via RabbitMQ
feat(events): adiciona event sourcing
fix(circuit-breaker): corrige circuit breaker pattern
```

## 🔄 DevOps/SRE

### Infraestrutura
```bash
# Infraestrutura como código
feat(terraform): adiciona provisionamento automático
feat(helm): cria charts para deploy no Kubernetes
fix(monitoring): corrige coleta de métricas
```

### Automação
```bash
# CI/CD
feat(pipeline): implementa pipeline de deploy automático
feat(testing): adiciona testes automatizados
fix(rollback): corrige processo de rollback
```

## 📈 Cenários de Crescimento

### Escalabilidade
```bash
# Performance sob carga
perf(database): implementa sharding horizontal
perf(cache): adiciona cache distribuído
fix(bottleneck): remove gargalo de performance
```

### Monitoramento
```bash
# Observabilidade
feat(metrics): adiciona métricas de negócio
feat(tracing): implementa distributed tracing
fix(alerting): corrige configuração de alertas
```

## 🎯 Dicas por Cenário

### Startup
- Commits frequentes e pequenos
- Foco em funcionalidades essenciais
- Documentação mínima mas clara

### Empresa Grande
- Commits bem documentados
- Referências a tickets/issues
- Consideração de impacto em outros times

### Produto Crítico
- Commits com contexto completo
- Testes obrigatórios
- Processo de review rigoroso

### Open Source
- Commits autoexplicativos
- Documentação completa
- Consideração da comunidade