# resumo-do-lab-DIO-AZ900
Este repositório contém o resumo das lições aprendidas durante o desenvolvimento do lab na DIO
Este repositório contém meu resumo do curso de **Fundamentos do Azure (AZ-900)** oferecido pela DIO.  
Até o momento, tivemos a introdução ao conceito de computação em nuvem e uma visão geral da plataforma Microsoft Azure.

---

# Microsoft AZ-900 – Resumo

## Computação em Nuvem
- **Definição**: fornecimento de serviços de computação pela internet, habilitando inovações rápidas, recursos flexíveis e economias de escala.  
- É a virtualização dos serviços de informática.  

### Modelos de Nuvem
- **Privada (On Premise):** ambiente em nuvem no datacenter da empresa; responsabilidade total da organização.  
- **Pública:** provedor fornece os recursos via rede; não há despesas de capital para escalar; pagamento conforme uso.  
- **Híbrida:** integração entre nuvem privada e pública; maior flexibilidade e conformidade legal.  

### CapEx x OpEx
- **CapEx:** despesas de capital em infraestrutura física (valor se deprecia ao longo do tempo).  
- **OpEx:** despesas operacionais; pagamento conforme uso.  

### Modelo baseado em consumo
- Pagamento somente pelos recursos usados.  
- Melhor previsão de custos.  

### Outros conceitos
- **Jump Server:** servidor intermediário.  
- **Versões Prévias:** recursos em testes, usar com cautela.  

---

## Benefícios da Nuvem
- **Alta disponibilidade:** garante funcionamento com créditos em caso de falhas.  
- **Escalabilidade:** ajustar recursos conforme demanda.  
- **Elasticidade:** ajuste dinâmico para picos de uso (ex.: Black Friday).  
- **Confiabilidade:** resiliência e recursos distribuídos.  
- **Previsibilidade:** clareza de custos e recursos.  
- **Segurança:** ferramentas fornecidas pela Microsoft, mas configuração é responsabilidade do cliente.  
- **Governança:** padrões, auditorias e conformidade.  
- **Gerenciabilidade:** várias formas de gerenciamento (portal, CLI, API, PowerShell).  

---

## Tipos de Serviço de Nuvem
- **IaaS (Infraestrutura como Serviço):** você gerencia SO, aplicativos e dados.  
- **PaaS (Plataforma como Serviço):** você gerencia apenas aplicativos e dados; provedor cuida do resto.  
- **SaaS (Software como Serviço):** uso direto do aplicativo final (ex.: Office 365, Netflix).  

---

## Alta Disponibilidade
- **Domínio de Falhas:** protege contra falhas físicas de hardware.  
- **Domínio de Atualização:** protege contra reinícios em atualizações planejadas.  

---

## Regiões e Disponibilidade
- Mais de **60 regiões em 140 países**.  
- Compostas por datacenters próximos, para reduzir latência.  
- **Pares de Região:** redundância para recuperação de desastres.  
- **Regiões Soberanas:** restritas a governos (ex.: EUA, militar).  
- **China:** operada pela 21Vianet, conforme leis locais.  
- **Zonas de Disponibilidade:** redundância dentro da mesma região.  

---

## Organização de Recursos
- **Recursos do Azure:** VMs, storage, redes etc.  
- **Grupo de Recursos:** organiza recursos relacionados.  
- **Assinaturas:** vinculadas a uma conta, definem custos e limites.  
- **Grupos de Gerenciamento:** agrupam assinaturas para aplicar políticas.  

---

## Computação no Azure
- **Máquinas Virtuais (VMs):** emulação completa de computadores físicos (IaaS).  
- **Conjunto de Dimensionamento:** ajusta automaticamente a quantidade ou o tamanho das VMs conforme a demanda.  
- **Conjunto de Disponibilidade:** distribui VMs em domínios de falha/atualização para garantir acesso.  
- **Área de Trabalho Virtual (AVD):** desktop Windows na nuvem, pronto para usuários acessarem.  

### Diferença VMs x Área de Trabalho
- **VMs:** controle total para administradores (SO, apps, rede).  
- **Área de Trabalho Remota (AVD):** desktop pronto, gerenciado pelo Azure para usuários finais.  

---

## Contêineres
- Permitem executar aplicativos empacotados com dependências em ambientes isolados, leves e portáteis.  
- Não exigem SO completo (diferente de VMs).  
- Serviços: **Azure Container Instances (ACI)** e **Azure Kubernetes Service (AKS)**.  
- Oferta baseada em **PaaS**.  

---

## Azure Functions
- Serviço **serverless** que executa código sob demanda em resposta a eventos.  
- Escala automaticamente e cobra apenas pelo uso.  
- Oferta de **PaaS**.  

---

## Serviços de Aplicativos
- Plataforma para criar, implantar e dimensionar aplicações web e APIs.  
- Suporte a .NET, Node.js, Java, Python, PHP.  
- Oferta de **PaaS**.  

---

## Serviços de Rede
- **VNet (Virtual Network):** rede privada e isolada na nuvem para conectar VMs e serviços.  
- Permite conexão com redes locais via **VPN** ou **ExpressRoute**.  

### VPN Gateway x ExpressRoute
- **VPN Gateway:** usa internet pública para conexões criptografadas; solução mais simples e barata.  
- **ExpressRoute:** conexão privada e dedicada; maior desempenho e confiabilidade, indicada para cenários críticos.  

