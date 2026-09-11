# Código-fonte (`src/`)

Todo o **código-fonte do MVP** deverá ficar dentro desta pasta.

> **Avaliação:** AV2. Na AV1 esta pasta pode permanecer apenas com este arquivo.

## Organização

**Não existe uma estrutura tecnológica obrigatória.** A organização depende das tecnologias escolhidas em [06-arquitetura-e-tecnologias.md](../docs/06-arquitetura-e-tecnologias.md).

Os exemplos abaixo são **apenas ilustrativos**:

**Exemplo 1** — frontend e backend separados:

```text
src/
├── frontend/
├── backend/
└── database/
```

**Exemplo 2** — aplicação web simples:

```text
src/
├── app.py
├── templates/
└── static/
```

**Exemplo 3** — aplicação organizada por componentes:

```text
src/
├── components/
├── pages/
├── services/
└── api/
```

## Boas práticas

- documente no [README principal](../README.md#como-executar-o-projeto) como instalar e executar o projeto;
- registre as dependências em um arquivo apropriado (por exemplo, `requirements.txt`, `package.json` ou equivalente);
- use variáveis de ambiente para configurações sensíveis e forneça um `.env.example` **sem valores reais**;
- **nunca** versione senhas, tokens, chaves de API ou arquivos `.env`;
- não versione pastas geradas automaticamente (`node_modules/`, `venv/`, `build/` etc.) — elas já estão no `.gitignore`.

## Descrição do código (preencher na AV2)

_Explique brevemente a organização das pastas e arquivos do código da equipe._
