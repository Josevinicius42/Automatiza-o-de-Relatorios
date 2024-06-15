# Automatização de Processos - Power Automate 

<img src="https://github.com/Josevinicius42/Projeto_PowerAutomate/assets/144733214/56146c88-55a6-4231-9cf4-965ee4ed29aa" alt="Microsoft Power Automate" width="40" />

## Envio de Relatório por Email

  O Power BI disponibiliza um envio de relatório já integrado ao workspace. Porém, o email que chega para as pessoas contém muitas informações e muitas vezes cai na caixa de spam, podendo gerar desconfianças dos destinatários em abrir ou até em visualizar o relatório. Com isso, criei um fluxo automatizado que pega o anexo do email enviado para o Power BI na minha caixa de mensagens e envia automaticamente colando apenas a imagem de forma muito mais visual no corpo do email.
  
  **Com isso, esse fluxo resolve esses problemas:**

![image](https://github.com/Josevinicius42/Projeto_PowerAutomate/assets/144733214/78c79dbe-f822-41f3-9593-cb00824dad5b)


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

### 3º Passo: "Quando um novo email é recebido (V3)"

![image](https://github.com/Josevinicius42/Projeto_PowerAutomate/assets/144733214/f7ea49b4-51e6-4cc8-a134-519c9f3f2aee)


  **Inicio de Fluxo no Automate:**

  Selecione o fluxo "Quando um novo email é recebido (V3)", selecione em parametros avançados "Incluir anexos" ; "Filtro de Assunto" ; "Importancia" ; "Somente com Anexos" ; "Pasta".
  
  Preencha conforme a imagem a seguir, apenas no "Filtro de Assunto", coloque o titulo do email que chega o seu relatorio do PBI.


    
![image](https://github.com/Josevinicius42/Projeto_PowerAutomate/assets/144733214/5c8b13a3-6d28-4e98-afc1-eaf04349baaa)

### 4º Passo: "Obter Anexo (V2)"

![image](https://github.com/Josevinicius42/Projeto_PowerAutomate/assets/144733214/81da2446-6079-4b25-b249-bcd0df718716)


 Ao selecionar, coloque em ID da mensagem: "ID da Mensagem" e no id do anexo, "Anexos ID do Anexo". Após isso, ira aparecer o termo "FOR EACH" automaticamente entre esse fluxo e o anterior.

 ![image](https://github.com/Josevinicius42/Projeto_PowerAutomate/assets/144733214/e3c6c2f3-4bab-4d07-9a30-411379e5fdc7)

 Após isso, dentro do mesmo fluxo "FOR EACH", selecione o fluxo "Atualizar Arquivo". Na parte de "Arquivo" coloque o caminho da pasta que salvou a imagem em .PNG e selecione "Bytes de Conteudo" na parte de Conteudo do Arquivo.

 **Com esse passo, voce esta informando que sempre que receber o email do PBI, deverá substituir a imagem salva sempre com o ultimo email enviado.**

![image](https://github.com/Josevinicius42/Projeto_PowerAutomate/assets/144733214/4ace3345-8f64-4248-86b5-e3612ebd5d32)

  

  

  

