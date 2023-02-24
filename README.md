## Script python para retenção de imagens ECR na AWS

  - A finalidade desse script é realizar a retenção de todas as imagens ECR untagged da sua conta AWS.
        
       - Fazendo isso de forma automatizada a cada 90 dias (você pode mudar o tempo dessa lifecycle no código).
  
  - O script importa a biblioteca boto3 do python para realizar a execução dentro da AWS.
        
       - O boto é responsável pela conexão do nosso código com os itens da AWS.
        - https://boto3.amazonaws.com/v1/documentation/api/latest/guide/sqs.html
       - No link acima você encontra a documentação da biblioteca boto.
  
  - Esse arquivo não contém inserção de keys AWS pois foi realizado e validado dentro de uma máquina AWS com SHH.
        
       - Você pode se conectar na sua máquina SSH através do remote explorer, extensão do VSCode.
       - Executar um arquivo dentro da AWS tem suas vantagens, a facilitação em relação as keys, que não precisam ser utilizadas nesse caso.
        
   - O arquivo vai listar o nome dos repositórios ECR contentes na sua conta AWS, e logo após vai aplicar a lifecycle sob os mesmos.
        
  
