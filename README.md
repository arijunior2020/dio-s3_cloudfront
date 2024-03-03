# Desafio: Criando Sites Estáticos com Amazon S3 e CloudFront

Este projeto visa demonstrar como criar e hospedar um site estático utilizando Amazon S3 e CloudFront, garantindo uma distribuição rápida e segura do conteúdo.

## Passos Realizados:

1. **Criação do Bucket S3:**
   - Foi criado um bucket no Amazon S3 sem permissão de acesso público.
   - Os arquivos do site estático foram carregados para o bucket. Os arquivos estão localizados na pasta `files_s3` deste projeto.

2. **Criação da Distribuição CloudFront:**
   - Uma distribuição do CloudFront foi configurada.
   - O bucket S3 criado foi configurado como origem (origin) para o CloudFront.

3. **Política de Acesso Restrito:**
   - No cloudfront foi criada uma OAC (Origin acess control) que é uma política para permitir apenas que o CloudFront acesse o bucket S3, garantindo assim uma camada adicional de segurança.

## Como Utilizar:

Para reproduzir este projeto, siga os seguintes passos:

1. Faça o clone deste repositório em sua máquina local.
2. Acesse a pasta `files_s3` e substitua os arquivos pelo conteúdo do seu site estático.
3. Configure um novo bucket no Amazon S3 e faça o upload dos arquivos do seu site para esse bucket.
4. Crie uma distribuição do CloudFront e configure o bucket S3 como sua origem.
5. Crie uma política de controle de acesso de origem (OAC) no CloudFront para permitir que o CloudFront acesse os arquivos no bucket S3.


Após seguir esses passos, seu site estático estará hospedado no Amazon S3 e será distribuído de forma rápida e segura pelo CloudFront.

## Site Funcionando pelo CloudFront:

Aqui estão algumas capturas de tela do site hospedado pelo CloudFront:

![Página Inicial](caminho/para/captura-de-tela-1.png)
*Página Inicial*

![Página do Blog](caminho/para/captura-de-tela-2.png)
*Página do Blog*



