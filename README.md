# resumo-do-lab-DIO-AZ900  

Este repositório contém o resumo das lições aprendidas durante o desenvolvimento do lab na DIO.  
Este repositório contém meu resumo do curso de **Fundamentos do Azure (AZ-900)** oferecido pela DIO.  

Até o momento, tivemos a introdução ao conceito de computação em nuvem e uma visão geral da plataforma Microsoft Azure.  

---

# Microsoft AZ-900 – Resumo  

## Computação em Nuvem  
- **Definição:** fornecimento de serviços de computação pela internet, habilitando inovações rápidas, recursos flexíveis e economias de escala.  
- Virtualização de serviços de informática.  

### Modelos de Nuvem  
- **Privada (On Premise):** ambiente em nuvem no datacenter da empresa; responsabilidade total da organização.  
- **Pública:** provedor fornece recursos via rede; escalabilidade sem investimento em infraestrutura; pagamento conforme uso.  
- **Híbrida:** integração entre nuvem privada e pública; maior flexibilidade e conformidade legal.  

### CapEx x OpEx  
- **CapEx:** despesas de capital em infraestrutura física, depreciáveis ao longo do tempo.  
- **OpEx:** despesas operacionais, pagamento conforme uso.  

### Modelo baseado em consumo  
- Pagamento somente pelos recursos usados.  
- Melhor previsão de custos.  

### Outros conceitos  
- **Jump Server:** servidor intermediário.  
- **Versões Prévias:** recursos em teste, usar com cautela.  

---

## Benefícios da Nuvem  
- **Alta disponibilidade:** funcionamento garantido com créditos em caso de falha.  
- **Escalabilidade:** ajuste de recursos conforme demanda.  
- **Elasticidade:** ajuste dinâmico para picos de uso.  
- **Confiabilidade:** resiliência e recursos distribuídos.  
- **Previsibilidade:** clareza de custos e recursos.  
- **Segurança:** ferramentas fornecidas pela Microsoft; implementação pelo cliente.  
- **Governança:** padrões, auditorias e conformidade.  
- **Gerenciabilidade:** gerenciamento via portal, CLI, API ou PowerShell.  

---

## Tipos de Serviço de Nuvem  
- **IaaS:** gerenciamento de SO, aplicativos e dados.  
- **PaaS:** provedor gerencia infraestrutura; usuário gerencia apps e dados.  
- **SaaS:** uso direto de aplicativos (ex.: Office 365, Netflix).  

---

## Alta Disponibilidade  
- **Domínio de Falhas:** proteção contra falhas físicas.  
- **Domínio de Atualização:** proteção contra reinícios durante atualizações.  

---

## Regiões e Disponibilidade  
- Mais de **60 regiões em 140 países**.  
- Datacenters próximos reduzem latência.  
- **Pares de Região:** redundância para recuperação de desastres.  
- **Regiões Soberanas:** restritas a governos.  
- **China:** operada pela 21Vianet, conforme leis locais.  
- **Zonas de Disponibilidade:** redundância dentro da mesma região.  

---

## Organização de Recursos  
- **Recursos do Azure:** VMs, storage, redes etc.  
- **Grupo de Recursos:** organiza recursos relacionados.  
- **Assinaturas:** vinculadas a uma conta; definem custos e limites.  
- **Grupos de Gerenciamento:** aplicam políticas a múltiplas assinaturas.  

---

## Computação no Azure  
- **Máquinas Virtuais (VMs):** emulação completa de computadores físicos.  
- **Conjunto de Dimensionamento:** ajuste automático da quantidade/tamanho das VMs.  
- **Conjunto de Disponibilidade:** distribui VMs em domínios de falha/atualização.  
- **Área de Trabalho Virtual (AVD):** desktop Windows na nuvem, pronto para usuários acessarem.  

### Diferença VMs x Área de Trabalho  
- **VMs:** controle total para administradores.  
- **AVD:** desktop pronto, gerenciado pelo Azure para usuários finais.  

---

## Contêineres  
- Execução de aplicativos empacotados com dependências em ambientes isolados.  
- Leves e portáteis; não exigem SO completo.  
- Serviços: **Azure Container Instances (ACI)** e **Azure Kubernetes Service (AKS)**.  
- Oferta PaaS.  

---

## Azure Functions  
- Serviço **serverless**; executa código sob demanda em resposta a eventos.  
- Escalabilidade automática; cobrança apenas pelo uso.  
- Oferta PaaS.  

---

## Serviços de Aplicativos  
- Criação, implantação e dimensionamento de apps web e APIs.  
- Suporte a .NET, Node.js, Java, Python, PHP.  
- Oferta PaaS.  

---

## Serviços de Rede  
- **VNet:** rede privada isolada para conectar VMs e serviços.  
- Conexão com redes locais via **VPN** ou **ExpressRoute**.  

### VPN Gateway x ExpressRoute  
- **VPN Gateway:** internet pública, conexões criptografadas.  
- **ExpressRoute:** conexão privada dedicada, alta performance e confiabilidade.  

---

## Armazenamento no Azure  
- **Contas de Armazenamento:** nomes globalmente únicos.  
- **Blob Storage:** grandes volumes de dados não estruturados (textos, imagens, vídeos, backups, logs).  
- **Disk Storage:** discos virtuais de alto desempenho para VMs e aplicativos.  
- **Queue Storage:** filas de mensagens, até 64 KB cada, ideal para comunicação entre componentes.  
- **File Storage:** compartilhamentos de arquivos via SMB, substituindo ou complementando servidores locais.  
- **Table Storage:** dados estruturados em pares chave/atributo, sem esquema fixo.  

### Camadas de Acesso  
- **Frequente:** dados acessados com frequência.  
- **Esporádico:** dados acessados ocasionalmente, armazenados por pelo menos 30 dias.  
- **Frio:** dados raramente acessados, armazenados por pelo menos 90 dias.  
- **Arquivo morto:** dados raramente acessados, armazenados por pelo menos 180 dias.  

---

## Migração e Sincronização  
- **Azure Data Box:** dispositivo físico para migrar grandes volumes de dados de forma segura e rápida, com criptografia.  
- **Data Box Disk:** até 8 TB por disco  
- **Data Box:** até 80 TB por dispositivo  
- **Data Box Heavy:** até 1 PB por dispositivo  
- **AzCopy:** ferramenta CLI para copiar e sincronizar arquivos entre armazenamento local e Azure.  
- **Gerenciador de Armazenamento do Azure:** gerencia Blobs, Files, Queues e Tables de forma prática.  
- **Sincronização de arquivos do Azure:** mantém dados locais e na nuvem sempre atualizados.  

---

# Microsoft Azure – Identidade e Segurança  

## Microsoft Entra  
**Microsoft Entra ID**  
É o serviço de gerenciamento de identidades e acesso baseado em nuvem do Microsoft Azure.  
- Garante a autenticação dos funcionários.  
- Permite logon único (SSO).  
- Facilita o gerenciamento de aplicativos.  

**Microsoft Entra Domain Services**  
Pensado para manter a compatibilidade com ambientes mais tradicionais, trazendo para a nuvem um Active Directory gerenciado.  

---

## Conceitos de Segurança  
- **Autenticação:** identifica a pessoa ou serviço, solicitando credenciais de acesso legítimas.  
- **Autorização:** determina o nível de acesso de uma pessoa ou serviço, definindo quais dados podem ser acessados.  
- **Autenticação multifator (MFA):** fornece segurança adicional exigindo dois ou mais elementos para completar a autenticação.  

---

## Recursos do Entra  
- **B2B do Microsoft Entra External ID:** permite que parceiros, fornecedores e convidados acessem recursos da empresa usando suas próprias credenciais.  
- **Azure AD B2C:** solução voltada ao consumidor, permitindo login com redes sociais ou contas próprias.  
- **Acesso condicional:** regras de login baseadas em fatores como localização, dispositivo e MFA.  
- **Controle de acesso baseado em função (RBAC):** organiza permissões por funções (ex.: leitor, colaborador, administrador).  
- **Modelo de confiança zero (Zero Trust):** nada é confiado por padrão; cada usuário ou dispositivo deve ser autenticado e autorizado em tempo real.  

---

## Proteção e Monitoramento  
- **Proteção completa:** fornece vários níveis de defesa; ataques contra uma camada não atingem a próxima.  
- **Microsoft Defender for Cloud:** serviço de monitoramento que fornece proteção nos datacenters.  

---

## Observações Importantes  
- Contas de usuários são excluídas permanentemente após **30 dias**.  

---

## Fatores que afetam os custos e gerenciamento financeiro no Azure  
- **Tipo de recurso:** cada recurso tem um custo específico associado.  
- **Consumo:** modelo pago conforme o uso.  
- **Manutenção:** monitorar o ambiente implantado para reduzir gastos desnecessários.  
- **Área geográfica:** o mesmo recurso pode ter preços diferentes conforme a região.  
- **Tráfego de rede:** entradas podem ser gratuitas, mas saídas geram custos.  
- **Assinatura:** o tipo e a configuração impactam nos valores.  

### Ferramentas de apoio  
- **Azure Marketplace:** catálogo de apps e serviços de parceiros.  
- **Calculadora de preços:** estima custos de produtos do Azure.  
- **Calculadora TCO:** compara custos de infraestrutura local com o Azure.  

---

## Monitoramento  

- **Azure Policy:**  
  - Impõe padrões organizacionais e avalia conformidade em escala.  
  - Impõe regras e bloqueios que não serão quebrados, mesmo por usuários com permissões elevadas.  
  - Pode ser criada e deixada desativada.  
  - Recursos fora da regra ficam como **Non-compliant**.  
  - **Remediation:** ajusta o recurso para ficar conforme a regra.  
  - **Compliant:** dentro dos padrões esperados.  
  - Obs: Policy é sobre **recursos**, não sobre usuários.  

- **Bloqueio de recursos:**  
  - Protege contra exclusões ou modificações acidentais.  
  - Pode ser aplicado na assinatura, grupo de recursos ou recurso individual.  
  - **Bloqueio de excluir:** permite leitura e atualização, mas não exclusão.  
  - **Bloqueio ReadOnly:** permite apenas leitura.  

- **Portal de Confiança do Serviço:**  
  - Local para verificar como a Microsoft segue padrões de segurança e conformidade com dados dos clientes.  

- **Microsoft Purview:**  
  - Família de soluções de governança, risco e conformidade de dados.  
  - Permite unificar e exibir dados em uma única visão.  
