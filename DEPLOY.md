# 🚀 Guia Rápido de Deploy - LOLZIN

## Deploy no Render (Recomendado)

### Passo 1: Preparar o Repositório GitHub

```bash
# Inicialize o Git (se ainda não fez)
git init

# Adicione todos os arquivos
git add .

# Faça o commit inicial
git commit -m "Initial commit - LOLZIN"

# Crie um repositório no GitHub e conecte
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/lolzin.git
git push -u origin main
```

### Passo 2: Deploy Automático via Blueprint

1. Acesse: https://dashboard.render.com/

2. Clique em **"New +"** → **"Blueprint"**

3. Conecte seu repositório GitHub

4. O Render detectará o arquivo `render.yaml` e criará automaticamente:
   - **lolzin-api**: Backend API (Node.js)
   - **lolzin-web**: Frontend (Static Site)

5. Aguarde o build e deploy (5-10 minutos)

6. Acesse a URL fornecida!

### Passo 3 (Alternativo): Deploy Manual

#### Deploy do Backend

1. **New +** → **Web Service**
2. Conecte o repositório
3. Configure:
   - Name: `lolzin-api`
   - Environment: `Node`
   - Build Command: `npm install`
   - Start Command: `node server/index.js`
4. Clique em **Create Web Service**
5. Copie a URL (ex: `https://lolzin-api.onrender.com`)

#### Deploy do Frontend

1. **New +** → **Static Site**
2. Conecte o mesmo repositório
3. Configure:
   - Name: `lolzin-web`
   - Build Command: `npm install && npm run build`
   - Publish Directory: `dist`
4. Em **Environment Variables**, adicione:
   - Key: `VITE_API_URL`
   - Value: URL do backend copiada acima
5. Clique em **Create Static Site**

## Testando Localmente

```bash
# Terminal 1 - Backend
npm run server

# Terminal 2 - Frontend
npm run dev
```

Acesse: http://localhost:5173

## Problemas Comuns

### Backend não conecta
- Verifique se `VITE_API_URL` está configurado corretamente
- Certifique-se de que ambos os serviços estão rodando

### Build falha
- Verifique se todas as dependências estão instaladas
- Confirme que Node.js está na versão 16+

### Dados não aparecem
- Verifique se o arquivo `src/data/database.json` existe
- Confirme que a API está respondendo em `/api/players`

## Atualizações

Para atualizar o site após mudanças:

```bash
git add .
git commit -m "Descrição das mudanças"
git push
```

O Render fará o deploy automático!

## URLs Importantes

- Dashboard Render: https://dashboard.render.com/
- Documentação Render: https://render.com/docs
- GitHub: https://github.com

## Contato

Para dúvidas ou problemas, abra uma issue no repositório GitHub.

---

✨ **Seu site estará online em minutos!**
