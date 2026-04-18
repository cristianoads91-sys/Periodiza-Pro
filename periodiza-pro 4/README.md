# Periodiza Pro ⚡

App PWA de periodização científica de treinamento esportivo.

Funciona **100% offline** após instalação. Compatível com iPhone, iPad, Android, MacBook e qualquer navegador moderno.

---

## 🚀 Como publicar (3 opções — escolha UMA)

### Opção A — Vercel (mais fácil, recomendado) ⭐

1. Crie conta grátis em https://vercel.com (pode logar com GitHub, Google ou email)
2. Na tela inicial, clique em **"Add New... → Project"**
3. Arraste a pasta inteira `periodiza-pro` ou faça upload do `.zip`
4. A Vercel detecta **Vite** automaticamente e clica em **"Deploy"**
5. Em ~1 minuto você recebe uma URL tipo `https://periodiza-pro.vercel.app`
6. **Pronto!** Acesse essa URL no Safari do iPhone.

### Opção B — Netlify

1. Acesse https://app.netlify.com/drop
2. Primeiro rode no seu computador: `npm install && npm run build`
3. Arraste a pasta `dist` gerada para a tela do Netlify
4. Recebe URL tipo `https://periodiza-pro.netlify.app`

### Opção C — Rodar localmente (desenvolvimento)

```bash
npm install
npm run dev       # modo desenvolvedor com hot reload
npm run build     # gera pasta dist/ pronta para produção
npm run preview   # testa a build antes de publicar
```

---

## 📱 Como instalar no iPhone/iPad

1. Abra a URL no **Safari** (precisa ser o Safari, não Chrome no iOS)
2. Toque no botão de **compartilhar** (ícone ⬆️ na barra inferior)
3. Role e toque em **"Adicionar à Tela de Início"**
4. Confirme com **"Adicionar"**

O app aparece com o ícone **PP** verde-lima na sua tela de início. Ao abrir:
- ✅ **Tela cheia**, sem barras do Safari
- ✅ **Funciona offline** — pode desligar o Wi-Fi/4G
- ✅ **Todos os dados ficam salvos** no dispositivo
- ✅ **Atualiza sozinho** quando você melhora o app (na próxima abertura online)

---

## 💻 Como instalar no MacBook

1. Abra a URL no **Safari** (versão 17+)
2. Menu superior: **Arquivo → Adicionar ao Dock...**
3. Confirme.

Ou no **Chrome/Edge**: clique no ícone de instalar na barra de endereço (aparece automaticamente).

---

## 🔄 Como atualizar o app depois de publicado

1. Modifique o código (principalmente `src/App.jsx`)
2. Faça novo deploy na Vercel (ela detecta automaticamente se você conectou GitHub)
   - OU rode `npm run build` e arraste `dist/` de novo
3. Na próxima vez que o usuário abrir o app, ele atualiza sozinho em background
4. Os **dados salvos não são perdidos** na atualização (ficam no localStorage do dispositivo)

---

## 💾 Backup dos dados

Os dados são salvos **localmente** no dispositivo. Para migrar entre aparelhos ou fazer backup:

1. Abra o app → aba **Backup**
2. Toque em **"Exportar Backup Agora"**
3. Salve o arquivo JSON no iCloud Drive ou envie via AirDrop
4. No outro aparelho: Backup → **"Importar Arquivo"**

---

## 📂 Estrutura do projeto

```
periodiza-pro/
├── package.json           # Dependências do projeto
├── vite.config.js         # Configuração do Vite + PWA
├── index.html             # HTML principal com meta tags iOS
├── src/
│   ├── main.jsx           # Entry point React
│   └── App.jsx            # Código completo do app
└── public/
    ├── icon-192.png       # Ícone PWA (Android/desktop)
    ├── icon-512.png       # Ícone PWA grande
    ├── apple-touch-icon.png  # Ícone iOS (na tela de início)
    └── favicon.svg        # Favicon para navegador
```

---

## 🎨 Personalização

- **Cores da marca**: edite o objeto `C` no topo de `src/App.jsx`
- **Ícones**: substitua os arquivos em `public/`
- **Nome do app**: edite em `vite.config.js` (manifest) e `index.html` (meta tags)

---

## ❓ Problemas comuns

**"O app não aparece a opção de instalar no Safari"**
→ Verifique se o site está em HTTPS (Vercel/Netlify fazem automaticamente). PWAs não funcionam em HTTP.

**"Os dados sumiram"**
→ Safari pode limpar dados de sites não visitados por 7+ dias. Solução: use o app pelo menos uma vez por semana OU sempre exporte backup semanalmente.

**"O ícone não aparece na tela de início"**
→ Certifique-se de ter clicado "Adicionar" no Safari, não em outro navegador. Para Android, use o Chrome.

---

## 📚 Base científica

Aplicativo fundamentado em:

- Verkhoshansky, Y. (1985, 2009) — Sistema de Blocos Concentrados, RFD
- Matveev, L. (1964, 1977) — Teoria da Periodização
- Bompa, T. (1999) — Periodização moderna
- ACSM (2009) — Diretrizes de prescrição de exercício
- Gomes, A. C. (2009) — Aplicação brasileira de periodização

Escalas psicofisiológicas:
- Borg, G. (1962) / Foster, C. (1998) — PSE/CR-10
- Kenttä & Hassmén (1998) — PSR
- Hooper & Mackinnon (1995) — Índice de bem-estar

---

**Versão 1.0 — 2026**
