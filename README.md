# Investidor Inteligente — Dashboard do Formulário

Este repositório contém uma página estática (`index.html`) com os resultados do formulário de validação acadêmica.

## Como visualizar no computador

Basta abrir o arquivo `index.html` no navegador, ou servir localmente:

```bash
python3 -m http.server 4173
```

Depois acesse: `http://localhost:4173`

## Como abrir no celular (mesma rede Wi‑Fi)

1. No computador, rode:

```bash
python3 -m http.server 4173 --bind 0.0.0.0
```

2. Descubra o IP local do computador:

```bash
hostname -I
```

3. No celular (na mesma rede Wi‑Fi), abra:

`http://SEU_IP_LOCAL:4173`

Exemplo: `http://192.168.0.15:4173`

## Como publicar e gerar link público (Vercel)

### Opção 1 — Via site (mais simples)

1. Acesse [https://vercel.com/new](https://vercel.com/new)
2. Importe este repositório do GitHub.
3. Framework: **Other** (ou auto detectado como estático).
4. Clique em **Deploy**.
5. A Vercel vai gerar uma URL pública (`https://...vercel.app`) para abrir no celular e compartilhar.

### Opção 2 — Via CLI

Pré-requisitos:

```bash
npm i -g vercel
vercel login
```

Deploy:

```bash
vercel
```

Produção:

```bash
vercel --prod
```

A CLI retorna o link público ao final.
