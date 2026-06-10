# WIHT — World Institute of Holistic Therapists

**Site oficial:** [https://lucianaN8n.github.io/wiht-org](https://lucianaN8n.github.io/wiht-org)

Website institucional da **Saber Consciente Worldwide LLC** — plataforma de credenciamento internacional e diretório global de terapeutas holísticos.

---

## Estrutura de Páginas

| Arquivo | URL | Descrição |
|---|---|---|
| `index.html` | `/` | Página principal — apresentação do WIHT, credenciais, diretório preview |
| `directory.html` | `/directory.html` | Diretório global de terapeutas verificados |
| `join.html` | `/join.html` | Como obter a certificação internacional |
| `ethics.html` | `/ethics.html` | Código de Ética WIHT |
| `privacy.html` | `/privacy.html` | Política de Privacidade + Termos de Uso (LGPD / CCPA / GDPR) |

---

## Deploy (GitHub Pages)

O site é servido via **GitHub Pages** a partir da branch `main`, pasta raiz `/`.

### Configuração inicial (fazer uma vez):

1. Acesse **Settings** → **Pages**
2. Em **Source**, selecione: `Deploy from a branch`
3. Branch: `main` / Folder: `/ (root)`
4. Clique **Save**

O site ficará disponível em:
`https://lucianaN8n.github.io/wiht-org`

### Para usar domínio próprio (ex: `wiht.org` ou `worldwide.saberconsciente.com.br`):

1. Em **Settings → Pages → Custom domain**, insira o domínio
2. No painel DNS do seu domínio, crie os seguintes registros:

**Opção A — Domínio raiz (ex: `wiht.org`):**
```
A     @     185.199.108.153
A     @     185.199.109.153
A     @     185.199.110.153
A     @     185.199.111.153
```

**Opção B — Subdomínio (ex: `worldwide.saberconsciente.com.br`):**
```
CNAME   worldwide   lucianaN8n.github.io
```

3. Aguarde até 24h para propagação DNS
4. Marque **Enforce HTTPS** após confirmação

---

## Atualizar o site

Para editar uma página e publicar:

```bash
# 1. Edite o arquivo desejado (ex: index.html)
# 2. Faça commit e push para a branch main

git add .
git commit -m "Atualiza conteúdo [descreva o que mudou]"
git push origin main
```

O GitHub Pages publica automaticamente em 1–2 minutos após o push.

---

## Adicionar terapeuta ao diretório

Abra `directory.html` e copie o bloco abaixo dentro de `<div class="therapist-list">`:

```html
<div class="therapist-row">
  <div class="avatar">XX</div>  <!-- Iniciais do nome -->
  <div class="therapist-info">
    <h3>Nome Completo</h3>
    <p class="therapist-meta">📍 Cidade, País · Online · Idiomas</p>
    <div class="therapist-tags-row">
      <span class="tag">Certificado</span>
      <span class="tag">Especialidade</span>
    </div>
  </div>
  <div class="therapist-actions">
    <span class="badge-verified">WIHT Verified</span>
    <span class="reg-num">SIHT-2025-00000</span>
    <a href="#" class="btn-profile">View Profile →</a>
  </div>
</div>
```

---

## Links dos Cursos Afiliados

| Curso | Link Hotmart |
|---|---|
| Terapeuta em Neurociências Comportamentais | https://go.hotmart.com/Q94931307D |
| Terapeuta em Análise Comportamental | https://go.hotmart.com/U89946513B |

---

## Contato Institucional

- **Email:** contato@saberconsciente.com.br
- **WhatsApp:** (11) 91331-2063
- **Instagram:** @ath_associacao
- **Entidade:** Saber Consciente Worldwide LLC — Wyoming, USA

---

*Maintained by Instituto Saber Consciente · saberconsciente.com.br*
