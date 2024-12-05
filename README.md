# INF2102-ProjetoFinalProgramacao

## Descrição do Projeto
Este projeto implementa um sistema para reconhecimento de tom de pele. Ele foi desenvolvido para identificar tons de pele em imagens com iluminação diferentes mas contando que seja possivel detectar um rosto, com foco em aplicações como recomendação de maquiagem.

### Principais Funcionalidades
- Treinamento e avaliação de modelos de aprendizado de máquina para detecção de tons de pele com dados de entrada RGB normalizados.
- Visualização de resultados gerando imagens dos tons de pele detectados.
- Exportação de modelos no formato ONNX para uso em diferentes plataformas.
  
### Público-Alvo
- Pesquisadores em áreas de aprendizado de máquina, visão computacional e tecnologia aplicada à indústria da beleza.
- Profissionais da indústria cosmética, especialmente aqueles que trabalham com personalização de produtos.
- Estudantes de ciências da computação interessados em técnicas de aprendizado de máquina aplicadas.

### Natureza do Programa
- Uma prova parcial de conceito.
- Ferramenta utilitária em desenvolvimento para experimentação e testes em projetos acadêmicos e de aplicação prática.

### Ressalvas
- O modelo depende da qualidade e variabilidade do dataset utilizado, podendo apresentar viés em situações não representadas nos dados de treinamento.
- Não aborda questões sociais relacionadas à representação racial ou implicações éticas do uso de reconhecimento de tom de pele.

## Visão de Projeto

### Cenário Positivo 1:

O professor Jan quer gerar um modelo treinado de reconhecimento de tom de pele e decide utilizar este projeto. Fazendo o download do projeto, e seguindo corretamente todos os passos descrito neste projeto, ele consegue gerar o modelo que fica salvo em seu Google Drive.

### Cenário Negativo 1:

O professor Alberto quer gerar um modelo treinado de reconhecimento de tom de pele e decide utilizar este projeto. Fazendo o download do projeto, ele não opta por utilizar o Google Colab, gerando inumeros erros.

### Cenário Negativo 2:

O professor Luiz quer gerar um modelo treinado de reconhecimento de tom de pele e decide utilizar este projeto. Fazendo o download do projeto, e optando por utilizar o Google Colab da forma como foi descrita aqui, ele esquece de apertar "Run All", e aperta para rodar apenas a celula que gera o modelo, gerando erros.

### Cenário Negativo 3:

O professor Paulo quer gerar um modelo treinado de reconhecimento de tom de pele e decide utilizar este projeto. Fazendo o download do projeto, e optando por utilizar o Google Colab da forma como foi descrita aqui, ele aperta "Run All" mas esqueceu de passar a pasta dos dados para seu drive, na pasta My Drive, corretamente gerando erros.

## Manual de Utilização para Usuários Contemplados
 
  ### Guia de Instruções:
  
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

  ### Exceções ou potenciais problemas:
  
  Caso fique muito tempo sem atividade no notebook:
  - O notebook irá parar de rodar, então faça: [Para rodar o projeto faça](#para-rodar-o-projeto-faça). 

 Caso dê erro de que não foi possível encontrar a pasta com o database:
  - Então faça: [Para Baixar o banco de dados utilizado no projeto faça](#para-baixar-o-banco-de-dados-utilizado-no-projeto-faça).

  Caso ao rodar tudo, chegue na útlima célula e quebre:
  - Então faça: [Para visualizar os resultados](#para-visualizar-os-resultados).




