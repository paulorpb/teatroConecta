# Guia de Contribuição

Este documento define como a equipe deve colaborar neste repositório.

## Participação de todos os integrantes

Todos os integrantes devem realizar **contribuições reais** — em documentação, protótipo, código, testes ou dados.

> O histórico de commits poderá ser utilizado pelo professor como uma das evidências de participação dos integrantes.

Recomendações:

- cada integrante deve fazer commits **com a sua própria conta** do GitHub;
- configure seu nome e e-mail no Git antes de começar:

  ```bash
  git config --global user.name "Seu Nome"
  git config --global user.email "seu-email@exemplo.com"
  ```

- evite que uma única pessoa envie o trabalho de todos.

## Padrão de commits

Use uma versão simplificada do **Conventional Commits**: `tipo: descrição curta no imperativo/presente`.

| Tipo | Quando usar |
|---|---|
| `docs` | Documentação (arquivos em `docs/`, README etc.) |
| `feat` | Nova funcionalidade |
| `fix` | Correção de erro |
| `test` | Criação ou ajuste de testes |
| `refactor` | Reorganização de código sem mudar comportamento |
| `chore` | Tarefas de manutenção (configuração, dependências etc.) |

Exemplos de mensagens:

```text
docs: descreve problema escolhido
docs: adiciona requisitos
feat: adiciona cadastro de usuário
feat: implementa mapa
fix: corrige autenticação
test: adiciona testes do cadastro
refactor: reorganiza serviço de dados
```

Boas práticas:

- faça commits **pequenos, frequentes e descritivos**;
- cada commit deve tratar de **um assunto**;
- evite mensagens genéricas como `update`, `ajustes` ou `commit final`.

## Fluxo de trabalho sugerido

1. Crie uma **issue** para cada tarefa (use os modelos em **Issues → New issue**).
2. Crie uma **branch** para a tarefa:

   ```bash
   git checkout -b docs/requisitos
   ```

3. Faça commits na branch.
4. Envie a branch e abra um **Pull Request** para `main`:

   ```bash
   git push -u origin docs/requisitos
   ```

5. Peça a revisão de outro integrante antes de fazer o merge.

> Para projetos pequenos, o professor pode permitir commits diretamente na `main`. Mesmo assim, mantenha commits pequenos e descritivos.

## Segurança

**NUNCA** versione:

- senhas;
- tokens;
- API keys;
- credenciais;
- arquivos `.env`;
- dados pessoais sensíveis.

Se a aplicação precisar de variáveis de ambiente:

1. use um arquivo `.env` **local** (já ignorado pelo `.gitignore`);
2. crie um `.env.example` com os **nomes** das variáveis e valores fictícios, por exemplo:

   ```text
   DATABASE_URL=coloque_aqui_a_url_do_banco
   API_KEY=coloque_aqui_sua_chave
   ```

3. **nunca** coloque valores reais no `.env.example`.

Se uma credencial for enviada por engano ao GitHub, **considere-a comprometida**: revogue/troque a credencial imediatamente e avise o professor. Apenas apagar o arquivo em um novo commit **não** remove a credencial do histórico.
