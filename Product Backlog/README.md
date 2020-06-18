# Product Backlog com novo escopo
Após a reunião de validação das entregas com o cliente SPC Brasil no dia 04/06/2020, fizemos algumas mudanças no projeto para adaptar a real necessidade do cliente. Foi pedido para que o time focasse em apresentar soluções de negócio e um valor real para o produto, e também, que o escopo do projeto estive claro com referência ao que vamos entregar. Diante dessas solicitações, segue o novo escopo, com as alterações e adaptações feitas pelo time. 
# Projeto: Auxílio Emergencial Positivo 
 
 <img src="https://raw.githubusercontent.com/marciosousa4/projeto-integrador/376d71b42da02278e03b7af2472d9488a8f6bcf2/Logo%20auxilio%20emergencial.jpg" width="230" height="130" />

# Objetivo
O programa Auxílio Emergencial Positivo foi concebido a partir da constatação do compromisso que a SPC Brasil tem com a sociedade nos momentos de risco ao seu crédito positivo e pelo compromisso que a empresa tem em ser um elo de confiança para consumidores e empresa conveniadas. 
O projeto tem como objetivo principal, desenvolver uma ferramenta de software que consiga dar suporte aos  assistentes de atendimento da SPC Brasil, para verificar a viabilidade da inclusão no auxilio emergencial positivo,  garantindo a segurança de crédito dos consumidores que estão inclusos no cadastro positivo e que estão adimplentes com suas contas nos 12 (doze) meses anteriores a solicitação.  
# Justificativa
O Programa que oferecemos nessa ferramenta de software, busca romper com o paradigma de que a empresa só participa como plataforma integradora de informações e inteligência de dados, ele reafirma o compromisso com a sociedade, além de imprimir um caráter de liderança que por si só, já gera um valor, não unicamente a ela, mas também à toda sociedade e ao entorno que ela opera, capitalizando os chamados valores intangíveis. 
A ferramenta desenvolvida também ajudará os assistentes de atendimento a fornecer ao consumidor segurança em permanecer no cadastro positivo, pois garante que, nos momentos mais difíceis seu crédito positivo estará protegido pela empresa que tem a missão de “Prover soluções que atendam às necessidades de negócio e de crédito”.

# Dimensões do projeto

# Atores
A ferramenta será usada pelo Assistente de Atendimento da SPC para dar suporte ao consumidor quando ele precisar realizar o cadastro no Auxílio Emergencial Positivo.
# Interface
Interface contendo a tela inicial da ferramenta 
Interface que apresente o que é o Auxílio emergencial positivo.
Interface que mostre a opção de consultar o CPF do consumidor 
Interface que mostre o histórico de pagamentos do consumidor 
Interface que apresente a opção de inclusão no Auxílio Emergencial positivo com as opções de situações emergenciais e de inclusão da documentação comprobatória. 

# Ações
- O consumidor envia um email para a SPC solicitando a inclusão do cadastro no Auxílio emergencial positivo.
- O assistente de atendimento recebe o email e faz a verificação do histórico de pagamentos desse consumidor. 
- Se aprovado, o assistente de atendimento verifica se o consumidor enviou e documentação que comprovam a real necessidade da inclusão no cadastro. 
- Se reprovado, o assistente de atendimento reponde o email, informado que não foi aprovada a solicitação. 
- Se o consumidor foi aprovado e enviou a documentação, o Assistente de Atendimento faz a inclusão da documentação no cadastro do consumidor, marca a opção que gerou a necessidade e o Score do consumidor fica congelado por 60 dias.
- Se ele foi aprovado e não enviou a documentação o Assistente de Atendimento faz a solicitação para o consumidor por email.

# Dados fundamentais para o funcionamento da aplicação.
- Dados de transações financeiras dos consumidores fornecidos pelas empresas credoras que constem os seguintes dados:
•	Valor total da compra
•	Valor e vencimento das parcelas
•	Valor e data do pagamento 
•	Parcelas a vencer

- Tabela de situações emergenciais para consulta dos consumidores 
- Canal de interação entre consumidor e SPC (email, telefone ou presencial)
Regra de negócio
- O Auxílio emergencial positivo garante que o consumidor tenha seu score congelado, ou seja, que não haja movimentação na pontuação do score, caso ele se enquadre em uma situação emergencial, por até 2 meses. 
- Situações emergenciais são: Desastres naturais, Doenças consideradas graves, pandemias ou perda de emprego sem justa causa. 
- O consumidor só poderá fazer esse requerimento uma vez por ano
- Se antes do prazo terminar o consumidor estiver em situação melhor e quiser informar o SPC para que seu score retorne a computação dos pagamentos, pode ser feito a qualquer momento, dentro do prazo de 2 meses. 
- O SPC garante proteção apenas da movimentação de computação dos pontos do score positivo, sem nenhuma relação com o comprometimento de pagamento das contas. 

# Ambiente
 - Uma aplicação para desktop, a fim de não comprometer a segurança das informações e facilitar a distribuição da ferramenta.
- Será usado o framework Electron que permite o desenvolvimento de aplicações para desktop GUI usando componentes criados para aplicações web.
- No desenvolvimento da interface, utilizamos a linguagem de marcação HTML e a folha de estilo CSS, por apresentarem grande versatilidade de edição de layout e cores.
- Para compor a estrutura de tratamento e análise de dados, optamos pela linguagem Python, por ter um grande acervo de bibliotecas específicas para tais funções.
- Na integração dos arquivos python com a parte visual, foi utilizada a linguagem Javascript e o interpretador Nodejs(ambos próprios do Electron) juntamente com o módulo Python-Shell, que lê scripts em python a partir do Nodejs.
# Qualidade
- O consumidor se sentirá seguro ao optar pelo Auxílio Emergencial Positivo, pois não haverá risco de um problema esporádico e temporário comprometer o seu score.
- Reduzirá o número de pedidos de exclusão do cadastro positivo
- O SPC estará comprometido com o consumidor protegendo seu produto mais valiosos que é o crédito dos consumidores.
- Cumprirá a sua missão de ser um elo de confinaça para o consumidor.
- Responsabilidade Social 
# Diagrama de caso de uso
![](https://raw.githubusercontent.com/marciosousa4/projeto-integrador/3bafc8f59cce9b46f4e6173ae71330dc82df095e/diagrama%20de%20caso%20de%20uso.jpg)


# Requisitos 

1.	Como consumidor preciso ser incluso no cadastro emergencial positivo, pois estou em uma situação emergencial que está comprometendo o equilíbrio entre receitas e despesas em minha vida pessoal.
*	Disponibilizar Canais de contato para que seja feita essa solicitação (email, telefone ou presencial). Incluir o item no campo de atendimentos da página fale conosco da SPC Brasil. 
*	Informar para o consumidor quais são as reais situações que pode ser requerido o auxílio. Colocar na página da SPC Brasil o item explicativo do projeto. 
*	Ter uma interface que apresente o que é o cadastro emergencial positivo, para colocar na página da SPC Brasil. 

2.	Como assistente de atendimento da SPC Brasil, quero dar suporte à solicitação do consumidor que precisa ser incluso no cadastro emergencial positivo.
*	Ter uma aplicação para desktop, a fim de não comprometer a segurança das informações e facilitar a distribuição da ferramenta.
*	Ter uma interface contendo a tela inicial da ferramenta que mostre a opção de consulta de CPF do cliente.
*	Usar o framework Electron que permite o desenvolvimento de aplicações para desktop GUI com componentes criados para aplicações web.
*	No desenvolvimento da interface, utilizar a linguagem de marcação HTML e a folha de estilo CSS, por apresentarem grande versatilidade de edição de layout e cores.
*	Aplicar a 8 heurística de Jakob Nielsen, “estética e designer minimalista”, assim o assistente poderá verificar com rapidez agilidade e de forma desburocratizada a possibilidade de atendimento do consumidor. 
*	Manter consistência entre as telas da aplicação com as telas padrões da SPC Brasil será essencial para que não seja necessário o entendimento de vários padrões e formas de interações diferentes para cada tela. 

3.	Como assistente de atendimento preciso verificar se o cliente está adimplente nos últimos 12 meses para dar prosseguimento à solicitação.
* Fazer um código que faça a verificação da qualidade dos dados recebidos pelas instituições financeiras do cadastro positivo.
*	Fazer um código que separe os consumidores que estão inclusos no cadastro positivo. 
*	Fazer um código que faça a separação do histórico de pagamentos dos clientes e mostre esses dados individualizados por CPF. 
*	Para compor a estrutura de tratamento e análise de dados, usar a linguagem Python, por ter um grande acervo de bibliotecas específicas para tais funções.
*	Na integração dos arquivos python com a parte visual, utilizar a linguagem Javascript e o interpretador Nodejs (ambos próprios do Electron) juntamente com o módulo Python-Shell, que lê scripts em python a partir do Nodejs.
*	Interface que mostre a opção de consultar o CPF do consumidor e mostre esses dados individualizados. 
4.	Como assistente de atendimento preciso incluir a situação emergencial do consumidor e a documentação comprobatória da real necessidade do auxílio no cadastro positivo. 
*	Com a verificação positiva do cadastro do cliente, acrescentar uma interface que tenha um campo para marcar o motivo da requisição do auxílio.
*	Colocar as opções com caixas de marcação para facilitar a navegação do assistente nas opções de inclusão. 
*	Aplicar a 8 heurística de Jakob Nielsen, “estética e designer minimalista”, assim o assistente poderá verificar de forma ágil, qual a classificação do cliente e como inserir a documentação no cadastro. 
5.	Como assistente de atendimento preciso enviar a confirmação para o cliente que seu cadastro se encontra incluso no Auxílio Emergencial Positivo e que, por 2 meses as suas contas não serão computadas negativamente em seu cadastro, caso haja algum atraso nos pagamentos.

# Product Backlog

Quando o projeto passou pela análise de viabilidade, e começamos a tomar conhecimento do escopo macro do projeto, já na fase de iniciação, fizemos algumas reuniões com pessoas da área de negócio e com os professores, para o entendimento e possível extração de alguns requisitos que serviriam para criação do Product Backlog, norteando, inclusive, o planejamento das primeiras Sprints.
Para se ter dimensão da complexidade, o escopo deste projeto contempla desde o estudo e conhecimento da nova legislação em vigor do cadastro positivo (LGPD) até criação de novas aplicações para interfacear a comunicação e a troca de arquivos entre vários agentes financeiros e a SPC Brasil. Além do redesenho de vários processos, incluindo uma robusta ferramenta de analise e qualificação dos dados recebidos, precisamos também tornar esses dados acessíveis aos setores que geram produtos e, consequentemente, acrescentam valor aos dados. Para atender as demandas de negócio, criamos 6 *users story cards* diferentes, sendo 6 entregas para a empresa que será impactada diretamente pelo projeto. Atualmente temos 4 estudantes de Análise e Desenvolvimento de Sistemas, trabalhando nesse PB ao longo de todo o projeto. Frisa-se que, a elevada complexidade fez com que este projeto fosse revisto e aprimorado o seu desenvolvimento de execução. Também houve mudanças nas datas previstas por causa da pandemia do coronarivírus no mundo todo, este episódio, por si só, faz com que a as expectativas e os desafio aumentem ainda mais. Por outro lado, porém, temos a nosso favor importantes e valiosas lições aprendidas como a utilização de ferramentas colaborativas e trabalho remoto.

# *User Story Cards*

O grau de complexidade de cada Sprint foi feito  em uma Planning Poker, usando como parâmetros a Sequência de Fibonacci que ajudou buscar uma estimativa via consenso da equipe e um melhor planejamento do desenvolvimento do projeto. 


![](https://raw.githubusercontent.com/marciosousa4/projeto-integrador/ec9931dee079aee4f5259eae6ee1f26e4785cf71/user%20story%20cards.jpeg)

# Requisitos Globais   

* Receber os dados das empresas conveniadas;

* Verificar da qualidade dos dados recebidos;

* Atender a legislação do Cadastro Positivo;

* Analisar a qualidade dos dados recebidos;

* Analisar as movimentações do Cadastro Positivo;
 
* Assegurar de forma ágil e com segurança o compartilhamento e integração das informações;

* Aplicar as métricas dos indicadores de qualidade dos dados e indicadores de négocio nos dados selecionados;

* Fazer uma interface, que apresente de maneira centralizada e de fácil manipulação,
o conjunto de indicadores e suas métricas.
