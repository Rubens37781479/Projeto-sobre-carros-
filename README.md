# Projeto-sobre-carros-
README.md — Documentação Externa do Código
markdown
Copiar
Editar
# Sistema de Gerenciamento de Carros com Pilha (em C)

## Funcionalidades

1. **Adicionar carro**: Insere um novo carro no topo da pilha.
2. **Mostrar nomes dos carros**: Exibe apenas os nomes dos carros, do mais recente para o mais antigo.
3. **Imprimir carros**: Mostra todos os dados (nome, marca, ano) de cada carro e os salva no arquivo `carros.txt`.
4. **Sair**: Finaliza a execução do programa.

---

## Estrutura do Código

### `struct Carro`

```c
struct Carro {
    char nome[50];
    char marca[50];
    int ano;
};
Essa estrutura representa um carro, contendo:

nome: nome do carro

marca: marca do carro

ano: ano de fabricação

Lógica da Pilha
O vetor pilha[100] simula uma pilha com capacidade para até 100 carros.

A variável topo controla o índice do topo da pilha.

A inserção e leitura dos carros sempre acontece no topo (último elemento adicionado).

Exemplo de Uso
plaintext
Copiar
Editar
--- MENU ---
1. Adicionar carro
2. Mostrar nomes dos carros
3. Imprimir carros 
4. Sair
Digite sua opcao: 1
Digite o nome do carro: Onix
Digite a marca do carro: Chevrolet
Digite o ano de fabricacao: 2022
Carro adicionado com sucesso!
Arquivo de Saída
Se a opção 3 for selecionada, o programa gera o arquivo carros.txt com os dados dos carros, no seguinte formato:
![Captura de Tela (2)](https://github.com/user-attachments/assets/5eaa76f9-59b2-42a5-8c8c-2b089710c224)
![Captura de Tela (3)](https://github.com/user-attachments/assets/4c539bdd-bc8b-44c6-ab6d-a0cee82e64ec)
![Captura de Tela (1)](https://github.com/user-attachments/assets/a1fd0ed8-2466-4fd4-8f2d-013d455c0994)

Copiar
Editar
1. Nome: Onix | Marca: Chevrolet | Ano: 2022
2. Nome: Gol | Marca: Volkswagen | Ano: 2021
Limitações
A pilha comporta até 100 carros.
