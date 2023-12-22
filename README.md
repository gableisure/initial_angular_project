## Configuração inicial do projeto

Para configurar o projeto no servidor, deve-se criar o arquivo .env no diretório raiz do projeto. Neste arquivo, defina as variáveis de ambiente necessárias para garantir o correto funcionamento do sistema. Essas configurações incluem informações sensíveis. Certifique-se de proteger o arquivo .env e não compartilhá-lo publicamente, garantindo a segurança e confidencialidade dos dados.

Copie as váriaveis de ambiente abaixo, cole no arquivo .env criado e salve.

``` Endpoint Eproc ES
ENDPOINT_JFES='https://eproc-ws.jfes.jus.br/eproc'

# Endpoint Eproc RJ
ENDPOINT_JFRJ='https://eproc-ws.jfrj.jus.br/eproc'

# Login Eproc
LOGIN='Preencha o login aqui...'

# Senha Eproc
SENHA='Preencha a senha aqui...'

# Diretório de destino dos arquivo baixados no scraping
PATH_RELATORIO='/dados/arquivos_a_processar/trf/trf2' ```

## Execução manual do projeto

1º Passo: Instalar o pacote virtualenv

`pip3 install virtualenv`

2º Passo: Criar um ambiente virtual

`virtualenv venv_sc_trf2`

3º Passo: Entrar no ambiente virtual

`source venv_sc_trf2/bin/activate`

4º Passo: Instalar os pacotes necessários

`pip3 install -r requirements.txt`

5º Passo: Executar o projeto

`python3 main.py`
