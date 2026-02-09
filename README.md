# 🚀 AILA - Formulário de Onboarding

## Deploy na Vercel

### Método 1: Via Interface (Mais Fácil)

1. Acesse: https://vercel.com
2. Faça login (ou crie conta)
3. Clique em "Add New..." > "Project"
4. Arraste a pasta `aila-vercel-deploy` inteira
5. Clique em "Deploy"
6. Aguarde 30 segundos
7. **Copie a URL gerada!**

### Método 2: Via CLI

```bash
npm install -g vercel
cd aila-vercel-deploy
vercel
```

## ⚠️ IMPORTANTE: Configurar Webhook

Após o deploy, você precisa:

1. Copiar a URL do site (ex: https://aila-onboarding.vercel.app)
2. Abrir o arquivo `index.html`
3. Procurar a linha 1089
4. Substituir:
   ```javascript
   const webhookURL = 'https://SEU-N8N-WEBHOOK-URL-AQUI/aila-onboarding';
   ```
   Por:
   ```javascript
   const webhookURL = 'https://sua-url-do-n8n.com/webhook/aila-onboarding';
   ```
5. Fazer novo deploy com o arquivo atualizado

## 📁 Estrutura

```
aila-vercel-deploy/
├── index.html (formulário completo)
├── vercel.json (configuração)
└── README.md (este arquivo)
```

## 🆘 Precisa de Ajuda?

Consulte o GUIA-INSTALACAO-COMPLETO.md na pasta pai.
