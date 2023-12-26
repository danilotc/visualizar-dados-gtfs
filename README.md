# Lendo Datasets de GTFS

Este repositório foi criado para visualizar alguns dados do [GTFS](https://developers.google.com/transit/gtfs?hl=pt-br) no [Google Colab](https://colab.research.google.com) através de um código simples escrito em Python. Este código utiliza uma biblioteca chamada [Pandas](https://pandas.pydata.org) para ler o arquivo e apresentar os dados em formato tabular.

## Como utilizar este repositório?

### Informações úteis
* O repositório contém uma pasta chamada `sample_feed` contendo os datasets de exemplo fornecidos neste [link](https://gtfs.org/pt_BR/schedule/example-feed).

* Além da pasta com os datasets de exemplo, você também encontra um arquivo chamado `gtfs_dados.ipynb` com algumas instruções e o código utilizado para visualizar os dados de cada dataset.

### Executando o código

* Este código foi criado e testado usando o Google Colab, por isso você pode acessá-lo através [deste link](https://colab.research.google.com/drive/1t8WS4WltiDQBVnfUbVghC8axOFYAomSV), mas para executar o código e visualizar os dados será necessário estar logado em uma conta google e subir os arquivos da pasta `sample_feed`. Caso não queira fazer este processo, tente a próxima possibilidade a seguir.

* Com os dados apresentados em informações úteis é possível executar o arquivo utilizando o Jupyter Notebook online através do projeto [JupyterLab](https://jupyter.org/try) sem precisar instalar a ferramenta. Caso queira simplesmente testar o código, faça o seguinte:

  * Baixe os arquivos deste repositório;
  * Acesse [este link](https://jupyter.org/try) e escolha a ferramenta JupyterLab;
  * No menu lateral esquerdo faça upload do arquivo `gtfs_dados.ipynb` e todos os arquivos da pasta `sample_feed`;
  * Por fim, abra o arquivo `gtfs_dados.ipynb` e clique no botão `run`.

### Se um erro for apresentado em qualquer tentativa de execução, realize uma das ações abaixo:

**Primeira opção:** Remova a string `"sample_feed/"` nesta linha de código, ela corresponde ao nome da pasta criada para organizar os datasets após o upload.

```python
fonte = "sample_feed/" + datasets[1] + ".txt"
```

**Segunda opção:** Após realizar o upload dos arquivos, crie uma pasta chamada `sample_feed` e coloque todos os arquivos de dataset dentro dela (como eu fiz). Esse processo é mais fácil se utilizar o JupyterLab online por ser possível selecionar múltiplos arquivos antes de movê-los. Neste caso, não será necessário remover nada no código como na primeira opção.