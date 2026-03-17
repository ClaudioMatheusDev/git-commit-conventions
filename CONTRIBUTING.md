# Contribuindo

Obrigado por contribuir! Este documento descreve passos e convenções para facilitar PRs e commits.

## Processo de Pull Request

1. Fork ou crie uma branch a partir de `develop`.
2. Faça commits pequenos e atômicos seguindo o padrão de commit (veja seção abaixo).
3. Abra um Pull Request apontando para `develop` e selecione o template de PR.
4. Preencha o checklist do template e aguarde a revisão.

## Convenções de Commit

Este projeto segue o padrão de Conventional Commits. O formato básico é:

```
<tipo>(<escopo>): <descrição>

<corpo opcional>

<rodapé opcional>
```

Exemplo: `feat(auth): adiciona login com JWT`

Tipos comuns: `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`, `perf`, `ci`, `build`.

## Validação de commits

Há duas camadas de validação de commit:

- **CI**: um workflow do GitHub Actions valida mensagens de commit automaticamente nas PRs.
- **Local (opcional, recomendado)**: hooks com `husky` + `commitlint` para bloquear commits locais que não seguem o padrão.

Para habilitar os hooks locais (requer Node.js + npm):

```bash
# instalar dependências de desenvolvimento
npm install

# configurar husky (instala os hooks no Git)
npx husky install

# adicionar o hook de commit-msg (caso não exista)
npx husky add .husky/commit-msg "npx --no-install commitlint --edit \"$1\""
```

Após isso, commits que não seguirem o padrão serão rejeitados localmente.

Se preferir apenas validar no CI, não é necessário rodar os passos acima.

## Testes e Lint

Documentação usa validação via GitHub Actions (Markdown lint, checagem de links e spellcheck). Execute localmente conforme as ferramentas que preferir.

## Templates e Issues

Use os templates disponíveis em `.github/` para abrir PRs e Issues.

## Código de Conduta

Veja o arquivo `CODE_OF_CONDUCT.md` para orientações sobre comportamento e respeito na comunidade.

## Contato

Para dúvidas sobre o processo, abra uma issue com a tag `question`.
# 🤝 Guia de Contribuição

Obrigado por considerar contribuir com o projeto **git-commit-conventions**! Este guia irá ajudá-lo a entender como você pode contribuir para melhorar este repositório.

## 📋 Como Contribuir

### 🐛 Reportar Problemas
- Verifique se o problema já não foi reportado nas [Issues](https://github.com/ClaudioMatheusDev/git-commit-conventions/issues)
- Use o template de issue apropriado
- Seja específico sobre o problema encontrado
- Inclua exemplos e contexto quando possível

### 💡 Sugerir Melhorias
- Abra uma [Issue](https://github.com/ClaudioMatheusDev/git-commit-conventions/issues) com o rótulo `enhancement`
- Descreva claramente a melhoria proposta
- Explique por que a melhoria seria útil
- Forneça exemplos de como funcionaria

### 📝 Contribuir com Documentação
- Corrija erros de digitação ou gramática
- Melhore explicações existentes
- Adicione exemplos práticos
- Traduza conteúdo (se aplicável)

### 🎯 Adicionar Novos Padrões
- Pesquise se o padrão já existe na documentação
- Baseie-se em convenções amplamente aceitas
- Forneça exemplos práticos
- Inclua justificativas para o padrão proposto

## 🚀 Processo de Contribuição

### 1. Fork do Repositório
```bash
# Clone seu fork
git clone https://github.com/SEU-USERNAME/git-commit-conventions.git
cd git-commit-conventions
```

### 2. Criar Branch para Sua Contribuição
```bash
# Crie uma branch seguindo os padrões do projeto
git checkout -b feature/minha-contribuicao
# ou
git checkout -b fix/correcao-documentacao
# ou
git checkout -b docs/melhoria-exemplo
```

### 3. Fazer as Mudanças
- Siga os padrões de commit do próprio projeto
- Mantenha as mudanças focadas e específicas
- Teste suas alterações

### 4. Commit das Mudanças
```bash
# Siga os padrões definidos no README
git add .
git commit -m "docs: adiciona exemplo de commit para hotfix"
```

### 5. Push e Pull Request
```bash
# Envie sua branch
git push origin feature/minha-contribuicao

# Abra um Pull Request no GitHub
# Use o template de PR se disponível
```

## 📏 Padrões de Contribuição

### Mensagens de Commit
- **OBRIGATÓRIO**: Siga os padrões definidos no README.md
- Use o formato: `<tipo>(<escopo>): <descrição>`
- Mantenha a descrição clara e concisa
- Use português para consistência

### Documentação
- **Idioma**: Mantenha o português como idioma principal
- **Formatação**: Use Markdown seguindo o estilo existente
- **Exemplos**: Inclua exemplos práticos sempre que possível
- **Estrutura**: Mantenha a estrutura de seções existente

### Estilo de Escrita
- Use linguagem clara e direta
- Evite jargões técnicos desnecessários
- Seja consistente com o tom do projeto
- Priorize exemplos práticos

## 🔍 Revisão de Código

### O que Esperamos
- Código/documentação que segue os padrões estabelecidos
- Mudanças bem testadas e documentadas
- Commits que seguem as convenções do projeto
- Respeito às discussões e feedback

### Processo de Revisão
1. **Revisão Automática**: Verificações básicas de formatação
2. **Revisão Manual**: Análise do conteúdo e qualidade
3. **Discussão**: Possíveis sugestões e melhorias
4. **Aprovação**: Merge após aprovação

## 🎯 Tipos de Contribuição Bem-Vindas

### 📚 Documentação
- Correção de erros de digitação
- Melhoria de explicações
- Adição de exemplos
- Estruturação de conteúdo

### 🛠️ Melhorias nos Padrões
- Novos tipos de commit
- Melhorias em escopos existentes
- Exemplos mais claros
- Casos de uso específicos

### 🎨 Organização
- Melhoria na estrutura dos arquivos
- Organização do conteúdo
- Otimização de navegação
- Adição de índices

### 🌍 Internacionalização
- Tradução para outros idiomas
- Adaptação cultural de exemplos
- Manutenção de consistência

## 🚫 O que NÃO Fazer

- ❌ Mudanças que quebram a compatibilidade sem discussão
- ❌ Commits que não seguem os padrões do projeto
- ❌ Adição de conteúdo não relacionado ao tema
- ❌ Mudanças massivas sem contexto
- ❌ Ignorar feedback da comunidade

## 📞 Ajuda e Suporte

### Onde Buscar Ajuda
- [Issues](https://github.com/ClaudioMatheusDev/git-commit-conventions/issues): Para dúvidas específicas
- [Discussions](https://github.com/ClaudioMatheusDev/git-commit-conventions/discussions): Para discussões abertas

### Contato
- Abra uma issue para discussões técnicas
- Use as discussions para ideias e sugestões gerais

## 📝 Licença

Ao contribuir, você concorda que suas contribuições serão licenciadas sob a [MIT License](LICENSE).

## 🙏 Agradecimentos

Obrigado por dedicar seu tempo para melhorar este projeto! Cada contribuição, por menor que seja, faz diferença para a comunidade de desenvolvedores.

---

**Lembre-se**: Este é um projeto da comunidade, para a comunidade. Seja respeitoso, construtivo e colaborativo! 🚀