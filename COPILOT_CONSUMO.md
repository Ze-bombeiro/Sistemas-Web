# Como Encontrar o Consumo do GitHub Copilot

Este documento explica onde encontrar informações sobre o uso e consumo do GitHub Copilot.

## 📊 Para Contas Individuais

### 1. Acessar as Configurações da Conta
1. Faça login no GitHub.com
2. Clique na sua foto de perfil no canto superior direito
3. Selecione **"Settings"** (Configurações)

### 2. Visualizar Cobrança e Uso
1. No menu lateral esquerdo, clique em **"Billing and plans"** (Cobrança e planos)
2. Na seção **"Plans and usage"** (Planos e uso), você encontrará:
   - **Subscription details** (Detalhes da assinatura)
   - **Usage this month** (Uso este mês)
   - **Billing history** (Histórico de cobrança)

### 3. Detalhes do Copilot Individual
- **Preço**: $10/mês ou $100/ano
- **Tipo de cobrança**: Por usuário
- **Trial gratuito**: 30 dias para novos usuários

## 🏢 Para Organizações (Copilot Business)

### 1. Configurações da Organização
1. Vá para a página da sua organização no GitHub
2. Clique na aba **"Settings"** (Configurações)
3. No menu lateral, selecione **"Billing and plans"** (Cobrança e planos)

### 2. Métricas de Uso
Na página de cobrança, você encontrará:
- **Total de licenças ativas**
- **Custo mensal atual**
- **Histórico de uso por usuário**
- **Relatórios de atividade**

### 3. Detalhes do Copilot Business
- **Preço**: $19/usuário/mês
- **Recursos adicionais**:
  - Controles administrativos
  - Auditoria e compliance
  - Suporte prioritário

## 📈 Métricas de Uso Disponíveis

### Informações que você pode acompanhar:
- **Sugestões aceitas**: Número de sugestões do Copilot aceitas
- **Sugestões mostradas**: Total de sugestões apresentadas
- **Taxa de aceitação**: Percentual de sugestões aceitas
- **Linguagens mais usadas**: Quais linguagens você mais usa com Copilot
- **Tempo economizado**: Estimativa de tempo poupado

## 🔗 Links Diretos

### Para Usuários Individuais:
- Configurações de cobrança: `https://github.com/settings/billing`
- Configurações do Copilot: `https://github.com/settings/copilot`

### Para Organizações:
- Configurações de cobrança: `https://github.com/organizations/[ORG-NAME]/settings/billing`
- Configurações do Copilot: `https://github.com/organizations/[ORG-NAME]/settings/copilot`

*Substitua `[ORG-NAME]` pelo nome da sua organização*

## 📱 Através da API

Para desenvolvedores que querem acessar dados programaticamente:

```bash
# Ver uso do Copilot (requer autenticação)
curl -H "Authorization: token YOUR_TOKEN" \
     -H "Accept: application/vnd.github.v3+json" \
     https://api.github.com/copilot/billing

# Ver métricas da organização
curl -H "Authorization: token YOUR_TOKEN" \
     -H "Accept: application/vnd.github.v3+json" \
     https://api.github.com/orgs/YOUR_ORG/copilot/billing
```

## ❓ Perguntas Frequentes

**P: Posso ver o uso de outros desenvolvedores na minha organização?**
R: Sim, administradores da organização podem ver métricas de uso de todos os membros.

**P: Os dados de uso são em tempo real?**
R: Os dados são atualizados diariamente, não em tempo real.

**P: Posso exportar os dados de uso?**
R: GitHub fornece relatórios que podem ser baixados em formato CSV.

**P: Como cancelo minha assinatura?**
R: Vá em Settings > Billing and plans > Manage subscription > Cancel subscription.

## 🆘 Suporte

Se você não conseguir encontrar as informações de uso:
1. Verifique se você tem as permissões adequadas
2. Entre em contato com o suporte do GitHub
3. Consulte a documentação oficial: https://docs.github.com/copilot

---
*Documento criado para ajudar usuários a encontrar informações sobre consumo do GitHub Copilot*