# Mochi Blog

Um blog pessoal criado com Jekyll, com tema customizado e estilo único.

## 📝 Criando Novos Posts

Use o script `new-post.sh` para gerar novos posts automaticamente:

```bash
# Post simples
./new-post.sh "Título do Meu Post"

# Post com categorias específicas
./new-post.sh "Tutorial de JavaScript" tutorial javascript programacao

# Ver ajuda
./new-post.sh --help
```

### O que o script faz:
- ✅ Cria o arquivo no formato correto: `YYYY-MM-DD-titulo-do-post.markdown`
- ✅ Adiciona o front matter automaticamente
- ✅ Inclui template com dicas de escrita
- ✅ Converte títulos com acentos e caracteres especiais
- ✅ Verifica se o arquivo já existe antes de sobrescrever

## 🚀 Desenvolvimento Local

```bash
# Instalar dependências
bundle install

# Executar servidor local
bundle exec jekyll serve

# Acessar em http://localhost:4000
```

## 📁 Estrutura do Projeto

```
mochi-blog/
├── _config.yml          # Configurações do Jekyll
├── _data/
│   └── navigation.yml   # Menu de navegação
├── _layouts/
│   ├── default.html     # Layout base
│   └── post.html        # Layout para posts
├── _posts/              # Seus posts em Markdown
├── _sass/               # Arquivos SCSS
│   ├── configs.scss     # Variáveis e configurações
│   ├── main.scss        # Estilos principais
│   ├── markdown.scss    # Estilos para conteúdo markdown
│   └── reset.scss       # Reset CSS
├── assets/
│   ├── css/             # Arquivos CSS compilados
│   ├── fonts/           # Fontes customizadas
│   ├── images/          # Imagens do site
│   └── js/              # Scripts JavaScript
└── new-post.sh          # Script para criar novos posts
```

## 🎨 Customização

### Cores do Tema
As cores principais estão definidas em `_sass/configs.scss`:
- Rosa Mochi (`$mochi-pink`)
- Roxo Mochi (`$mochi-purple`)  
- Azul Mochi (`$mochi-blue`)
- Contraste (`$mochi-contrast`)

### Adicionando Imagens
1. Coloque suas imagens em `assets/images/`
2. Referencie no markdown: `![Alt text](/assets/images/sua-imagem.png)`

### Modificando a Navegação
Edite `_data/navigation.yml` para adicionar/remover itens do menu.

## 📋 Checklist para Novos Posts

- [ ] Criar post com `./new-post.sh "Título"`
- [ ] Adicionar conteúdo interessante
- [ ] Adicionar imagens se necessário
- [ ] Revisar markdown e formatação
- [ ] Testar localmente
- [ ] Commit e push

---

Feito com ❤️ e muito 🍡 (mochi)
