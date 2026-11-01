# Sistema de Encomendas da Biblioteca

Sistema em linha de comando, escrito em C, que simula o fluxo de pedidos de livros dentro de uma biblioteca, do pedido do aluno até a entrega.

## Como funciona

O sistema tem três perfis de acesso:

| Perfil | O que faz |
|---|---|
| **Estagiário** | Registra pedidos de alunos (nome, matrícula e descrição) e lista os pedidos |
| **Secretário** | Transforma um pedido em encomenda, com localização do livro, destino e prioridade |
| **Transportador** | Lista as encomendas e dá baixa nas retiradas |

## Estruturas de dados

- **Árvore binária de busca** para os pedidos, indexados por ID
- **Lista encadeada** para as encomendas e para os usuários

## Arquivos

- `main.c` — ponto de entrada
- `functions_menu.h` — menus de cada perfil
- `functions_pedidos.h` — operações de pedidos, encomendas e usuários
- `structs_pedidos.h` / `structs_usuarios.h` — definição das estruturas

## Como rodar

```bash
gcc main.c -o sistema
./sistema
```

Os usuários de teste são carregados direto no código (`carrega_usuarios`), todos com dados fictícios.

---
Projeto acadêmico de Estrutura de Dados.
