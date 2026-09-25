<h1 align="center">Conceito de DataLake</h1>

<h2>Conceito</h2>
<p>O DataLake é um repositório centralizado projetado para armazenar e processar grandes volumes de dados (estruturados e não estruturados) em escala e em seu formato bruto, oferecendo maior flexibilidade do que bancos tradicionais.</p>

<h2>Casos de Uso</h2>
<ul>
  <li><b>Dados em fomato bruto:</b>Preservação dos dados originais e flexibilidade total de análise posterior.</li>
  <li><b>Grandes volumes de dados:</b>Armazenamento e processamento eficiente em alta escala.</li>
  <li><b>Diversidade de tipos de dados:</b>Suporte simultâneo a dados estruturados e não estruturados.</li>
  <li><b>Escalabilidade:</b>Expansão simples do ambiente conforme a necessidade de dados cresce.</li>
  <li><b>Repositório centralizado:</b>Unificação e integração do armazenamento de dados provenientes de múltiplas fontes em um único local.</li>
</ul>

<h2>Diagrama do Projeto</h2>
<img src="./Diagrama DataLake.jpg">

<p>A arquitetura segue o padrão medalhão, dividida em 3 camadas:</p>
<ul>
  <li><b>Raw/Bronze:</b>É a camada responsável por receber os dados em sua forma bruta, sendo usada de forma que permita recuperar dados de forma original caso necessário, ou localizar a fonte dos dados.</li>
  <li><b>Silver/Prata:</b>É a camada responsável pelo processamento/limpeza dos dados, essa etapa viabiliza limpar os dados e torná-los mais aderentes para a próxima etapa.</li>
  <li><b>Gold/Ouro:</b>É a camada responsável pelas regras de negócio do projeto de dados e a modelagem relacional, sendo um reflexo para as métricas do negócio.</li>
</ul>

<h2>Tecnologias Usadas</h2>
<p>Nesse pequeno projeto foram utilizadas tecnologias simples com o fito de entender melhor o conceito de DataWarehouse, dessa forma, foi utilizado:</p>
<ul>
  <li><b>Python:</b>Usado como linguagem de programação do projeto, sendo utilizada para ingestão e processamento dos dados.</li>
  <li><b>Jupyter Notebook:</b>O Jupyter Notebook foi utilizado devido a sua facilidade em disponibilizar bibliotecas e recursos necessários para realizar as tratativas.</li>
  <li><b>Pandas:</b>Biblioteca usada para tratar os dados.</li>
  <li><b>DuckDB:</b>O DuckDb foi utilizado para funcionar como o banco de dados relacional do projeto, sendo usado para armazenar os dados nas diferentes etapas da arquitetura.</li>
</ul>
