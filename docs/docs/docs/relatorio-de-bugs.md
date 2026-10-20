# Relatório de Bugs — Testes Manuais

## Sobre este documento

Este documento apresenta exemplos de defeitos identificados durante testes manuais em um aplicativo de gestão de tarefas.

Os registros foram organizados para demonstrar a documentação de problemas, incluindo comportamento esperado, comportamento observado e passos para reprodução. Informações confidenciais foram omitidas.

## BUG-001 — Data da tarefa salva incorretamente

**Categoria:** Manipulação de datas

**Descrição:** Após salvar uma tarefa, a data apresentada pelo sistema ficou um dia anterior à data selecionada.

**Passos para reprodução:**
1. Acessar o formulário de cadastro ou edição de tarefa.
2. Selecionar uma data para o prazo.
3. Salvar a tarefa.
4. Consultar novamente a tarefa salva.

**Resultado esperado:** A data selecionada deve ser mantida após salvar.

**Resultado observado:** A data apresentada ficou um dia anterior à data selecionada.

**Impacto:** Pode causar confusão sobre o prazo real da tarefa.

## BUG-002 — Campo de e-mail aceita formato inválido

**Categoria:** Validação de formulário

**Descrição:** O campo de e-mail permitiu inserir um valor fora do formato esperado de um endereço de e-mail.

**Passos para reprodução:**
1. Acessar o formulário que contém o campo de e-mail.
2. Inserir um texto sem formato válido de e-mail.
3. Tentar salvar o formulário.

**Resultado esperado:** O sistema deve validar o formato do e-mail e informar quando o valor for inválido.

**Resultado observado:** O campo aceitou um valor em formato inválido.

**Impacto:** Pode permitir o cadastro de dados inconsistentes.

## BUG-003 — Mensagem de lista vazia exibida durante o carregamento

**Categoria:** Experiência do usuário e carregamento

**Descrição:** Durante o carregamento da lista, o sistema exibiu a mensagem de que nenhuma tarefa havia sido encontrada. Após o carregamento terminar, as tarefas apareceram normalmente.

**Passos para reprodução:**
1. Acessar a área de listagem de tarefas.
2. Observar a tela enquanto os dados estão sendo carregados.
3. Aguardar o carregamento terminar.

**Resultado esperado:** Durante a busca dos dados, o sistema deve indicar que está carregando. A mensagem de lista vazia deve aparecer apenas quando não houver tarefas após a consulta.

**Resultado observado:** A mensagem de nenhuma tarefa encontrada apareceu temporariamente, embora as tarefas tenham sido exibidas após o carregamento.

**Impacto:** Pode levar o usuário a interpretar incorretamente o estado da listagem.

