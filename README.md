# SOMALIG - Landing Page

Landing page da SOMALIG, empresa especializada em soluções de consórcio.

## 🚀 Deploy na Vercel

### Opção 1: Deploy via GitHub (Recomendado)

1. **Faça upload do projeto para o GitHub:**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/seu-usuario/somalig-landing-page.git
   git push -u origin main
   ```

2. **Conecte com a Vercel:**
   - Acesse [vercel.com](https://vercel.com)
   - Faça login com sua conta GitHub
   - Clique em "New Project"
   - Selecione o repositório `somalig-landing-page`
   - Clique em "Deploy"

### Opção 2: Deploy direto via Vercel CLI

1. **Instale a Vercel CLI:**
   ```bash
   npm i -g vercel
   ```

2. **Faça login:**
   ```bash
   vercel login
   ```

3. **Deploy:**
   ```bash
   vercel
   ```

## 📁 Estrutura do Projeto

```
somalig-landing-page/
├── index.html          # Página principal
├── package.json        # Dependências do projeto
├── vercel.json         # Configuração da Vercel
├── README.md           # Este arquivo
└── assets/             # Pasta para imagens (se houver)
```

## 🖼️ Imagens

**Importante:** Certifique-se de que todas as imagens referenciadas no HTML estejam na pasta do projeto:

- `Logo teste.png` - Logo principal
- `logo.png` - Logo alternativo
- `happy-family-celebration.png` - Imagem do herói
- Imagens dos depoimentos (se houver)

## 🔧 Configurações

- **Framework:** HTML estático com Tailwind CSS
- **Build:** Não requer build - deploy direto
- **Domínio:** A Vercel fornecerá um domínio `.vercel.app`

## 📱 Responsividade

A página é totalmente responsiva e funciona em:
- Desktop
- Tablet
- Mobile

## 🚀 Comandos Locais

```bash
# Instalar dependências
npm install

# Rodar localmente
npm run dev

# Build (não necessário para este projeto)
npm run build
```

## 📞 Suporte

Para dúvidas sobre o deploy, consulte a [documentação da Vercel](https://vercel.com/docs).
