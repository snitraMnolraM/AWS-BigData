# AWS-BigData
 Repositório do código da Dio Live Coding com AWS EMR e Python Neste repositório há os arquivos de configuração e execução de análise de dados.

## 

* Acessar S3: https://s3.console.aws.amazon.com/s3/ 
  * Criar estrutura de data lake : _Nome_de_sua_escolha_
  * Criar estrutura de pastas:
    * _data_

    * _output_

    * _temp_

      ​

* Acessar EMR: https://console.aws.amazon.com/elasticmapreduce/
    * O cluster será criado pelo MrJob e não pelo console

    * Infraestrutura como código 

      ​

* Criar chave SSH
    * Acessar  Console do EC2: https://console.aws.amazon.com/ec2/ -> Key Pairs -> Create Key Pair	

    * Download .pem file

      ​

* Obter Id e chave secreta AWS para configurar MrJob
   * Profile

   * My Security Credentials: https://console.aws.amazon.com/iam/home?region={region}#/security_credentials

   * Access Keys - Create new access key

   * Fazer download - única chance de visualizar

     ​

* Ambiente linux no terminal
   * Criar ambiente virtual python: _virtualenv --python=python3.8 venv_nome_de_sua_preferência_

   * Ativar o ambiente virtual python: source venv_teste/bin/activate

   * Instalar boto3: _pip install boto3_

   * Instalar mrjob: _pip install mrjob_

   * Acessar com o vs code

     ​

* Instalar vscode no Ubuntu
   *  code .

      ​

* Criar algoritmo de análise de palavras
   * dio-live-wordcount-test.py

   * map-reduce-count : contar

     ​

* Acessar S3
   * Upload de arquivo para o bucket na pasta data

     ​

* Preeche os dados no arquivo mrjorb.conf

   * _nano ~/.mrjob.conf_

     ​

* Excetute o aqruivo Python

   * _python3 dio-live-wordcount-test.py -r emr s3://{your_s3_bucket_name}/data/biblia.txt --output-dir=s3://{your_s3_bucket_name}/output/logs1 --cloud-tmp-dir=s3://{your_s3_bucket_name}/temp/_ --conf-path mrjob.conf

      