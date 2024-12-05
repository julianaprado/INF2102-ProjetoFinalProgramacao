# INF2102-ProjetoFinalProgramacao

Este projeto utiliza redes neurais convolucionais (CNNs) para detectar tons de pele em imagens, mesmo em condições de iluminação variadas. O modelo foi desenvolvido para realizar regressão de valores RGB, possibilitando a identificação de tons de pele em aplicações como recomendação de maquiagem. Este projeto é voltado para pesquisadores, desenvolvedores de sistemas de recomendação e profissionais da área de cosméticos interessados em personalização baseada em tons de pele.


## Manual de Utilização para Usuários Contemplados
 
  ### Guia de Instruções
  
  #### Para poder utilizar este projeto:
  - Passo 1: Tenha uma conta no google.

  #### Para Baixar o projeto faça:
  - Passo 1: Estando dentro do repositório.
  - Passo 2: Selecione o botao "Code".
  - Passo 3: Baixe o .zip.
  - Passo 4: Extraia este arquivo .zip para dentro do seu computador. (Caso tenha dúvidas, siga este [manual](https://support.microsoft.com/pt-br/windows/compactar-e-descompactar-arquivos-f6dde0a7-0fec-8294-e1d3-703ed85e7ebc))
  
  #### Para Baixar o banco de dados utilizado no projeto faça:
  - Passo 1: Acesse este link [data.zip](https://drive.google.com/file/d/1RfgX7bfDt06fNO6TjDxcSEKvz_jFXw3z/view?usp=sharing) e baixe o zip.
  - Passo 2: Extraia este arquivo .zip para dentro do seu computador. (Caso tenha dúvidas, siga este [manual](https://support.microsoft.com/pt-br/windows/compactar-e-descompactar-arquivos-f6dde0a7-0fec-8294-e1d3-703ed85e7ebc))
  - Passo 3: Após aberto, abra seu Google Drive e inclua a pasta *data* que foi extraida para dentro do seu drive, dentro da pasta My Drive (ou Meu Drive).

  #### Para rodar o projeto faça:
  - Passo 1: Acesse o [Google Colab](https://colab.research.google.com/).
  - Passo 2: Caso o popup *open notebook* já esteja aberto ao acessar o site, aperte em *upload* na esquerda e faça upload do arquivo SkinDetection+FaceDetection.ipynb para o Colab.
  - OU Passo 2: Em File > Open Notebook, siga o Passo 2 anterior.
  - Passo 3: Com o Notebook SkinDetection+FaceDetection.ipynb aberto no Google Colab, vá em Runtime > Run All.
  - Passo 4: Ao chegar na celula *Connectting to Google Drive* que conecta o drive ao notebook, será pedido permissão para conectar o Google Drive. Para continuar, conecte a conta que possui a pasta *data* baixada no My Drive.
  - Passo 5: Ao chegar na útlima celula do notebook chamada *Evaluation and Validation*, o código irá tentar acessar o modelo que está na salvo na pasta, é preciso mudar o nome para o útlimo modelo gerado. Siga o passo [Para visualizar os resultados](#para-visualizar-os-resultados)

  #### Para visualizar os resultados:
  - Passo 1: Após treinamento, o modelo é salvo dentro do seu Drive na pasta data > results > training > PASTA EM FORMATO: execution_AAAA_MM_DD_HH_MM_SS_PM ou AM (exemplo: execution_2024_12_02_23_39_20_PM).
  - Passo 2: Caso queira apenas baixar o modelo, é possível baixar o modelo que se encontra nesta pasta.
  - Passo 3: Caso queira validar e avaliar o modelo dentro do Notebook, é preciso trocar o nome da variável *modelSaved* para o nome da pasta no Passo 1 (essa variável se encontra dentro das duas funções da seção *Evaluation and Validation*).
