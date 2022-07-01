# ai-ag-robocode

## Projeto template para a aula de Algoritmos Genéticos com Robocode da disciplina de Inteligencia Artificial do curso de Engenharia de Software

### Passo à passo

1. Intalar o Robocode na máquina. Disponível em: https://robocode.sourceforge.io/

2. Fazer o download do JGAP (Java Genetic Algorithms Package): Disponível em: https://sourceforge.net/projects/jgap/files/jgap/

Faça download do arquivo jgap_<versão>_full.zip
Depois de extrair os arquivos, deverá haver um arquivo chamado jgap.jar dentro da pasta, este usaremos posteriormente

3. Fazer Clone/Fork deste repositório

4. Abra o projeto com o Eclipse IDE

5. Importe os seguintes arquivos JAR:

JGAP: jgap.jar que está na pasta gerada no item 2
ROBOCODE: robocode.jar que está na pasta /libs dentro da instalação do robocode

6. Executar o arquivo src/robocodeGA.java

Com isso, será aberto o robocode e criadas algumas batalhas já incluindo o robo AGRobot

### Versões utilizadas neste projeto

JDK 11.0.12
JGAP 3.6.3
Robocode 1.9.4.6

### Programação

Agora com o projeto funcionando, podemos criar nosso próprio robô

#### Primeiro vamos entender cada classe:

1. src/robocodeGA.java

Esta é a lógica principal do programa. Aqui que usamos o JGAP para criar cromossomos a partir de genes e evoluir através de gerações a partir do melhor de cada população

Nesta classe você irá configurar tudo que diz respeito ao Algorítmo Genético

2. src/createRobo.java

Este arquivo é usado para escrever e compilar o robô para batalha. Ele recebe uma matriz dos valores (cromossomos) depois de passados pelo JGAP. Os valores podem ser usados para escrever a lógica do bot

Nesta classe você vai criar a lógica padrão do seu robô, bem como seu nome

3. src/battleObserver.java

Este é o arquivo que observa a batalha e passa os resultados de volta para o programa principal. Lógica muito simples atualmente para obter qual robô marca a maior quantidade de pontos na batalha. Pode ser estendido para obter acertos/erros etc.

4. robots/custom/AGRobot.java

Arquivo de robô gerado a partir do programa. Este é compilado para AGRobot.class, que é usado para combater outros robôs pela evolução

Este arquivo vai ter o nome que você usar no item 2.

#### Programando o seu robô

Uma vez entendidas as classes, você irá trabalhar inicialmente em duas classes:

1. src/createRobo.java

Edite essa classe com o intuito de programar a lógica inicial do robô a ser gerado e seus métodos, faça uso dos cromossomos gerados ao longo das gerações

2. src/robocodeGA.java

Aqui você editará os parametros de geração dos algoritmos genéticos de acordo com o que vimos na aula


### Referências:
https://github.com/samternent/robocode-jgap-template
