# 🚀 DEPLOY — Passo a Passo Completo

Guia para subir o site WIHT no GitHub Pages do zero.

---

## PARTE 1 — Criar o repositório no GitHub

1. Acesse https://github.com/new
2. Preencha:
   - **Repository name:** `wiht-org`
   - **Visibility:** Public ✅ (obrigatório para GitHub Pages gratuito)
   - **Description:** WIHT — World Institute of Holistic Therapists
   - NÃO marque "Add a README file" (já temos um)
3. Clique **Create repository**

---

## PARTE 2 — Fazer upload dos arquivos

### Opção A — Pelo navegador (mais fácil, sem instalar nada)

1. No repositório recém-criado, clique em **"uploading an existing file"**
2. Arraste TODOS os arquivos da pasta `wiht-org` de uma vez:
   - `index.html`
   - `directory.html`
   - `join.html`
   - `ethics.html`
   - `privacy.html`
   - `README.md`
   - `_config.yml`
   - `.gitignore`
3. Em **Commit changes**, escreva: `Initial deploy — WIHT website`
4. Clique **Commit changes**

### Opção B — Via linha de comando (Git)

```bash
# Na pasta onde estão os arquivos:
git init
git add .
git commit -m "Initial deploy — WIHT website"
git branch -M main
git remote add origin https://github.com/LucianaN8n/wiht-org.git
git push -u origin main
```

---

## PARTE 3 — Ativar o GitHub Pages

1. No repositório, clique em **Settings** (aba superior)
2. No menu lateral esquerdo, clique em **Pages**
3. Em **Source**, selecione:
   - Branch: `main`
   - Folder: `/ (root)`
4. Clique **Save**
5. Aguarde 1–2 minutos

✅ O site estará disponível em:
**https://lucianaN8n.github.io/wiht-org**

---

## PARTE 4 — Verificar se está funcionando

Acesse cada URL e confirme:

- [ ] https://lucianaN8n.github.io/wiht-org → Página principal
- [ ] https://lucianaN8n.github.io/wiht-org/directory.html → Diretório
- [ ] https://lucianaN8n.github.io/wiht-org/join.html → Certificação
- [ ] https://lucianaN8n.github.io/wiht-org/ethics.html → Código de Ética
- [ ] https://lucianaN8n.github.io/wiht-org/privacy.html → Privacidade

---

## PARTE 5 — Domínio próprio (opcional)

Se quiser usar `wiht.org` ou `worldwide.saberconsciente.com.br`:

### 5a. Criar arquivo CNAME no repositório

1. No repositório, clique **Add file → Create new file**
2. Nome do arquivo: `CNAME`
3. Conteúdo (coloque apenas o domínio, sem https://):
   ```
   worldwide.saberconsciente.com.br
   ```
   ou
   ```
   wiht.org
   ```
4. Commit

### 5b. Configurar DNS

**Para subdomínio (`worldwide.saberconsciente.com.br`):**
No painel DNS do seu registro de domínio, adicione:
```
Tipo:  CNAME
Nome:  worldwide
Valor: lucianaN8n.github.io
```

**Para domínio raiz (`wiht.org`):**
```
Tipo: A  Nome: @  Valor: 185.199.108.153
Tipo: A  Nome: @  Valor: 185.199.109.153
Tipo: A  Nome: @  Valor: 185.199.110.153
Tipo: A  Nome: @  Valor: 185.199.111.153
```

### 5c. Ativar HTTPS

Após a propagação do DNS (até 24h):
1. Settings → Pages
2. Marque **Enforce HTTPS** ✅

---

## PARTE 6 — Atualizar o site no futuro

Para editar qualquer página:

1. Acesse https://github.com/LucianaN8n/wiht-org
2. Clique no arquivo que quer editar (ex: `directory.html`)
3. Clique no ícone de lápis ✏️ (Edit this file)
4. Faça as alterações
5. Clique **Commit changes**

O site atualiza automaticamente em 1–2 minutos.

---

## Suporte

Em caso de dúvida: contato@saberconsciente.com.br
