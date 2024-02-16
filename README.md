# Como Executar o Projeto

## Estrutura do Projeto
- O repositório possui alguns arquivos, sendo eles:
- HuggingFaceModel-v2.ipynb -> Modelo final, seguindo requisições do projeto
- Classification-Better-2.ipynb -> Modelo alternativo, que não possui desempenho satisfatório nas perguntas exemplo, mas vejo potencial futuro para maior velocidade, menor limitação de requests e sem custo
- /datasets -> diretório onde os Jsons são armazenados
- /datasets/Classification/email.json -> Perguntas enviadas por email
- /datasets/Classification/small.json -> Perguntas falsas criadas para utilização no Classification-Better-2.ipynb

## Requisitos
- O modelo final foi criado baseando-se no seguinte [projeto](https://www.pinecone.io/learn/series/langchain/langchain-intro/)
- Portanto, para executar o projeto é necessário possuir um Jupyter Notebook (Ou outra plataforma compatível) com Python 3.9
- Também é necessário instalar as biblitoecas langchain com `pip install langchain` e huggingface_hub com `pip install huggingface_hub`
- Criar uma conta [Hugging Face](https://huggingface.co/settings/tokens) e uma API key com write acess
- Substituir a API key na parte dedicada do código, conforme imagem:

<p align="center">
<kbd>
<img src="https://github.com/Lucas-Inacioo/LLM/assets/110082578/8908498f-9135-42cc-a067-b146214eab2d">
</kbd>
</p>

## Utilização
- Por padrão, o código executará as 10 perguntas de teste que foram feitas por e-mail
- Caso deseje incluir outras perguntas, de forma a melhorar a visualização dos resultados e permitir diversas perguntas serem feitas simultâneamente, crie um arquivo Json com a seguinte estrutura e coloque-o no diretório `datasets/Classification`:

<p align="center">
<kbd>
<img src="https://github.com/Lucas-Inacioo/LLM/assets/110082578/9b38d80f-371b-4a77-8963-fdbd102a6ad3">
</kbd>
</p>

- No diretório `datasets/Classification/email.json` um exemplo pode ser encontrado
- Com o arquivo no local correto, altere no Notebook o caminho para o arquivo que deseja utilizar, conforme imagem:

<p align="center">
<kbd>
<img src="https://github.com/Lucas-Inacioo/LLM/assets/110082578/e2b131a7-dd7b-4f6c-8ea0-53bd6bc63d32">
</kbd>
</p>
