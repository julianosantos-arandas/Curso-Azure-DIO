# Curso-Azure-DIO
Repositório referente às etapas do curso Azure.
Este README tem como objetivo mostrar o processo de criação do ambiente básico, que foi apresentado até este momento no curso Microsoft AI for Tech - Azure Databricks.

➡️ Definição de tipos de serviços cloud:

 Existem 3 modelos de serviçõs cloud.

◾ IaaS - Infrastructure as a Service.
 - Modelo em nuvem que oferece servidores, armazenamento e rede, onde não existe a necessidade de hardware físico.
 - O acesso a esse tipo de serviço ocorre por meio de uma interface web ou API, utilizando recursos virtualizados e hospedados em Data Centers dos provedores     e nuvem.

◾ PaaS - Plataform as a Service.
 - Modelo em nuvem onde o provedor do serviço fica responsável pela manutenção, escalabilidade e infraestrutura; o cliente fica com a parte do                    desenvolvimento: compilar, implantar e gerenciar aplicativos.

◾ SaaS - Software as a Service.
 - Modelo em nuvem onde o provedor entrega um software baseado em nuvem, e o cliente pode acessar os aplicativos pela internet.
 -  Este modelo opera com base em assinaturas e elimina a necessidade de instalação ou manutenção local do software.
    Exemplos comuns de Saas:
    ▪️Serviços de emails - Gmail e Outlook.com
    ▪️ Armazenamento online - Dropbox e Google Drive
    ▪️APPs de produtividade - Trello e Notion
    
![Iass, Saas, PaaS](https://github.com/user-attachments/assets/088823b6-53bd-4fe1-8f2c-982fb97f42e8)

➡️ Tipos de Clouds:

◾ Pública
 - Modelo onde o cliente usa, por meio da internet, os recursos de um provedor (como a Azure) em vez de servidores físicos no local.
   
◾ Privada
 - Modelo de computação em nuvem onde os recursos são dedicados exclusivamente a uma única organização, e os dados e a infraestrutura pertencem somente a ela    (hardware e software). Garante maior controle, segurança e personalização.
◾ Híbrida
 - Modelo que combina a nuvem privada ou infraestrutura local (on-premises) com uma nuvem pública (Azure), permitindo integração entre ambas.

![nuvem-hibrida-priava-publica](https://github.com/user-attachments/assets/74be086f-32f9-4894-adf3-d0332960e47e)

➡️ Sobre a Azure:

◾ A Azure se baseia nos conceitos da computação em nuvem (um conjunto de serviços usados por meio da internet para construir e rodar qualquer tipo de sistema).
Anteriormente, as empresas tinham que arcar com os custos e o trabalho de:
 - comprar servidores
 - instalar sistemas
 - manter tudo ativo
 - pagar os custos com energia 
 - segurança e atualização de hardwares
Com os serviços da Azure você aluga tudo isso e só paga pelo que usa, diminuindo os gastos de um ambiente on-premises, executando a infraestrutura com mais eficiência e escalando as operações conforme a necessidade do negócio.

◾ Possibilidades de serviços usando a Azure:
 - criar servidores virtuais
 - armazenar arquivos
 - gerenciar bancos de dados
 - desenvolver aplicativos
 - treinar IA
 - proteger sistemas
 - conectar redes
 - fazer análises de dados
 - integrar dispositivos IoT

➡️ Availability Zones - Zonas de disponibilidade: 
 - É uma região da Azure composta por localizações físicas exclusivas projetadas para proteger aplicações contra falhas de data center (cada uma com energia,     rede e resfriamento independentes).
 - Cada zona é composta por um ou mais data centers.
 - A separação física das zonas de disponibilidade protege os aplicativos e os dados contra problemas de nível de instalação.
 - A Azure copia seu sistema para várias zonas independentes, garantindo que, se uma falhar, o serviço continue funcionando sem interrupção.

➡️ Criar o ambiente básico: 

<img width="1553" height="483" alt="image" src="https://github.com/user-attachments/assets/24747086-61a0-4670-95bd-930d6b5aa4e7" />

 - 🌐 Criar conta na Azure:
   - Acesse: https://portal.azure.com
   - Clique em Create Microsoft Account ou Sign up
   - Faça login com seu e-mail (pode ser Gmail).
   - Preencha:
   - nome, país, CPF
   - número de telefone
   - Cadastre um cartão de crédito (eles não cobram nada sem aviso).
   - Confirme o e-mail e o telefone.
   - Você ganha: 200 dólares de crédito por 30 dias e acesso ao Azure Free Tier por 12 meses.

 - 🏗 2) Criar um Resource Group (RG) — “pasta” da Azure:
   - O Resource Group é onde você organiza seus serviços (VM, banco, storage, rede…).
   - No portal, procure: Resource groups
   - Clique em Create
   - Preencha:
      - Subscription: Azure free trial
      - Resource group name: rg-lab-juliano
      - Region: Brazil South (ou East US se quiser mais barato)
   - Clique em Review + Create → Create
 
  <img width="1225" height="798" alt="create-account-basics-v2" src="https://github.com/user-attachments/assets/98762d61-7fa7-4721-aafa-3d6856826ff1" />

 - 🏗 Criar um Data Factory:
   - Cique no serviço Azure Data Factory.

      <img width="807" height="236" alt="image" src="https://github.com/user-attachments/assets/84bf1217-cdc1-4ec7-955d-0ac0d252decc" />

   - Clique em: Create (Criar)

      <img width="259" height="210" alt="image" src="https://github.com/user-attachments/assets/5622b6ae-2177-4e5c-a995-f0434e170c7c" />

   - Preencher as configurações básicas:
      - Project details
      - Subscription: Azure Free Trial
      - Resource Group: rg-lab-juliano (ou o que você criou
      - Factory details
      - Name: adf-juliano-lab (não pode ter espaço nem acento)
      - Region: East US ou Brazil South (East US geralmente é mais barato)
      - Version - Select version: V2 (sempre escolha V2)
        <img width="738" height="611" alt="image" src="https://github.com/user-attachments/assets/0d8ac802-5867-46c8-b116-ff90b9506dfd" />

   - Revisar e criar:
      - Review + Create
      - Depois em Create

   - Abrir o Data factory:
      - Go to resource
      - Launch Data Factory Studio
        <img width="1398" height="611" alt="image" src="https://github.com/user-attachments/assets/0e397788-534b-4e4e-967c-6980d2be61b0" />
      - Por meio deste painel você cria:
         - Pipelines
         - Dataflows
         - Linked Services
         - Triggers
         - Integrações com Storage, SQL entre outros recursos.



     
