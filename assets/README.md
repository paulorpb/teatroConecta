# Recursos visuais (`assets/`)

Esta pasta armazena os **recursos visuais** utilizados na documentação do projeto.

## Utilização

- imagens;
- diagramas;
- screenshots;
- arquitetura;
- capturas do protótipo;
- recursos da documentação.

## Boas práticas

- use nomes de arquivos descritivos, em minúsculas e sem espaços, por exemplo:

  ```text
  prototipo-tela-inicial.png
  diagrama-arquitetura.png
  mvp-fluxo-principal.png
  ```

- prefira formatos leves (`.png`, `.jpg`, `.svg`);
- evite arquivos muito grandes;
- **não** publique imagens com dados pessoais (nomes, rostos, documentos, telefones) sem autorização.

## Como referenciar uma imagem na documentação

Em um arquivo dentro de `docs/`:

```markdown
![Descrição da imagem](../assets/nome-do-arquivo.png)
```

No `README.md` da raiz:

```markdown
![Descrição da imagem](assets/nome-do-arquivo.png)
```
