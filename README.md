# API de Produtividade de Funcionários com Flask

Este projeto é uma API simples criada com **Python** e **Flask**, que simula um sistema de **monitoramento de produtividade de funcionários**. Ele armazena dados de setores, funcionários e tarefas, e permite consultar essas informações via rotas HTTP no formato JSON.

---

## Funcionalidades

- **Setores**
  - Lista todos os setores cadastrados.

- **Funcionários**
  - Os funcionários estão associados a setores e possuem cargos específicos.
  - Dados são inseridos automaticamente ao iniciar o sistema.

- **Tarefas**
  - Cada tarefa está vinculada a um funcionário e contém:
    - Nome da tarefa
    - Data de execução
    - Tempo gasto (em horas)
  - Consulta de tarefas traz também o nome do setor e do funcionário.

---

## Estrutura do Banco de Dados (SQLite)

O banco de dados `produtividade.db` é criado automaticamente com as seguintes tabelas:

- `setores (id, nome)`
- `funcionarios (id, nome, setor_id, cargo)`
- `tarefas (id, funcionario_id, nome, data, tempo_gasto)`

Com dados fictícios já inseridos para teste.

---

## Como Executar

1. Instale o Flask:
   ```bash
   pip install flask
