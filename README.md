# Seu Negócio Aqui - Sistema de Vendas 100% Grátis

Um sistema completo de vendas para pequenos varejistas brasileiros, com **todas as funções liberadas gratuitamente** - sem planos pagos, sem limites.

## 🚀 Funcionalidades

### 📊 Dashboard
- Visão geral de vendas do dia, semana e mês
- Gráfico de vendas dos últimos 14 dias
- Produtos mais vendidos
- Alertas de estoque baixo e zerado
- Resumo de despesas e contas a receber

### 🧾 PDV (Ponto de Venda)
- Venda rápida no balcão
- Busca por nome, SKU ou código de barras
- Scanner de código de barras (câmera)
- Carrinho com controle de quantidade
- Múltiplas formas de pagamento: Dinheiro, Pix, Cartão (crédito/débito), Boleto, Fiado, Link
- Cálculo automático de troco
- Parcelamento em até 12x
- Registro de cliente (opcional)
- Impressão de comprovante
- Baixa automática de estoque

### 📦 Produtos
- Cadastro completo com foto, descrição, preço e custo
- Controle de estoque com estoque mínimo
- Variações de produto (cor, tamanho, modelo)
- Categorias personalizáveis
- SKU e código de barras
- Ativar/desativar produtos
- Geração de descrição com IA
- Busca e filtros avançados

### 💰 Vendas
- Histórico completo de vendas
- Filtros por data e status
- Detalhes do pedido com itens
- Alteração de status (concluída, pendente, cancelada)
- Cancelamento com reposição de estoque
- Total filtrado em tempo real

### 👥 Clientes
- Cadastro de clientes com dados completos
- Controle de fiado (crédito)
- Limite de crédito por cliente
- Saldo atual de cada cliente
- Registro de pagamentos recebidos
- Envio de cobrança via WhatsApp
- Busca por nome, telefone ou email

### 💸 Despesas
- Cadastro de despesas e contas a pagar
- Categorias personalizáveis
- Controle de pagamento (pago/pendente)
- Data de vencimento
- Filtros por status
- Resumo de despesas pagas e pendentes

### 📈 Relatórios
- Receita total e lucro
- Ticket médio
- Vendas por forma de pagamento
- Vendas por canal (PDV, WhatsApp, Instagram, Catálogo)
- Evolução de vendas por dia
- Margem de lucro
- Filtro por período
- Impressão de relatório

### 🌐 Catálogo Online
- Loja virtual pública com link personalizado
- Design responsivo e bonito
- Busca e filtros de categoria
- Carrinho de compras
- Checkout via WhatsApp
- Compartilhamento fácil (link, WhatsApp)
- Personalização de cores e logo
- Prévia do catálogo no admin

### ⚙️ Configurações
- Dados da loja (nome, descrição, contato)
- WhatsApp e Instagram
- Endereço e telefone
- Cor personalizada
- Chave Pix
- Logo da loja

## 🛠️ Tecnologias

- **Frontend**: Next.js 16 (App Router), React 19, TypeScript
- **Estilização**: Tailwind CSS 4
- **Backend**: Next.js API Routes
- **Banco de Dados**: PostgreSQL
- **ORM**: Drizzle ORM
- **UI/UX**: Design moderno e responsivo

## 📦 Instalação

```bash
# Instalar dependências
npm install

# Configurar variáveis de ambiente
cp .env.example .env
# Edite o .env com suas configurações do PostgreSQL

# Aplicar migrations do banco
npx drizzle-kit push

# Rodar em desenvolvimento
npm run dev

# Build de produção
npm run build
npm start
```

## 🗄️ Banco de Dados

O sistema cria automaticamente as seguintes tabelas:

- `store` - Configurações da loja
- `categories` - Categorias de produtos
- `products` - Produtos
- `product_variations` - Variações de produtos (cor, tamanho, etc)
- `customers` - Clientes
- `sales` - Vendas
- `sale_items` - Itens das vendas
- `expenses` - Despesas
- `customer_payments` - Pagamentos de fiado

## 🎯 Diferenciais do Seu Negócio Aqui vs outros sistemas pagos

| Funcionalidade | Sistemas Pagos | Seu Negócio Aqui |
|----------------|----------------|------------------|
| Catálogo online | Limitado no plano grátis | ✅ **Ilimitado e grátis** |
| Produtos | Limite no plano grátis | ✅ **Ilimitado** |
| Variações de produto | Pago | ✅ **Grátis** |
| PDV completo | Limitado | ✅ **Completo e grátis** |
| Controle de fiado | Pago | ✅ **Grátis** |
| Relatórios avançados | Pago | ✅ **Grátis** |
| Scanner de código de barras | Pago | ✅ **Grátis** |
| Catálogo público com link | Pago | ✅ **Grátis** |
| Checkout via WhatsApp | Pago | ✅ **Grátis** |
| IA para descrições | Limitado | ✅ **Ilimitado** |
| Impressão de recibos | Pago | ✅ **Grátis** |
| Múltiplos usuários | Pago | ✅ **Grátis** |
| **Preço** | R$ 49-199/mês | ✅ **100% GRÁTIS** |

## 📱 Uso Mobile

O sistema é totalmente responsivo e funciona perfeitamente em:
- 💻 Desktop
- 📱 Tablet
- 📲 Celular

Use como PWA (Progressive Web App) adicionando à tela inicial do seu celular.

## 🔐 Segurança

- Senhas e chaves API armazenadas em variáveis de ambiente
- Validação de dados no frontend e backend
- Proteção contra SQL injection (Drizzle ORM)
- Sanitização de inputs

## 🎨 Personalização

O sistema permite personalizar:
- Nome e descrição da loja
- Logo
- Cor principal do catálogo
- Dados de contato (WhatsApp, Instagram, telefone)
- Chave Pix
- Categorias de produtos
- Categorias de despesas

## 📊 Dados de Demonstração

Ao iniciar pela primeira vez, o sistema cria automaticamente:
- Loja de exemplo
- 6 categorias
- 6 produtos de demonstração
- 3 clientes
- 4 despesas de exemplo

Você pode editar ou excluir tudo e começar do zero.

## 🚀 Deploy

### Vercel (Recomendado)
```bash
npm install -g vercel
vercel
```

### Docker
```bash
docker build -t stoqui-clone .
docker run -p 3000:3000 stoqui-clone
```

### VPS/Servidor Próprio
```bash
npm run build
npm start
```

## 🤝 Contribuindo

Este é um projeto open source. Contribuições são bem-vindas!

## 📄 Licença

MIT License - Use livremente para fins pessoais e comerciais.

## 🎉 Comece Agora!

Acesse o sistema, configure sua loja em **Configurações** e comece a vender!

Todas as funções são 100% gratuitas, sem limites, sem mensalidade.

---

**Feito com ❤️ para pequenos empreendedores brasileiros**
