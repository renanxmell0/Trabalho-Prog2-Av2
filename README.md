# Trabalho de Programação II

Este trabalho consiste em modelar e implementar um sistema gerenciador para
uma loja de casacos. Leia atentamente o enunciado do problema, identifique
os elementos do sistema e cumpra as etapas abaixo. O projeto será testado
contra plágio vindo de Inteligência Artificial (ChatGPT entre outros). Caso o
código seja produzido desta maneira, o trabalho do grupo será desconsiderado.


## Enunciado do Problema
Uma loja de casacos precisa controlar suas vendas, entender seus clientes e
realizar algumas consultas. Para isso, você foi contratado para desenvolver a
primeira versão de um software gerenciador desta loja.

---

## Etapas

> **Leia todas as etapas antes de começar a implementar o trabalho.**  
> Lembre-se que a participação de todos influencia diretamente na nota final do trabalho.

---

### 1. Criar o menu principal
Você deve fazer um menu pedindo para o usuário escolher entre as seguintes
opções:
- Cadastrar novas vendas
- Ver informações de uma venda específica, baseado no nome do cliente
- Ver informações de todas as vendas
- Encerrar o programa

### 2. Fazer o cadastro de uma quantidade de vendas definida pelo usuário
Pergunte ao usuário qual a quantidade de vendas que ele deseja cadastrar. Crie
um vetor com alocação dinâmica de memória e cadastre cada venda realizada.

#### Cada venda é uma estrutura representada por:

- Cliente (estrutura)
    - Nome
    - Sexo 
    - Idade 
- Número de itens 
- Nome do vendedor (Luiza ou Juca) 
- Valor total da venda.

#### Observe as validações abaixo:

- Impedir o cadastro de valores negativos e informar este erro.
- Impedir o cadastro de vendedor inválido (diferente das possibilidades).
- Impedir o cadastro quando o sexo do cliente for inválido (diferente de m, f ou n) e informar este erro.
- Impedir o cadastro se o nome do cliente possuir menos de 3 letras e informar este erro. 
- Validar também se possui mais de 40 caracteres no mesmo if mas não exibir nenhuma mensagem informando este erro.

- Informar ao final de cada cadastro de compra que a mesma foi cadastrada com sucesso caso não aconteça nenhum erro.
#### OBS:
- Após o término de todo o cadastro, salve as informações em um bloco de notas nomeado de “loja.txt”. 
- Pergunte ao usuário se ele deseja cadastrar mais itens (quantidade informada novamente) ou voltar ao menu principal.

### 3. Pesquisar uma venda específica
- Você deve pedir o nome do cliente a ser pesquisado.
- Informar todas as vendas feitas para este cliente, ou seja, o valor total de cada compra, a nome do vendedor e a quantidade de itens em cada compra.
- Exiba também a soma total do valor das compras feitas por este cliente.
- Caso não encontre o cliente deve-se informar que não há compras naquele nome.
- Mostre o valor da compra mais barata do cliente também.
Após exibir a informação das compras ou a informação que não encontrou,
perguntar se o usuário deseja pesquisar novamente ou retornar ao menu
principal.

### 4. Ver informações de todas as vendas
#### Você deve:
- Pedir um valor que será usado para exibir a quantidade de vendas abaixo deste valor.
- Exibir a quantidade de vendas que teve exatamente 1 item vendido.
- Exibir a quantidade de vendas que foram realizadas pela “Luiza”.
- Exibir a quantidade de compradores que não quiseram informar o sexo. Exiba tam bém o total comprado por homens.
- Exibir o valor total comprado por mulheres.
- Exibir a quantidade total de itens vendidos. Exiba também a quantidade total de vendas.
- Exibir o valor total das vendas.
- Exibir o valor médio de uma venda.
- Exibir o valor de compra mais cara feito por um homem. Calcule também o valor de compr a m ais bar ata usando a vari ável menorVenda mas não exiba nenhum a m ensag em.
- Exibir os dados da venda do cliente com o maior nome (se ele fez mais de
uma compra, exibir os dados de cada venda).
- Exibir os dados da venda do cliente mais novo (se ele fez mais de uma
compra, exibir os dados de cada venda).

Após exibir as informações:
- Perguntar se o usuário deseja retornar ao menu principal.
    - Se sim retorne ao menu principal.
    - Se não encerre o
programa.

### 5. Ao abrir o programa, carregue todas as compras do bloco de notas, caso exista

Todo o registro de compras deve ser salvo no bloco de notas “loja.txt”. Ao
cadastrar novas vendas, todas elas devem ser adicionadas às vendas já
existentes no bloco de notas. A gerência das informações salvas no bloco de
notas assim como a melhor forma de navegar no bloco de notas para obter as
informações é de livre decisão do desenvolvedor.