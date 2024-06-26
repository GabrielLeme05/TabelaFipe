
O projeto está estruturado da seguinte forma:

consulta-preco-veiculos/
│
├── index.html          # Página principal do aplicativo
├── styles.css          # Estilos CSS para estilizar a página
├── app.js              # Código JavaScript com a lógica do aplicativo
├── sw.js               # Service Worker para habilitar funcionalidade offline
└── README.md           # Documentação do projeto (este arquivo)

Funcionalidades Principais
1 -Consulta de Preços: Os usuários podem selecionar o mês de referência, tipo de veículo, marca, modelo e ano/combustível do veículo desejado. Ao clicar em "Consultar", o aplicativo faz uma requisição à API da FIPE e exibe o preço médio do veículo.

2 -Histórico de Preços: Quando disponível, o aplicativo exibe um histórico de preços para o ano selecionado em formato de gráfico. Isso permite aos usuários visualizarem as variações de preço ao longo do tempo.

3 -Funcionalidade Offline: O aplicativo utiliza um Service Worker para possibilitar o acesso offline. Isso significa que os usuários podem continuar utilizando o aplicativo mesmo sem uma conexão ativa com a internet. O Service Worker cacheia os recursos estáticos (HTML, CSS, JavaScript) para que eles possam ser acessados offline.



Funcionamento Detalhado
*Carregamento da Página: Quando a página é carregada, o JavaScript é ativado e inicia o carregamento dos dados do mês de referência através da função loadReferencia().

*Interatividade: Os usuários interagem com os selects na página para escolher o mês de referência, tipo de veículo, marca, modelo e ano/combustível do veículo desejado.

*Requisições à API da FIPE: Ao selecionar as opções desejadas e clicar em "Consultar", o aplicativo faz requisições à API da FIPE para obter os preços médios dos veículos.

*Renderização dos Resultados: Os resultados da consulta são renderizados na página em formato de tabela, exibindo informações como mês de referência, código FIPE, marca, modelo, ano, combustível, data da consulta e preço médio.

*Exibição do Histórico de Preços: Se disponível, o aplicativo exibe um gráfico com o histórico de preços para o ano selecionado. Isso é feito através da função renderChart(), que utiliza a biblioteca Chart.js para renderizar o gráfico.

*Funcionalidade Offline: O Service Worker controla o cache dos recursos estáticos do aplicativo, permitindo que ele seja acessado offline. Se o usuário tentar acessar o aplicativo sem uma conexão ativa com a internet, ele será redirecionado para uma página offline.

## Hospedagem

Este projeto está hospedado no Netlify. Para acessar o site online, você pode visitar [(https://tabelafipe001.netlify.app)](https://seu-site.netlify.app/).

## Autor

[(https://github.com/GabrielLeme05)]




#   t a b e l a f i p e 0 0 1  
 #   t a b e l a f i p e 0 0 1  
 #   t a b e l a f i p e 0 0 1  
 #   M a r c i o T a b e l a  
 #   M a r c i o T a b e l a  
 