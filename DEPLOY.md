# 🚀 Deploy na Vercel - Passo a Passo

## 📋 Pré-requisitos

- Conta no GitHub (gratuita)
- Conta na Vercel (gratuita)

## 🔧 Passo 1: Preparar o Projeto

### 1.1 Organizar arquivos
```
somalig-landing-page/
├── index.html          ✅ Página principal
├── package.json        ✅ Configuração do projeto
├── vercel.json         ✅ Configuração da Vercel
├── public/             ✅ Pasta com imagens
│   ├── logo.png
│   └── logo-teste.png
├── README.md           ✅ Documentação
└── .gitignore          ✅ Arquivos ignorados
```

### 1.2 Verificar imagens
- ✅ `public/logo.png` - Logo principal
- ✅ `public/logo-teste.png` - Logo alternativo
- ❌ `happy-family-celebration.png` - **FALTANDO** (imagem do herói)
- ❌ Imagens dos depoimentos - **FALTANDO**

## 🚀 Passo 2: Deploy via GitHub (Recomendado)

### 2.1 Criar repositório no GitHub
1. Acesse [github.com](https://github.com)
2. Clique em "New repository"
3. Nome: `somalig-landing-page`
4. Descrição: `Landing page da SOMALIG - Soluções de Consórcio`
5. Público ou Privado (sua escolha)
6. **NÃO** inicialize com README (já temos um)
7. Clique em "Create repository"

### 2.2 Fazer upload do projeto
```bash
# No terminal, na pasta do projeto
git init
git add .
git commit -m "Initial commit: Landing page SOMALIG"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/somalig-landing-page.git
git push -u origin main
```

### 2.3 Deploy na Vercel
1. Acesse [vercel.com](https://vercel.com)
2. Faça login com sua conta GitHub
3. Clique em "New Project"
4. Selecione o repositório `somalig-landing-page`
5. Clique em "Deploy"

## 🔧 Passo 3: Deploy via Vercel CLI (Alternativo)

### 3.1 Instalar Vercel CLI
```bash
npm install -g vercel
```

### 3.2 Fazer login
```bash
vercel login
```

### 3.3 Deploy
```bash
vercel
```

## ⚠️ Problemas Comuns e Soluções

### ❌ Imagem não encontrada
**Problema:** `404` para imagens
**Solução:** Verificar se as imagens estão na pasta `public/` e se os caminhos estão corretos

### ❌ CSS não carrega
**Problema:** Tailwind CSS não funciona
**Solução:** O Tailwind está sendo carregado via CDN, deve funcionar automaticamente

### ❌ JavaScript não funciona
**Problema:** Funções não respondem
**Solução:** Verificar se não há erros no console do navegador

## 🌐 Após o Deploy

### URL fornecida pela Vercel
- Formato: `https://somalig-landing-page-XXXX.vercel.app`
- Você pode personalizar o domínio nas configurações

### Configurações adicionais
1. **Domínio personalizado** (se tiver)
2. **HTTPS** (automático)
3. **Cache** (configurado automaticamente)

## 📱 Teste

### Testar em diferentes dispositivos
- ✅ Desktop
- ✅ Tablet
- ✅ Mobile

### Funcionalidades a verificar
- ✅ Navegação entre páginas
- ✅ Modal de simulação
- ✅ Carrossel de produtos
- ✅ Formulário de contato
- ✅ WhatsApp button
- ✅ Responsividade

## 🔄 Atualizações

### Para atualizar o site
```bash
git add .
git commit -m "Update: descrição da mudança"
git push origin main
```
A Vercel fará deploy automático!

## 📞 Suporte

- **Vercel Docs:** [vercel.com/docs](https://vercel.com/docs)
- **GitHub Docs:** [docs.github.com](https://docs.github.com)

---

**🎯 Próximo passo:** Fazer upload das imagens que estão faltando para a pasta `public/`
