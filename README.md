# padrao-de-git-commit
Definição de um padrão de estilo para escrita das mensagens do git commit e Pull Requests.

# Padrão de Estilo para Mensagens Git

## Mensagens de commit

- Na primeira linha resuma o commit em no máximo 72 caracteres (O commit pelo PyCharm já ajuda nisso);
- Use SEMPRE o modo imperativo ("Adiciona feature" e não "Adicionando feature" ou "Adicionada feature");
- Inicie as frases com letras maiúsculas;
- Não termine a linha de resumo com ponto final (.);
- Use uma linha em branco para separar a linha de resumo do corpo da mensagem;
- Considere descrever com detalhes no corpo do commit (limitadas a 72 caracteres por linha)
- No corpo explique "o que" e "por que" e não o "como";
- Considere usar um emoji no início da mensagem de commit

Emoji | Code | Commit Type
------------ | ------------- | -------------
:tada: | `:tada:` | initial commit
:art: | `:art:` | quando melhorar a estrutura/formato do código
:racehorse: | `:racehorse:` | quando melhorar a performance
:memo: | `:memo:` | quando escrever alguma documentação
:bug: | `:bug:` | quando corrigir um bug
:fire: | `:fire:` | quando remover códigos ou arquivos
:green_heart: | `:green_heart:` | quando corrigir uma build no CI
:white_check_mark: | `:white_check_mark:` | quando adicionar testes
:lock: | `:lock:` | quando melhorar a segurança
:arrow_up: | `:arrow_up:` | quando der upgrade em dependências
:arrow_down: | `:arrow_down:` | quando der downgrade em dependências
:poop: | `:poop:` | deprecated
:construction: | `:construction:` | em construção
:rocket: | `:rocket:` | nova feature
:see_no_evil: | `:see_no_evil:` | gambiarra
:gift: | `:gift:` | nova versão

### Exemplo
```bash
git commit -m ":memo: Adiciona instruções sobre commits
>
> Foi criado o arquivo README.md com as instruções de
> como fazer um bom commit"
``` 

## Por que uma boa mensagem importa?
### Alguns motivos:
- Caso um bug seja introduzido, uma boa mensagem de commit facilita a identificação de onde/quando isso aconteceu;
- Se você reverter um commit, a mensagem será Revert "mensagem original", deixando claro o que está sendo revertido;
- Boas mensagens se tornam útias ao exibir listas de commits através de comandos como git blame, git log, git shortlog, etc.
