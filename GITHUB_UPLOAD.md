# Guia de Upload para GitHub

Este arquivo contém instruções passo a passo para fazer upload do projeto para o GitHub.

## 📋 Pré-requisitos

1. **Conta GitHub**: Crie uma em [github.com](https://github.com)
2. **Git instalado**: Baixe em [git-scm.com](https://git-scm.com)
3. **Configurar Git** (se não fez ainda):
   ```bash
   git config --global user.name "Seu Nome"
   git config --global user.email "seu.email@example.com"
   ```

## 🚀 Passo a Passo

### 1. Criar Repositório no GitHub

1. Acesse [github.com](https://github.com) e faça login
2. Clique no ícone **+** no canto superior direito
3. Selecione **New repository**
4. Preencha os dados:
   - **Repository name**: `omnichannel-clinica`
   - **Description**: `Sistema Omnichannel centralizado para clínica médica`
   - **Public** ou **Private**: Escolha sua preferência
   - **Initialize with**: Deixe em branco (já temos arquivos locais)
5. Clique em **Create repository**

### 2. Configurar Repositório Local

```bash
# Navegue até o diretório do projeto
cd /home/ubuntu/omnichannel_clinica

# Adicione o repositório remoto
git remote add origin https://github.com/SEU_USUARIO/omnichannel-clinica.git

# Verifique se foi adicionado corretamente
git remote -v
```

### 3. Fazer Push para GitHub

```bash
# Renomear branch para 'main' (padrão do GitHub)
git branch -M main

# Fazer push dos arquivos
git push -u origin main
```

### 4. Autenticação

Você será solicitado a se autenticar. Escolha uma opção:

**Opção A: Token de Acesso Pessoal (Recomendado)**

1. No GitHub, vá para **Settings** → **Developer settings** → **Personal access tokens**
2. Clique em **Generate new token**
3. Selecione os escopos: `repo`, `workflow`
4. Clique em **Generate token**
5. Copie o token
6. Quando solicitado, use o token como senha

**Opção B: SSH (Avançado)**

1. Gere uma chave SSH:
   ```bash
   ssh-keygen -t ed25519 -C "seu.email@example.com"
   ```
2. Adicione a chave ao GitHub (Settings → SSH and GPG keys)
3. Use a URL SSH ao adicionar o remote:
   ```bash
   git remote set-url origin git@github.com:SEU_USUARIO/omnichannel-clinica.git
   ```

## 📤 Após o Upload

### Verificar Upload

1. Acesse seu repositório no GitHub
2. Verifique se todos os arquivos estão lá
3. Veja o histórico de commits

### Adicionar Badges ao README

Você pode adicionar badges ao README para mostrar informações do projeto:

```markdown
# Sistema Omnichannel para Clínica Médica

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub stars](https://img.shields.io/github/stars/SEU_USUARIO/omnichannel-clinica.svg)](https://github.com/SEU_USUARIO/omnichannel-clinica/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/SEU_USUARIO/omnichannel-clinica.svg)](https://github.com/SEU_USUARIO/omnichannel-clinica/network)
```

### Habilitar GitHub Pages (Opcional)

Para hospedar o site automaticamente:

1. Vá para **Settings** → **Pages**
2. Em **Source**, selecione **main branch**
3. Selecione a pasta **root**
4. Clique em **Save**
5. Seu site estará em: `https://SEU_USUARIO.github.io/omnichannel-clinica/`

## 🔄 Atualizações Futuras

Para fazer push de novas mudanças:

```bash
# Faça suas mudanças
# ...

# Adicione os arquivos modificados
git add .

# Crie um commit
git commit -m "Descrição das mudanças"

# Faça push para GitHub
git push origin main
```

## 🌿 Trabalhando com Branches

Para trabalhar em novas funcionalidades:

```bash
# Crie uma nova branch
git checkout -b feature/nova-funcionalidade

# Faça suas mudanças
# ...

# Commit
git add .
git commit -m "feat: Descrição da nova funcionalidade"

# Push da branch
git push origin feature/nova-funcionalidade

# Abra um Pull Request no GitHub
```

## 📊 Estatísticas do Repositório

Após fazer upload, você poderá ver:

- **Insights**: Análise de código e atividade
- **Network**: Visualizar branches e merges
- **Releases**: Criar versões do projeto
- **Wiki**: Documentação adicional
- **Discussions**: Fórum de discussão

## 🆘 Troubleshooting

### Erro: "fatal: remote origin already exists"

```bash
# Remova o remote existente
git remote remove origin

# Adicione novamente
git remote add origin https://github.com/SEU_USUARIO/omnichannel-clinica.git
```

### Erro: "Permission denied (publickey)"

Use HTTPS ao invés de SSH:
```bash
git remote set-url origin https://github.com/SEU_USUARIO/omnichannel-clinica.git
```

### Erro: "fatal: 'origin' does not appear to be a 'git' repository"

Verifique se está no diretório correto:
```bash
cd /home/ubuntu/omnichannel_clinica
git remote -v
```

## 📚 Recursos Úteis

- [GitHub Docs](https://docs.github.com/)
- [Git Documentation](https://git-scm.com/doc)
- [GitHub Flow](https://guides.github.com/introduction/flow/)
- [Markdown Guide](https://www.markdownguide.org/)

## ✅ Checklist Final

- [ ] Repositório criado no GitHub
- [ ] Remote adicionado localmente
- [ ] Arquivos fazem push com sucesso
- [ ] Todos os arquivos estão no GitHub
- [ ] README está visível
- [ ] Licença está configurada
- [ ] GitHub Pages habilitado (opcional)

---

**Pronto!** Seu projeto está no GitHub! 🎉

Você pode compartilhar o link do repositório com outras pessoas:
`https://github.com/SEU_USUARIO/omnichannel-clinica`
