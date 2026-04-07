# Finanças · Família Oliveira

Sistema de gestão financeira familiar — seguro, offline-first, sem custos.

## Como publicar (passo a passo)

### 1. Criar conta no GitHub (gratuito)
- Acesse https://github.com e crie uma conta
- É gratuito e não precisa de cartão

### 2. Criar repositório
- Clique em "New repository"
- Nome: `financas-familia` (ou qualquer nome)
- Marque como **Private** (privado — só você vê)
- Clique em "Create repository"

### 3. Fazer upload dos arquivos
- Na página do repositório, clique em "uploading an existing file"
- Arraste todos os arquivos desta pasta:
  - `index.html`
  - `sw.js`
  - `manifest.json`
- Clique em "Commit changes"

### 4. Ativar GitHub Pages
- Vá em Settings → Pages
- Source: "Deploy from a branch"
- Branch: main → / (root)
- Clique em Save
- Em ~2 minutos o site estará em: `https://seu-usuario.github.io/financas-familia`

### 5. Acessar no celular
- Abra a URL no Chrome do celular
- Toque no menu (3 pontos) → "Adicionar à tela inicial"
- O app aparece como ícone nativo no celular

---

## Segurança

### Como funciona
- **Criptografia AES-256-GCM** com PBKDF2 (200.000 iterações)
- Os dados ficam **apenas no seu dispositivo** (localStorage criptografado)
- Nenhum dado vai para servidores — nem para o GitHub
- O GitHub Pages serve apenas o código HTML (sem acesso aos dados)

### Senha padrão
A senha inicial é: **Oliveira2026**
**Troque imediatamente** em Configurações → Trocar senha

### Sincronização entre dispositivos
Como os dados ficam locais, para sincronizar entre computador e celular:
1. No dispositivo principal, vá em Configurações → Exportar backup
2. Salve o arquivo `.fo-backup` no Google Drive
3. No outro dispositivo, abra o arquivo do Drive e use Configurações → Restaurar backup
4. Faça isso mensalmente após registrar os dados

### Backup
- Exporte o backup mensalmente após lançar os dados
- O arquivo `.fo-backup` é criptografado — só abre com sua senha
- Salve no Google Drive para não perder

---

## Como usar mensalmente

1. **Acesse o sistema** e entre com sua senha
2. Vá na aba **Importar**
3. Selecione o mês de referência
4. **Faça upload** dos arquivos:
   - Fatura HTML do cartão (Nubank/XP)
   - Relatório XP em PDF ou Excel
   - Extrato Bradesco em PDF (imóvel/carro)
5. Clique em **Processar arquivos**
6. **Confirme os custos fixos** do mês (ajuste se algo mudou)
7. Clique em **Salvar dados do mês**
8. Veja o **Dashboard** atualizado
9. Exporte o backup e salve no Google Drive

---

## Funcionalidades

- Login com senha e criptografia AES-256
- Dashboard com KPIs atualizados a cada mês
- Importação de faturas HTML, PDF, Excel
- Custos fixos editáveis mês a mês
- Evolução patrimonial em gráficos
- Análise de gastos vs metas por categoria
- Alertas automáticos de desvios
- Marcos financeiros (dívidas, quitações)
- Backup criptografado exportável
- PWA instalável no celular
- Funciona offline após primeiro acesso

---

## Dados pré-carregados (Abril/2026)

- Patrimônio líquido: R$ 202.900
- Investimentos: R$ 70.330 (XP + Nubank)
- Gastos cartão: R$ 10.744
- Imóvel: saldo R$ 239.290 · parcela R$ 2.358
- Carro: saldo R$ 61.140 · parcela R$ 2.447
- Renda fixa: R$ 15.000 | Comissão: ~R$ 5.000
