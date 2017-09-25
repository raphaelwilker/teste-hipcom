# teste-hipcom #

### Sinal de socorro recebido ###

Fonte: 61 Ursa Maior
Tipo: Sinal de Socorro
Tipo do Emissor: Espaçonave
Detalhes do Emissor: Embarcação de Exploração Classe IV

/// Início da Mensagem ///

Ao acionar meu motor de dobra no último salto de sistema atingi uma anomalia que danificou os sistemas de suporte a vida de minha nave. Tenho apenas 2 horas de oxigênio restante. Meu software de dobra também sofreu uma interferência e foi corrompido. Preciso de ajuda urgentemente para efetuar o upload de uma interface para alimentar meu motor de dobra com as coordenadas de planetas viáveis para reabastecer minha nave com oxigênio o mais rápido possível e realizar um salto.

A interface do software do motor de dobra é alimentada via Json e deve ser implementada em uma página HTML. Segue em anexo a especificação da funcionalidade em sua completude.

/// Fim da Mensagem ///

/// Anexo 1 ///

Implemente, no arquivo interface.html, uma tabela dinâmica utilizando apenas Javascript e jQuery (plugins jQuery são permitidos) para armazenar os dados dos planetas mais próximos que foram encontrados. A tabela deve ser alimentada pelo JSON que pode ser obtido invocando o método scanPlanets(), já implementado no arquivo, imediatamente ao carregar a página.
Todos os plugins devem ser linkados remotamente (ex. <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>);

A tabela deve conter as seguintes colunas:

* Id: O id do planeta. Um número inteiro, incremental (ex. 1, 2, 3);
* Nome: O nome do planeta (ex. "Terra");
* Nível de O2: uma porcentagem inteira (a fonte de dados é de 0 a 1, sendo 0 = 0% e 1 = 100%), obrigatoriamente com dois dígitos (ex. 25%, 07%);
* Gravidade: número com duas casas decimais obrigatórias, em Gs (ex. 3,75G, 0,50G);
* Distância: em Anos Luz (LY). Exibir no máximo 4 casas decimais (ex. 7,4567LY, 0,4LY);
* Carregar: Esta coluna deve conter um botão que abre uma nova janela exibindo o JSON com as informações da linha. Mais detalhes abaixo.

A página deve conter as seguintes funcionalidades:

* Todos os campos, exceto o Id, devem ser editáveis;
* Inserir linha: Um botão que insere uma nova linha vazia na tabela, para inserir coordenadas de planetas manualmente;
* Imprimir Dados: Deve abrir uma nova janela exibindo o JSON completo da tabela, contemplando todas as modificações feitas manualmente;
* Carregar: Ao clicar no botão "Carregar" de uma dada linha, uma janela deve abrir contendo o JSON daquela linha apenas. Um botão "Saltar" deve ser exibido, mas só pode estar ativo caso o planeta esteja na distância de salto. A distância máxima de salto é de 24,327LY.

Outras considerações:

* Qualquer melhoria na usabilidade do software que não tenha sido especificada é bem vinda (ordenação da tabela, paginação etc);
* Minha vida está em suas mãos. Tenho família na estação orbital em LXA-437. Caso não sobreviva peç/// Fim do Anexo 1 ///
*** Fim do sinal de socorro ***
