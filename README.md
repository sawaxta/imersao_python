# Automação de Cadastro de Produtos com Python

Este projeto de automação, desenvolvido em Python, foi criado como parte da aula **Python Power UP** e tem como objetivo simplificar o processo de cadastro de múltiplos produtos em um sistema, evitando o trabalho manual repetitivo.

## Objetivo

Imagine que você possui uma grande quantidade de produtos para cadastrar em um sistema, com informações como código, marca, tipo, preço, custo, entre outros. Ao invés de cadastrar esses produtos um por um, essa automação permite que o Python faça isso para você, controlando o mouse e o teclado, replicando as ações humanas de forma automática.

## Funcionalidades

O código é capaz de:
- Abrir o navegador e acessar o sistema de login automaticamente.
- Inserir as credenciais de login.
- Ler as informações dos produtos de um arquivo CSV.
- Preencher os campos de cadastro no sistema com os dados de cada produto.
- Submeter cada cadastro e repetir o processo para todos os produtos do arquivo.

## Pré-requisitos

- **Python 3**
- Bibliotecas necessárias:
  - `pyautogui`: para automação de ações do mouse e do teclado.
  - `pandas`: para manipulação e leitura de arquivos CSV.

Para instalar as bibliotecas, execute:
`
pip install pyautogui pandas
`
## Estrutura do Código

1. **Abrir o Sistema**: O script abre o navegador e acessa o sistema de login.
2. **Login**: Insere o e-mail e a senha do usuário para acessar o sistema.
3. **Importar Dados**: Lê o arquivo `produtos.csv` que contém as informações dos produtos.
4. **Cadastro Automático**: Itera por cada linha do arquivo CSV, preenchendo os campos necessários no sistema e enviando o formulário.

## Como Utilizar

1. **Configure o arquivo CSV**: Certifique-se de que o arquivo `produtos.csv` esteja no mesmo diretório que o script Python. Ele deve conter colunas como `codigo`, `marca`, `tipo`, `categoria`, `preco_unitario`, `custo` e `obs` para que as informações sejam lidas corretamente.
2. **Ajuste as Coordenadas (se necessário)**: O código utiliza coordenadas de tela específicas para cliques (posição `x`, `y`). Você pode ajustar essas coordenadas conforme o layout do seu sistema.
3. **Execute o Script**:
`
   python automacao_cadastro.py
`


