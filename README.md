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
- **Autenticação**: identifica a pessoa ou serviço, solicitando credenciais de acesso legítimas.  
- **Autorização**: determina o nível de acesso de uma pessoa ou serviço, definindo quais dados podem ser acessados.  
- **Autenticação multifator (MFA)**: fornece segurança adicional exigindo dois ou mais elementos para completar a autenticação.  

---

## Recursos do Entra
- **B2B do Microsoft Entra External ID**: permite que parceiros, fornecedores e convidados acessem recursos da empresa usando suas próprias credenciais, sem precisar criar contas internas.  
- **Azure AD B2C**: solução voltada ao consumidor, permitindo login com redes sociais ou contas próprias criadas pelo usuário.  
- **Acesso condicional**: define regras de login baseadas em fatores como localização, dispositivo e MFA, liberando ou bloqueando acesso conforme o risco.  
- **Controle de acesso baseado em função (RBAC)**: organiza permissões por funções (ex.: leitor, colaborador, administrador), garantindo que cada usuário tenha apenas o acesso necessário.  
- **Modelo de confiança zero (Zero Trust)**: abordagem onde nada é confiado por padrão; cada usuário ou dispositivo deve ser autenticado e autorizado em tempo real.  

---

## Proteção e Monitoramento
- **Proteção completa**: fornece vários níveis de defesa; ataques contra uma camada não atingem a próxima.  
- **Microsoft Defender for Cloud**: serviço de monitoramento que fornece proteção nos datacenters. Oferece recomendações de segurança, detecta e bloqueia malware, analisa e identifica ataques potenciais.  

---

## Observações Importantes
- Contas de usuários são excluídas permanentemente após **30 dias**.

---

## Fatores que afetam os custos e gerenciamento financeiro no Azure
- **Tipo de recurso:** cada recurso tem um custo específico associado.  
- **Consumo:** modelo pago conforme o uso; quanto mais consome, maior o custo.  
- **Manutenção:** monitorar o ambiente já implantado para reduzir gastos desnecessários.  
- **Área geográfica:** o mesmo recurso pode ter preços diferentes conforme a região.  
- **Tráfego de rede:** transferências de entrada podem ser gratuitas, mas as de saída (ex.: entre regiões) geram custos.  
- **Assinatura:** o tipo e a configuração da assinatura impactam nos valores.  

### Ferramentas de apoio  
- **Azure Marketplace:** catálogo de aplicativos e serviços de parceiros; garantia oferecida pelo fabricante, não pela Microsoft.  
- **Calculadora de preços:** permite estimar custos de produtos do Azure considerando região, camada, opções de cobrança, suporte, programas e ofertas.  
- **Calculadora de Custo Total de Propriedade (TCO):** compara os custos da infraestrutura local com os custos no Azure, ajudando a estimar economias potenciais.  
- **Monitoramento**  

---

## Azure Policy
- As políticas do Azure ajudam a impor padrões organizacionais e a avaliar a conformidade em escala.  
- Impõe regras e bloqueios que não serão quebrados, mesmo com usuários que tenham todos os poderes de manejamento.  
- Avalia e identifica: é uma regra acima de qualquer permissão.  
- Pode ser criada e deixada desativada.  
- Se aplicada após a existência de recursos que não estão dentro da regra, ficará como **Non-compliant** apontando esses recursos.  
- **Remediation:** altera e deixa o recurso da maneira “correta”.  
- **Compliant:** segue todos os padrões esperados.  
- **Policy** não é sobre usuários, e sim sobre os recursos.  

---

## Bloqueio de Recursos
- Protege os recursos do Azure contra exclusões ou modificações acidentais.  
- Pode ser gerenciado na assinatura, grupo de recursos ou níveis de recursos individuais dentro do portal do Azure.  
- **Bloqueio de Excluir:** permite leitura e atualização, mas não a exclusão.  
- **Bloqueio ReadOnly:** permite apenas a leitura do recurso.  

---

## Portal de Confiança do Serviço
- Local onde pode-se ver como a Microsoft segue os padrões de segurança e política com os dados dos clientes.  

---

## Microsoft Purview
- Família de soluções de governança, risco e conformidade de dados.  
- Auxilia a unificar e exibir os dados em uma única exibição unificada.  

---

## Ferramentas para Interagir com o Azure
- **Portal do Azure**  
- **Azure Cloud Shell**  
- **Azure PowerShell**  
- **Interface de Linha de Comando (CLI)**  

---

## Azure Arc
- Serve para gerir recursos multicloud, recursos que não estão dentro do Azure.  
- Gestão de recursos tanto de outras Clouds quanto de on-premises.  
- Obs: administra apenas recursos que estão fora do Azure.  

---

## Azure Resource Manager (ARM)
- É uma camada de gerenciamento que permite criar, atualizar ou excluir recursos Azure.  
- Ele recebe todas as requisições, independente do modelo que o usuário está fazendo, administra e segue conforme o comando solicitado.  

### Modelos do ARM
- São arquivos no modelo JSON (JavaScript Object Notation) que podem ser usados para criar e implantar a infraestrutura do Azure sem a necessidade de escrever comandos de programação.  

---

## Infraestrutura como Código
- Garante consistência na implantação em todo o ecossistema da nuvem.  
- Gerencie a configuração em escala.  
- Provisionamento de ambiente de forma rápida.  

---

## Bicep
- Linguagem de programação nativa da Microsoft para descrever recursos do Azure.  

---

## Ferramentas de monitoramento
- **Assistente do Azure:** analisa recursos implantados no Azure e faz recomendações com base nas práticas recomendadas para otimizar os recursos.  
  - Confiabilidade, segurança, desempenho, custo e excelência operacional.  
- **Integridade do serviço do Azure (Status do Azure):** mantém você informado sobre o status geral do Azure, incluindo serviços e recursos que podem afetar ou já estar afetando o usuário.  
- **Azure Monitor:** focado em maximizar a disponibilidade e desempenho de aplicativos e serviços, coletando, analisando e tomando decisões com base na telemetria da nuvem e de ambientes locais.  
- **Resource Health:** mostra a saúde e disponibilidade de recursos individuais do Azure, informando se estão funcionando corretamente e alertando sobre problemas que possam afetá-los.
