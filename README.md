# resumo-do-lab
Este repositório contém o resumo das lições aprendidas durante o desenvolvimento do lab na DIO
---
## Tipos de serviços de nuvem (Lab realizado em 04/04/2025)

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
