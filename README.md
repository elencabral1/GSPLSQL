# Projeto EcoWave

## Introdução
Este documento descreve a estrutura e o desenvolvimento do banco de dados utilizado no projeto EcoWave. O EcoWave é um aplicativo de educação ambiental destinado a promover a reciclagem de lixo em praias, lagos e oceanos, incentivando a coleta e o tratamento de resíduos através de funcionalidades interativas e recompensas.

## Estrutura do Banco de Dados
O banco de dados é composto por várias tabelas que suportam as funcionalidades principais do aplicativo. As tabelas foram projetadas para armazenar informações sobre usuários, itens reciclados, recompensas, localizações e mais. As operações principais implementadas incluem criação, leitura, atualização e exclusão (CRUD) para cada tabela, além de blocos anônimos PL/SQL para operações específicas.

## Tabelas
## Usuarios
Armazena informações dos usuários do aplicativo, incluindo dados pessoais e informações de login.

## ItensReciclados
Registra os itens reciclados pelos usuários, com detalhes sobre o tipo, data e quantidade dos resíduos coletados.

## Recompensas
Guarda informações sobre recompensas resgatadas pelos usuários, vinculadas à quantidade de pontos acumulados.

## Amigos
Mantém registros de amizades entre usuários, facilitando funcionalidades sociais no aplicativo.

## ReconhecimentoItens
Armazena informações sobre o reconhecimento de resíduos por imagem, associado aos usuários e à localização.

## Localizacoes
Registra detalhes sobre as localizações onde os itens foram coletados, incluindo coordenadas geográficas e descrições.

## Configuracoes
Armazena configurações do usuário que podem influenciar o comportamento do aplicativo.

## Usuarios_Amigos
Tabela de relacionamento entre usuários e amigos, suportando a funcionalidade de redes sociais no aplicativo.

## LogErros
Registra erros ocorridos no sistema, útil para monitoramento e manutenção.

## Blocos Anônimos PL/SQL
Bloco Anônimo 1: Listar todos os dados da tabela Usuarios
Recupera todos os registros de usuários cadastrados.

Bloco Anônimo 2: Listar e sumarizar dados da tabela ItensReciclados pelo campo tipo_item
Agrupa os itens reciclados por tipo e sumariza a quantidade coletada por usuário.

Bloco Anônimo 3: Atualizar e listar recompensas de um usuário específico
Atualiza informações de recompensas e lista as recompensas de um usuário selecionado.

Bloco Anônimo 4: Listar e sumarizar dados da tabela Localizacoes agrupados por nome_localizacao
Agrupa as localizações e sumariza os dados associados a cada nome de localização.

## Tecnologias Utilizadas

Oracle: Sistema de gerenciamento de banco de dados utilizado para armazenar todas as informações do projeto.

PL/SQL: Linguagem de programação utilizada para criar blocos anônimos e executar operações específicas no banco de dados.
Conclusão

O banco de dados do EcoWave foi projetado para suportar todas as funcionalidades necessárias para a operação eficiente do aplicativo. A estrutura permite a coleta, gestão e análise de dados relacionados à reciclagem e engajamento dos usuários, contribuindo para o objetivo principal de promover um ambiente mais sustentável.
