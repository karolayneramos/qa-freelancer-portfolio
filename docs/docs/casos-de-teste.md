# Casos de Teste — Aplicativo de Gestão de Tarefas

## Objetivo

Documentar exemplos de cenários utilizados para avaliar o comportamento de um aplicativo de gestão de tarefas.

Os exemplos abaixo são modelos de documentação para o portfólio. Eles não representam necessariamente todos os casos executados durante o trabalho original.

## Caso de teste CT-001 — Cadastro de tarefa

**Objetivo:** Verificar se o sistema permite cadastrar uma tarefa com dados válidos.

**Pré-condição:** Usuário autenticado no sistema.

**Passos:**
1. Acessar a área de tarefas.
2. Selecionar a opção de criar uma nova tarefa.
3. Preencher os campos obrigatórios com dados válidos.
4. Salvar a tarefa.

**Resultado esperado:** A tarefa deve ser salva e apresentada na lista de tarefas.

## Caso de teste CT-002 — Campo obrigatório vazio

**Objetivo:** Verificar a validação de campos obrigatórios no cadastro de tarefa.

**Pré-condição:** Usuário autenticado no sistema.

**Passos:**
1. Acessar o formulário de cadastro de tarefa.
2. Deixar um campo obrigatório vazio.
3. Tentar salvar a tarefa.

**Resultado esperado:** O sistema deve informar que o campo obrigatório precisa ser preenchido e impedir o cadastro inválido.

## Caso de teste CT-003 — Consulta de tarefas

**Objetivo:** Verificar se o usuário consegue visualizar as tarefas cadastradas.

**Pré-condição:** Existência de tarefas cadastradas para o usuário.

**Passos:**
1. Acessar a área de tarefas.
2. Consultar a lista apresentada.
3. Verificar se as tarefas cadastradas estão visíveis.

**Resultado esperado:** O sistema deve apresentar corretamente as tarefas disponíveis para o usuário.

## Observação

Estes são exemplos ilustrativos de casos de teste. Para representar fielmente o trabalho freelancer, os casos deverão ser substituídos ou complementados pelos cenários realmente executados e autorizados para divulgação.
