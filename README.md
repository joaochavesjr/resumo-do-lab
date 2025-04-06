# resumo-do-lab
Este repositório contém o resumo das lições aprendidas durante o desenvolvimento do lab na DIO
---
### Computação e Rede do Azure (Lab realizado em 06/04/2025)
Configurando Recursos e Dimensionamentos em Máquinas Virtuais na Azure

- Primeiro iniciamos a criação de uma VM e observamos que há uma sugestão de vários padrões de máquinas pré definidos, divididos em ambientes de trabalho de desenvolvimento e produção e também o tipo de carga de trabalho, como uso geral, otimizado para memória e computação otimizada.
- Também foi observado que há a possibilidade de escolhar sistemas operacionas já com recursos instalados como por exemplo, um servidor Wordpress que já vem instalado e configurado todos os componentes necessários.
- Criação passo a passo de uma VM:
  - Inicilmente definida a escolha de assinatura e grupo de recursos;
  - Nome da VM;
  - Região (EAST US 2);
  - Opções de disponibilidade (Zona de Disponibilidade), dimensionamento automático, previsão de escalonamento, definir condições de dimensionamento para escalar horizontalmente (aumentar e diminuir limite (mínimo e máximo), duração da consulta);
  - Selecionada imagem do Windows Server 2019 Datacenter - x64 Gen2;
  - Entender o "Executar com desconto de Spot do Azure";
  - Definir tamanho da VM entre os vários disponíveis (CPU, Memória, Disco, IOPS) e ver uma prévia do custo;
  - Imgagens personalizadas;
  - Definir usuário e senha para usuário administrador;
  - Regas de portas de entrada, como por exemplo RDP, para acesso remoto;
  - Tamanho e tipo de disco como HDD, SSD;
  - Alerta para excluir os discos com a VM (opção) para evitar discos orfãos;
  - Escolha de rede virtual e boas práticas para não expor portas em IPs públicos;
  - Alerta para excluir o IP público e a NIC quando a VM for excluida (opção);
  - Integração com o Azure AD, desligamento automático;
  - Habilitar backup, definição de política;
  - Habilitar monitoramento e regras de alertas;
  - Instalação de agentes e estensões como CONTROL-M, HPE Security Fortify, agentes de monitoramento;
  - Revisão de recursos e custos;
  - Área de trabalho do Azure;
    - Criar imagem personalizada
    - Selecionar host pessoal ou em pool
  - Aplicativos de Funções
     - Código
     - Image de Contâiner
     - Pilha de runtime (.NET, Node.js, Python, Java, PowerShell Core, Custom Handler)
     - Versão, região
     - Sistema Operacional (Linux, Windows)
    
---
### Componentes de Arquitetura do Azure (Lab realizado em 04/04/2025)

- Acesso página do Azure global infraestructure, onde é possível abrir uma tela que exibe o globo e possibilita interagir e visualizar todas as regiões, datacenters e suas interligações em 3D.
- É possível observar o datacenter de São Paulo e que sua replicação é com uma região dos Estados Unidos.
- Existe um datacenter no Rio de Janeiro (Southeast) apenas para replicação de dados para atender exigências da LGPD e no caso de Disaster Recovery.
- Ainda no globo (Global Map) é possível efetuar um tour virtual em um datacenter da Microsoft, com a possibilidade de acessar áreas internas, externas e sala de servidores.
- Já retornando no portal do Azure, vimos a criação de um Grupo de Recursos, escolhendo a assinatura e a região, definição de marcações (rótulos).
- Após a criação foram verificados recursos como log de atividade, IAM (Controle de acesso);
- Comentado no aula que a permissão de acesso deve ser o mais restrito possível;
- Observado também a tela de visualização de recursos, que permite uma representação gráfica e hierarquica;
- Na parte de eventos é possível observar as automatizações.
- Depois vimos a criação de uma rede virtual e seu endereçamento dentro do grupo de recursos.
  
  
---
### Tipos de serviços de nuvem (Lab realizado em 04/04/2025)

Vimos os seguintes tipos de serviços:

- IaaS (Infraestrutura como Serviço) 
  - Fornece infraestrutura virtualizada

- PaaS (Plataforma como Serviço) 
  - Oferece uma plataforma para desenvolver aplicativos
  - Por exempplo instalação de Banco de dados;
    
- SaaS (Software como Serviço) 
  - Fornece toda a aplicação pronta hospedada por terceiros
  - Por exemplo, Office 365 

- Observamos na criação de uma nova máquina virtual, a possibilidade de selecionar uma imagem de sistema operacional, seu tamanho e ter uma previsibilidade inicial de custos.
- Outros detalhes da máquina também foi observado como discos adicionais, a parte de rede como endereçamento, gerenciamento, proteção, desligamento automático, entre outros.
- Foi orientado que é importante verificar todas as opções e detalhes para criação da máquina no portal.
- Também observamos a criação de banco de dados SQL, que inicialmente é necessário criar um servidor e definir recursos como localização, método de autenticação, redundância, e com base na configuração definida, podemos observar um resumo do custo mensal. 
   
---

## Benenfícios da Nuvem (Lab realizado em 03/04/2025)

- Foram observados os níveis de SLA, conforme listado abaixo:

| SLA     | Tempo de inatividade por semana | Tempo de inatividade por mês | Tempo de inatividade por ano |
|---------|---------------------------------|------------------------------|------------------------------|
| 99%     | 1.68 hora                       | 7.2 horas                    | 3.65 dias                    |
| 99.9%   | 10.1 minutos                    | 43.2 minutos                 | 8.76 horas                   |
| 99.95%  | 5 minutos                       | 21.6 minutos                 | 4.38 horas                   |
| 99.99%  | 1.01 minuto                     | 4.32 minutos                 | 52.56 minutos                |
| 99.999% | 6 segundos                      | 25.9 segundos                | 5.26 minutos                 |

- Quanto maior for o número de noves menor será a indisponibilidade.
- Caso a indisponibilidade seja maior que a contratada a Azure gera créditos para ressarcimento do cliente.
- Também foi verificado, nos recursos de Computação, a possibilidade de criar VMs em mais de uma zona de disponibilidade, permitindo escolher até 3 zonas distintas, com a criação de uma VM em cada zona, possibilitando assim alta disponibilidade.
- Outro ponto interessante foi a observação de dicas na interface (i) que apresenta um resumo de cada opção, clicando no ícone este leva para a página de documentação do recurso (saiba mais).
- Também foi observado as contas de armazenamento, que permite escolher a estratégia de redundância que define como os dados serão replicados entre data centers e regiões.
- E finalmente podemos concluir que todos os recursos para implementação de redundância e nível de disponibilidade impactam diretamente o custo das soluções.


---
## Acesso Portal Microsoft Azure

- Verificação da lista de recursos disponíveis na tela incial

- Observado as possibilidades de configuração do perfil, permitindo customizações como escolha do idioma, posicionamento dos menus e aplicação de temas.

- Acesso ao botão "Todos os serviviços" permitindo visualizar todos os serviços disponíveis, classificados por categoria.
- Verificada as opções de computação como Imagens, Máquinas Virtuais, Computação de Alto Desempenho, entre outros.
- Também foram observadas algumas opções em Rede onde foi destacado a possibilidade de criação de Bastion (jump server), Gerenciadores de Redes, Firewall, Gateway, Endereços IP Públicos, Interfaces de rede, entre outros.
