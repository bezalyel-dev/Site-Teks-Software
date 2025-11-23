# Guia de Deploy - Site Teks Software

## 📋 Pré-requisitos

1. Ter uma conta no GitHub
2. Ter o Git instalado no seu computador
3. Ter acesso ao repositório: https://github.com/bezalyel-dev/Site-Teks-Software.git

## 🚀 Passos para Fazer o Deploy

### 1. Fazer Push para o GitHub

Execute os seguintes comandos no terminal (PowerShell ou CMD):

```bash
cd "C:\Users\duck\Downloads\site 5.0 (1)\SITE 2027"
git push -u origin main
```

**Nota:** Na primeira vez, você precisará fazer login no GitHub. O Git pode pedir suas credenciais.

### 2. Configurar GitHub Pages

Após fazer o push:

1. Acesse: https://github.com/bezalyel-dev/Site-Teks-Software
2. Vá em **Settings** (Configurações)
3. No menu lateral, clique em **Pages**
4. Em **Source**, selecione:
   - Branch: `main`
   - Folder: `/ (root)`
5. Clique em **Save**

### 3. Acessar o Site

Após alguns minutos, seu site estará disponível em:
- `https://bezalyel-dev.github.io/Site-Teks-Software/`

Ou, se você configurou um domínio personalizado, use seu domínio.

## 🔄 Atualizar o Site

Sempre que fizer alterações no site:

```bash
cd "C:\Users\duck\Downloads\site 5.0 (1)\SITE 2027"
git add .
git commit -m "Descrição das alterações"
git push
```

O GitHub Pages atualiza automaticamente em alguns minutos.

## ⚙️ Configurações Adicionais

### Domínio Personalizado

Se você tem um domínio (ex: tekssoftware.com.br):

1. Crie um arquivo `CNAME` na raiz do projeto com o domínio:
   ```
   tekssoftware.com.br
   ```
2. Configure o DNS do seu domínio apontando para o GitHub Pages
3. Faça commit e push do arquivo CNAME

### HTTPS

O GitHub Pages fornece HTTPS automaticamente para todos os sites.

## 🐛 Solução de Problemas

### Erro de Autenticação

Se tiver problemas ao fazer push, você pode precisar usar um Personal Access Token:

1. Vá em GitHub → Settings → Developer settings → Personal access tokens
2. Crie um novo token com permissões de `repo`
3. Use o token como senha ao fazer push

### Site não atualiza

- Aguarde alguns minutos (pode levar até 10 minutos)
- Verifique se o commit foi feito corretamente
- Verifique as configurações do GitHub Pages

## 📝 Notas Importantes

- O arquivo `index.html` deve estar na raiz do projeto
- Todos os caminhos de imagens e CSS devem ser relativos
- Arquivos grandes (vídeos) podem demorar mais para carregar

