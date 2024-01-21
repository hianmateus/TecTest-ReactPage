Primeiramente Agradeço pela oportunidade de praticar minhas habilidades nesse teste. Para começar vou ser honesto e deixar claro que sou desenvolvedor Frontend, Backend ainda não é o meu forte
fiz o possivel para entender os conceitos mas como o prazo de entrega era curto vou lhe entrega este projeto Frontend Sem banco de dados. Muito bem, o sistema todo foi feito no Frontend, logo
você dara de cara com essa tela, o Header decorativo e ao centro a seção principal onde temos um Botão de cadastro e um input para filtrarmos os clientes

![Captura de tela 2024-01-21 030512](https://github.com/hianmateus/TecTest-ReactPage/assets/103609199/e3ef9a8a-70c7-411b-b914-9fe3c2440e51)

como pode ver as informções do cliente vão ser divididas abaixo desses paragrafos em: "Cliente" onde tera seu nome, "email" ficara o email, "telefone" seu telefone, adicionei mas duas informações,
"Realizadas?" seria se a visita para limpeza foi feita ou não no cliente, Status exebirá a informação de "Realizada" ou "Não Realizada" isso pode ser genrenciado com apenas um clique em ambos.


para o cadastro basta clicar no botão ao lado do H1 "Visitas", abrirá uma box onde serão colocadas as informações, optei por algo mais "clean" simples mas com um pouco de beleza:

![Captura de tela 2024-01-21 031251](https://github.com/hianmateus/TecTest-ReactPage/assets/103609199/865545a7-f777-457e-9111-dde4baff4650)

A codificação foi simples, A div ja existe e esta apenas oculta com o display: "none", se clicar no botão vermelho com um "X" a box será fechada e as informações nos inputs se apagarão

![Captura de tela 2024-01-21 031440](https://github.com/hianmateus/TecTest-ReactPage/assets/103609199/9c51afb1-5779-4c67-90b9-18552442162c)


colocando as informações manualmente, pois não tive tempo de melhorar os inputs, estava mais preocupado com o funcionamento de outras partes do sistema, "Cidade" e "Bairro" seriam ulteis na hora
de localiza-los no mapa Bidimensional, mas essa parte estava além das minhas capacidades no momento devido ao tempo, no fim acabou sendo adicionado para preencher o espaço na tela

![Captura de tela 2024-01-21 031844](https://github.com/hianmateus/TecTest-ReactPage/assets/103609199/0d1a80ca-5d4c-4a2a-a4e9-c49445ef2a10)


Clicando em "Cadastrar" a box se feichará e as informações dos inputs são apagadas e enviadas para a lista de clientes, nessa função é enviado um Objeto com os valores dos inputs, obtidos pelo
useRef

![Captura de tela 2024-01-21 032525](https://github.com/hianmateus/TecTest-ReactPage/assets/103609199/3e864e81-9093-4fd1-b0a9-24c081897b2e)

![Captura de tela 2024-01-21 032621](https://github.com/hianmateus/TecTest-ReactPage/assets/103609199/a8d099ac-d362-4aa3-be82-c07c01ac573d)


Logo após isso, sera criado uma <li> com as informações colocadas anteriormente, todas abaixo de seus respectivos "Titulos", foi feita através do "Map" mapeando dentro de uma "ul" uma Lista criada pelo "StyledCompents"
(aliás foi usado Styled-Components na aplicação) a variavel "Clientes" que depois foi alterada para "Clientes Filtrados" logo mais terá o porque,

![Captura de tela 2024-01-21 033414](https://github.com/hianmateus/TecTest-ReactPage/assets/103609199/a66ba6de-d51b-4b6d-8211-9b069879dd4c)

![Captura de tela 2024-01-21 033706](https://github.com/hianmateus/TecTest-ReactPage/assets/103609199/1742e83e-7feb-470f-b301-d7887bac679e)


se reparar agora, há um botão de "delete" ao lado de Status, ele serve exataamente para deletar este cliente, o css es bom mas não esta perfeito, como pode ver se for adicionado mais clientes
na Lista algumas informações de nome, email e telefone podem ser maiores ou menores, isso altera um pouco a posiçao dos elementos mas nada que atrapalhe a compreensão.

![Captura de tela 2024-01-21 034843](https://github.com/hianmateus/TecTest-ReactPage/assets/103609199/4f28ec64-c8ef-402b-9a28-c8e73e4e970f)


nas areas de "Realizadas?" e "Status" quando clicados mudam seus valores, de "Não" para "Sim" e de "Não Realizada" para "Realizada", o sistema disso seria melhor, onde selecionando um mudaria
o outro e a cor do Status mudando de vermelho para azul, mas essa parte começou ficar complicado então deixei de lado para poder terminar a tempo. O codigo dessa parte ficou bem simples, uma
função com IF e Else, mundando dependo do valor do paragrafo

![Captura de tela 2024-01-21 035235](https://github.com/hianmateus/TecTest-ReactPage/assets/103609199/55deae8d-faac-4bd0-9f5d-13bc73172ec5)


![Captura de tela 2024-01-21 035416](https://github.com/hianmateus/TecTest-ReactPage/assets/103609199/4a8b9ad9-9e6e-4371-93b7-b68d5b5dfa55)


Seguindo agora para a parte de Filtrar os clientes, ao input, você pode escrever o nome do cliente e então a lista irá diminuir até chegar ao cliente q busca, foi nesse momento que o 
codigo para mapear a lista precisou ser alterado de "Clientes" para "ClientesFiltrados", mas para filtrar a lista bastou apenas umas linhas de codigo para o "Filter" e outra diretamente no input, seguido de uma função para
buscar o nome do cliente na lista

![Captura de tela 2024-01-21 035625](https://github.com/hianmateus/TecTest-ReactPage/assets/103609199/4c204c8a-2576-49f1-bc95-5c4c6d6e512f)

![Captura de tela 2024-01-21 040606](https://github.com/hianmateus/TecTest-ReactPage/assets/103609199/531fba2e-c862-4cf5-b609-25021aba0ba7)


![Captura de tela 2024-01-21 040342](https://github.com/hianmateus/TecTest-ReactPage/assets/103609199/a4c4dbeb-88c5-40c2-bba5-651facbe22a5)

![Captura de tela 2024-01-21 040456](https://github.com/hianmateus/TecTest-ReactPage/assets/103609199/830c0082-3365-4a98-a7cc-84fc279a5762)


Infelizmente O backend não é meu ponto forte ja que desde que comecei minha jornada na programação me vi mais inclinado para o Fronend, por isso aplicação infelizmente n possui um servidor
feito com Nodejs utilizando PostgreSQL, por isso as informações não ficam salvas quando se aperta o F5, a segunda Parte do teste assumo que estava além da minhas capacidades, quando fui atras
de como implementar o mapa Bidimensional vi que nao daria tempo, pois eu precisaria fazer uma Representação dos Indivíduos, Função de Avaliação (Função Fitness), Inicialização Populacional
Algoritmo Genético / Colônia de Formigas / Enxame de Partículas e uma Condição de Parada, esses eram Conceitos novos para mim quando estava estudando para fazer o teste então só pude entregar
aquilo na qual estava mais capacitado que era o Frontend em React. No mais agradeço pela oportunidade de melhorar minhas habilidades de Criação de interfaces e Resolução de Problemas



