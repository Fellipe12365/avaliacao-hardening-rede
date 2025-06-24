# Avaliação de Risco de Segurança – Hardening de Rede

## 📌 Cenário

A organização de mídia social onde atuo como analista de segurança sofreu recentemente uma **grande violação de dados**, expondo informações pessoais de clientes, como nomes e endereços. Após uma análise da rede, foram identificadas quatro vulnerabilidades principais:

- Compartilhamento de senhas entre funcionários
- Senha de administrador do banco de dados definida como padrão
- Firewalls sem regras de filtragem de tráfego
- Ausência de autenticação multifatorial (MFA)

Para mitigar essas falhas, foram selecionadas e implementadas práticas de **hardening de rede** com o objetivo de reforçar a segurança da infraestrutura e prevenir futuras violações.

---

## ✅ Parte 1: Ferramentas e Métodos de Hardening Selecionados

1. **Política de gerenciamento de senhas com autenticação multifator (MFA)**
2. **Configuração e atualização de regras de firewall**
3. **Remoção de senhas padrão e aplicação do princípio do menor privilégio**

---

## 🛡️ Parte 2: Explicação das Recomendações

### 1. Política de Gerenciamento de Senhas com MFA

**🔐 Vulnerabilidades abordadas:**
- Compartilhamento de senhas
- Ausência de MFA

**✅ Ações:**
- Implementar autenticação multifator (Google Authenticator, Microsoft Authenticator, Duo Security)
- Criar política de senhas fortes e com expiração periódica
- Proibir o compartilhamento de credenciais

**🎯 Benefícios:**
- Protege contas mesmo se senhas forem vazadas
- Reduz drasticamente acessos não autorizados
- Melhora a cultura de segurança organizacional

---

### 2. Configuração de Regras de Firewall

**🔥 Vulnerabilidade abordada:**
- Firewalls sem regras de controle de tráfego

**✅ Ações:**
- Definir regras de entrada e saída com base em portas, IPs e protocolos
- Aplicar política de "tudo negado por padrão" e permitir apenas o necessário
- Utilizar firewalls com inspeção profunda de pacotes (DPI) e geração de logs

**🎯 Benefícios:**
- Bloqueia tráfego malicioso antes que alcance os sistemas
- Reduz a superfície de ataque da rede
- Permite auditoria e resposta rápida a incidentes

---

### 3. Remoção de Senhas Padrão e Princípio do Menor Privilégio

**🔑 Vulnerabilidade abordada:**
- Senha padrão do banco de dados

**✅ Ações:**
- Alterar todas as senhas padrão imediatamente
- Usar gerenciadores de senhas
- Ajustar permissões com base em funções e necessidades reais

**🎯 Benefícios:**
- Impede uso de credenciais públicas ou conhecidas
- Minimiza o impacto em caso de comprometimento de contas
- Garante que usuários só tenham acesso ao necessário

---

## 🧾 Conclusão

A aplicação dessas práticas de hardening oferece uma abordagem robusta e proativa para proteger os ativos da organização. Elas fortalecem os pontos vulneráveis atuais, criam barreiras contra futuros ataques e contribuem para uma cultura de segurança sólida e sustentável.
