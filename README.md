# resumo-do-lab-DIO-AZ900
Este repositório contém o resumo das lições aprendidas durante o desenvolvimento do lab na DIO
Este repositório contém meu resumo do curso de **Fundamentos do Azure (AZ-900)** oferecido pela DIO.  
Até o momento, tivemos a introdução ao conceito de computação em nuvem e uma visão geral da plataforma Microsoft Azure.

---

## Conceitos aprendidos

# Microsoft AZ-900 – Anotações

## Computação em Nuvem
- **Definição**: fornecimento de serviços de computação pela internet, habilitando inovações mais rápidas, recursos flexíveis e economias de escala.  
- É a **virtualização dos serviços de informática**.

### Modelos de Nuvem
- **Nuvem Privada (on premise):** ambiente em nuvem no datacenter da empresa; toda responsabilidade é da organização.  
  - Responsável por hardware, software, atualizações e upgrades.  
  - Usuários externos não têm acesso.  
- **Nuvem Pública:** um provedor fornece os recursos via rede.  
  - Nenhuma despesa de capital para escalar verticalmente.  
  - Aplicativos podem ser provisionados e desprovisionados rapidamente.  
  - Paga-se somente pelo que for utilizado.  
- **Nuvem Híbrida:** conecta recursos de nuvem privada e pública.  
  - Flexibilidade para decidir onde executar aplicativos.  
  - Controle de segurança e conformidade legal.  

### CapEx x OpEx
- **CapEx (Capital Expenditure):** investimento inicial em infraestrutura física. O valor se deprecia com o tempo.  
- **OpEx (Operational Expenditure):** pagamento por produtos/serviços conforme necessidade; modelo de pagamento por uso.  

### Modelo baseado em consumo
- Paga apenas pelos recursos usados.  
- Melhora a previsão de custos.  
- Preços fornecidos por recurso individual.  

### Outros conceitos
- **Jump server:** servidor intermediário.  
- **Versões prévias:** versões em testes; usar com cautela.  

---

## Benefícios da Nuvem
- **Alta disponibilidade:** garantia contratual de funcionamento com crédito em caso de falha.  
- **Escalabilidade:** ajuste da capacidade conforme demanda (mais ou menos recursos).  
- **Elasticidade:** ajuste dinâmico dos recursos por picos de uso (ex.: Black Friday).  
- **Confiabilidade:** resiliência a falhas, com recursos distribuídos em múltiplos locais.  
- **Previsibilidade:** clareza nos recursos e custos.  
- **Segurança:** ferramentas fornecidas pela plataforma, mas responsabilidade de configuração é do cliente.  
- **Governança:** aplicação de padrões, auditorias e conformidade com políticas.  
- **Gerenciabilidade:** várias formas de gestão (portal, CLI, APIs, PowerShell).  

---

## Tipos de Serviço de Nuvem
- **IaaS (Infraestrutura como Serviço):** você gerencia SO, aplicativos e dados; provedor cuida da infraestrutura.  
- **PaaS (Plataforma como Serviço):** você gerencia apenas aplicativos e dados; provedor cuida do resto.  
- **SaaS (Software como Serviço):** uso direto do aplicativo final (ex.: Office 365, Netflix).  

---

## Alta Disponibilidade no Azure
- **Domínio de falhas (Fault Domain):** protege contra falhas físicas de hardware.  
- **Domínio de atualização (Update Domain):** protege contra reinícios em atualizações planejadas.  

---

## Modelo de Responsabilidade Compartilhada
O provedor e o cliente dividem responsabilidades de segurança e gestão.  

---

## Regiões e Disponibilidade
- **Regiões:** +60 regiões em 140 países, compostas por um ou mais datacenters próximos.  
- **Pares de região:** cada região tem uma região par para recuperação de desastres.  
- **Zonas de disponibilidade:** fornecem redundância dentro da mesma região.  
- **Regiões soberanas:** usadas apenas por governos (ex.: EUA, militar).  
- **China:** operada pela 21Vianet, seguindo leis locais.  

---

## Recursos e Organização
- **Recursos do Azure:** componentes como VMs, redes e storage.  
- **Grupo de recursos:** organiza recursos relacionados; um recurso só pode estar em um grupo.  
- **Assinaturas:** vinculadas a contas; definem limites de cobrança e gestão.  
- **Grupos de gerenciamento:** agregam múltiplas assinaturas para aplicar regras e governança. 

---

## Próximos passos
Continuar os estudos aprofundando os principais serviços do Azure (computação, rede, armazenamento e segurança), além de explorar a prática na plataforma.  

---
*Resumo pessoal de estudos para apoiar a certificação **AZ-900 Microsoft Azure Fundamentals***  
