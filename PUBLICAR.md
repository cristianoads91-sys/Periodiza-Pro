# 🚀 COMO PUBLICAR O PERIODIZA PRO EM 5 MINUTOS

Este guia é para quem **nunca publicou um site**. Sem conhecimento técnico necessário.

---

## ⚡ Caminho mais rápido — Vercel

### 1️⃣ Crie uma conta grátis
- Acesse: https://vercel.com/signup
- Clique em "Continue with Email" ou logue com Google/GitHub
- Confirme seu email

### 2️⃣ Prepare o arquivo ZIP
- Compacte a pasta `periodiza-pro` inteira em um arquivo ZIP
- No Mac: clique com botão direito → "Comprimir"
- No Windows: botão direito → "Enviar para" → "Pasta compactada"

### 3️⃣ Faça o deploy
- Entre em https://vercel.com/new
- Clique em **"Import Third-Party Git Repository"** — NÃO, use o botão mais embaixo
- Procure por **"Deploy without Git"** ou arraste o ZIP na tela
- Se pedir configurações:
  - **Framework Preset:** Vite
  - **Build Command:** `npm run build` (já vem preenchido)
  - **Output Directory:** `dist` (já vem preenchido)
- Clique em **Deploy**

### 4️⃣ Aguarde 1-2 minutos
- A Vercel faz tudo sozinha: instala dependências, gera os arquivos, publica
- Ao final, você recebe uma URL tipo `periodiza-pro-abc123.vercel.app`

### 5️⃣ Instale no iPhone
- Abra a URL no **Safari do iPhone**
- Toque no botão **Compartilhar** (quadrado com seta ⬆️ na barra inferior)
- Role as opções → **"Adicionar à Tela de Início"**
- Toque em **"Adicionar"**
- ✅ **Pronto!** Ícone verde-lima **PP** na sua tela de início

### 6️⃣ Teste offline
- Abra o app pelo ícone
- Ative modo avião no iPhone
- O app continua funcionando normalmente 🎉

---

## 🔗 Alternativa simples — Netlify Drop

Se a Vercel parecer complicada, use o **Netlify Drop**:

1. Primeiro você precisa gerar a pasta `dist` uma vez:
   - No computador, abra o terminal na pasta `periodiza-pro`
   - Rode: `npm install` (aguarde 1 min)
   - Rode: `npm run build` (aguarde ~30s)
   - Pronto, a pasta `dist` foi criada

2. Acesse https://app.netlify.com/drop

3. Arraste a pasta `dist` (apenas ela, não a `periodiza-pro`) para a tela

4. Recebe URL instantânea tipo `adorable-cat-123.netlify.app`

5. Instale no iPhone do mesmo jeito descrito acima

---

## 💡 Dicas importantes

**Usar URL personalizada**
- Vercel e Netlify permitem domínios gratuitos tipo `seunome.vercel.app`
- Configure em **Settings → Domains** do painel

**Atualizar o app depois**
- Se encontrar algum ajuste depois de publicar:
- Na Vercel: faça novo upload do ZIP atualizado
- Seus usuários recebem a atualização automaticamente na próxima abertura

**Backup dos dados**
- Oriente os atletas a exportar backup semanalmente pela aba "Backup"
- Safe storage: iCloud Drive para usuários Apple

---

## ❓ Ajuda

Se travar em algum passo, me chame com o erro exato que aparece e eu te guio!
