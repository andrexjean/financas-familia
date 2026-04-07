# Finanças · Família Oliveira

Sistema de gestão financeira familiar — seguro, offline-first, sem custos.

---

## Segurança — 3 camadas

1. **Gate** — código pedido antes de qualquer coisa (padrão: `Familia@2026`)
2. **Login** — senha do sistema com criptografia AES-256 (padrão: `Oliveira2026`)
3. **Dados** — armazenados criptografados no dispositivo, nunca em servidor

**Troque ambos imediatamente após instalar** em Configurações.

---

## Como atualizar o sistema (substituir index.html no GitHub)

1. Acesse github.com → seu repositório `financas-familia`
2. Clique no arquivo `index.html` → ícone de lápis (editar)
3. Selecione todo o conteúdo (Ctrl+A) e delete
4. Cole o novo conteúdo do arquivo atualizado
5. Clique em "Commit changes" → pronto

OU use o botão de upload: clique no ícone da lixeira para deletar o arquivo antigo, depois faça upload do novo.

---

## Configurar Google Drive — backup automático

### Passo 1 — Google Cloud Console
1. Acesse: https://console.cloud.google.com (login com sua conta Google)
2. Topo → "Selecionar projeto" → "Novo projeto"
3. Nome: `FinancasFamilia` → Criar

### Passo 2 — Ativar API do Drive
1. Menu → "APIs e serviços" → "Biblioteca"
2. Pesquise `Google Drive API` → Ativar

### Passo 3 — Tela de consentimento OAuth
1. Menu → "APIs e serviços" → "Tela de consentimento OAuth"
2. Tipo: **Externo** → Criar
3. Nome: `Financas Familia` · email: seu email → Salvar e continuar
4. Na etapa "Usuários de teste" → Adicionar → coloque seu email E o da Bruna

### Passo 4 — Criar credencial
1. Menu → "APIs e serviços" → "Credenciais"
2. "+ Criar credenciais" → "ID do cliente OAuth"
3. Tipo: **Aplicativo da Web** · Nome: `Financas`
4. Origens JavaScript autorizadas: `https://andrexjean.github.io`
5. URIs de redirecionamento: `https://andrexjean.github.io/financas-familia/`
6. Criar → **copie o Client ID** (termina em `.apps.googleusercontent.com`)

### Passo 5 — Conectar no sistema
1. Abra o sistema → ⚙ Configurações
2. Clique "Conectar Google Drive" → cole o Client ID
3. Autorize com sua conta Google
4. Pronto — backup automático após cada salvamento!

---

## Usar todo mês

1. Gate → Login
2. Aba Importar → selecione o mês → upload dos arquivos → Processar → Salvar
3. Backup vai automaticamente para o Google Drive

---

## Instalar como app no celular

**Android:** Chrome → menu 3 pontinhos → "Adicionar à tela inicial"
**iPhone:** Safari → botão compartilhar → "Adicionar à tela de início"
