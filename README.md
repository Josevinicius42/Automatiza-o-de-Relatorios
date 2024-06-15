# Automatização de Processos - Power Automate 

<img src="https://github.com/Josevinicius42/Projeto_PowerAutomate/assets/144733214/56146c88-55a6-4231-9cf4-965ee4ed29aa" alt="Microsoft Power Automate" width="40" />

## Envio de Relatório por Email

  O Power BI disponibiliza um envio de relatório já integrado ao workspace. Porém, o email que chega para as pessoas contém muitas informações e muitas vezes cai na caixa de spam, podendo gerar desconfianças dos destinatários em abrir ou até em visualizar o relatório. Com isso, criei um fluxo automatizado que pega o anexo do email enviado para o Power BI na minha caixa de mensagens e envia automaticamente colando apenas a imagem de forma muito mais visual no corpo do email.
  Com isso, esse fluxo resolve esses problemas:

  

Segue passos:

### 1º Passo: Crie uma nova pasta no email

  No seu email, voce vai criar uma pasta com o nome que desejar. Aqui, botei o nome como "POWERBI"
  
  ![image](https://github.com/Josevinicius42/Projeto_PowerAutomate/assets/144733214/e3791164-9192-4cf9-a6d9-3488800aeba8)

### 2º Passo: Crie uma regra

  No seu email, crie uma regra para todos os emails que vier do PowerBI, ser redirecionado para essa nova pasta que criou.

  ![image](https://github.com/Josevinicius42/Projeto_PowerAutomate/assets/144733214/facaa2f9-391e-49af-8899-8adceec0a4d2)
  
### 3º Passo: Faça o teste de envio

  Vá no seu relatorio do powerbi, selecione em "Assinar o relatorio". Crie uma assinatura e envie para seu email.
  Após chegar no seu email, na pasta que criou chamada POWERBI, salve o anexo .png.
  Crie uma pasta de trabalho no seu computador e coloque o aquivo salvado nela.

     ![image](https://github.com/Josevinicius42/Projeto_PowerAutomate/assets/144733214/caa03b37-ddbc-43d3-8d4b-4cba69655c11)

### 3º Passo: 1º Fluxo no Automate

  

