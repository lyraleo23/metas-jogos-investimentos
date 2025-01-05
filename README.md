# Metas de Jogos

Este é um projeto pessoal com a ideia de que a cada dia eu incremento a meta de troféus. Ao ganhar um troféu, a meta diminui e a dívida aumenta. A dívida é um valor (dinheiro) que devo investir ou aplicar a cada troféu ganho.

## Função Principal

A função principal gerencia a planilha de metas de jogos. Ela verifica se o arquivo Excel `metas_jogos.xlsx` existe e, caso não exista, cria um novo workbook. Em seguida, verifica a quantidade de linhas na planilha e adiciona os dados de metas diárias e dívidas. Se a data atual já estiver registrada, não adiciona novos dados.

### Variáveis

- **meta_diaria** (int): Meta diária de troféus.
- **meta_trofeus** (int): Total de troféus acumulados.
- **divida** (int): Dívida acumulada.
- **data_atual** (str): Data atual no formato "dd/mm/yyyy".

### Exceções

- **FileNotFoundError**: Se o arquivo `metas_jogos.xlsx` não for encontrado, cria um novo workbook.

### Ações

- Adiciona dados na planilha se a data atual for diferente da última registrada.
- Salva o arquivo Excel com os dados atualizados.

### Prints

- Informa a quantidade de linhas na planilha.
- Informa se a data atual já foi registrada.
- Informa o sucesso ao salvar a planilha com as metas e dívidas atualizadas.
