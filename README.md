<h1>Algoritmos-e-Estrutura-de-Dados :technologist:</h1>
<br/>
<p>Projeto de Algortimos do curso de Sistemas de Informação UFPE</p>
<h3>Objetivo do projeto:</h3>
<ul>
  <li> Utilizar o algoritmo de dijkstra em um contexto real de aplicação</li>
</ul>
<h3>Sobre o problema:</h3>
<p>Dentre tantos aeroportos internacionais espalhados pelo mundo, o número de rotas que podem ser feitas entre dois aeroportos é gigantesco. Com o objetivo de otimizar o tempo gasto na tarefa de encontrar esses caminhos, e de conseguir o caminho mais curto possível, decidimos colocar em prática os nossos conhecimentos e desenvolver um algoritmo que resolva esse problema.</p>
<h3>Base de dados utilizada: :shipit:</h3>
<p>Com o uso do site www.flightconnections.com anotamos em um arquivo.txt alguns dos aeroportos (93) e suas conexões (135). Cada linha do arquivo segue o seguinte padrão: origem destino distância. Os nomes dos aeroportos estão abreviados pelas iniciais e a distância é dada em milhas. Os aeroportos representam os vértices do grafo, as conexões as arestas e a distância o peso da aresta</p>

![dados](https://user-images.githubusercontent.com/104574086/213192856-4f444667-06ee-4481-baff-2b9c58ff2c9f.png)
<h3>Bibliotecas utilizadas</h3>
<ul>
  <li>MatPlotLib</li>
  <li>Networkx</li>
  <li>PySimpleGUI</li>
</ul>
<h3>A Solução:</h3>
<p>Para resolver o problema, escolhemos o algoritmo de Dijkstra, por ser simples e não haver arestas de peso negativo no nosso grafo. O algoritmo funciona da seguinte maneira</p><br/>
<ol>
  <li>O nó de origem recebe peso de caminho 0, e os demais recebem esse peso como infinito.</li><br/>
  <li>O algoritmo começa pelo nó de origem e analisa o grafo inteiro em busca do menor caminho. Ele mantém o valor do menor caminho armazenado e o atualiza sempre que encontra um caminho menor.</li><br/>
  <li>O peso de caminho que um nó recebe é igual ao peso do seu antecessor + peso da aresta que os liga.</li><br/>
  <li>Uma vez que o algoritmo encontra o menor caminho entre a origem e um nó, ele o marca como visitado e o adiciona ao caminho. O processo continua até que todos os nós tenham sido visitados, retornando o caminho mais curto para cada nó a partir da origem.</li><br/>
</ol>
<h3>Descrição da implementação :computer:</h3>
<ol>
  <li>Foi definida uma classe de heap de mínimo para a implementação do Dijkstra posteriormente.</li>
  <li>Foi definida uma classe de grafo, para que o mesmo fosse construído com a base de dados.</li>
  <li>A função calcula_caminho, dentro da classe grafo, foi definida e faz uso do algoritmo Dijkstra.</li>
  <li>O arquivo.txt da base de dados foi convertido para um objeto grafo.</li>
  <li>Uma interface de usuário para visualização em python foi feita com a biblioteca PySimpleGUI.</li>
  <li>As bibliotecas MatPlotLib e Networkx são usadas para a visualização do grafo e o menor caminho.</li>
</ol>
<h3>Resultados</h3>

![projeto2](https://user-images.githubusercontent.com/104574086/213194324-bff044f1-33da-45b8-b908-fa391acc6dba.png)

![PROJETO 4](https://user-images.githubusercontent.com/104574086/213195553-84841fb9-066c-4bb8-87e7-1dd89984e762.png)

![projeto3](https://user-images.githubusercontent.com/104574086/213196027-9ad81591-a523-473b-a6cc-6b4842554b2d.png)

<h3>Links Importantes</h3>
<ul>
  <li>Slides da apresentação: https://docs.google.com/presentation/d/1mBEifS8Lc5fEZelkMCYgq7sHbQPOXUf9E9jQDVZ4L2s/edit?usp=sharing </li>
  <li>Video da apresentação do projeto: https://www.youtube.com/watch?v=Llw_FmcFQTY</li>
</ul>

<h3>Referências</h3>

* https://www.flightconnections.com/
* https://www.freecodecamp.org/news/dijkstras-shortest-path-algorithm-visual-introduction/#:~:text=Dijkstra%27s%20Algorithm%20finds%20the%20shortest,node%20and%20all%20other%20nodes
* https://www.youtube.com/watch?v=3vBx8GqlVT4&t=1968s
* icone do avião: <a href="https://www.flaticon.com/br/icones-gratis/ao-redor-do-mundo" title="ao redor do mundo ícones">Ao redor do mundo ícones criados por surang - Flaticon</a>





