# Objetivos

  - Apresentar o escopo do projeto e a nova documentação com as alterações solicitadas pelo cliente
  - Sugerir o canal de comunicação entre o consumidor e a SPC Brasil para solicitação de inclusão n Auxílioo emergencial positivo.
  - Apresentaro algoritmo desenvolvido para verificar os clientes que solicitaram a exclusão dos seus dados do Cadastroal Positivo, que constam na tabela de pagamentos.
  -  O algoritmo desenvolvido para verificar a consistência do padrão de números do CPF dos consumidores.
  -  A interface que será utilizada pelo Assistente de Atendimento da SPC Brasil para dar suporte a solicitação do consum
  
  # Comunicação: Consumidor e SPC Brasil para solicitar o Auxílio Emergencial Positivo
    

Para que o consumidor faça a solicitação do cadastro emergencial positivos, sugerimos criar a opção na página da SPC Brasil contendo essa solicitação. Com a criação desse canal de relacionamento a SPC Brasil, já pode receber as solicitações dos consumidores enquanto aguarda o desenvolvimento do produto final.
E para os que não tem acesso aos canais web fornecer os canais de teleatediemento e os postos de atedimento do consumidor.

# Tratamento de dados.

Elaboramos um algoritmo para verificar na tabela de pagamentos os consumidores que solicitaram a exclusão do cadastro positivo e retirá-los da base de dados que vai para o cadastro emergencial.
Também desenvolvemos um código que verifica na tabela de operações e cadastro de pessoa física, se os números de CPF estão dentro do padrão de 11 números. Se sim eles irão compor a base da dados do auxílio emergencial positivo.
Os algoritmos desenvolvidos são capazes de ler as extensões xlsx e csv da base de dados enviadas pelo SPC e fazer a verificação nas tabelas específicas onde se encontram os dados
