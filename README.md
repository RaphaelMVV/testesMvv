# Testes Sistemas MVV

Este repositório centraliza evidências e relatórios de teste dos sistemas do MVV.

## Convenção de nomes

- Este repositório usa `snake_case` nas pastas e na estrutura.
- Priorizar a convenção usada no seu time ou empresa.
- Usar datas no formato `AAAA-MM-DD`.
- Evitar mistura de padrões dentro da mesma categoria de arquivo.

## Padrão adotado

- Pastas, imagens técnicas e relatórios Markdown usam `snake_case`: `testes_app_portal_aluno`, `login_app_portal_aluno.jpeg`, `relatorio_de_testes_app_alumni_2026-04-14.md`
- As pastas de sistema usam o prefixo `testes_` para não confundir com os repositórios originais dos aplicativos.
- PDFs podem usar nome legível, com espaço e letra maiúscula: `Relatório de Testes App Alumni - 2026-04-14.pdf`

## Estrutura

Cada sistema fica em sua própria pasta:

- `testes_app_alumni/`
- `testes_app_portal_aluno/`
- `testes_church_app/`
- `testes_sistema_igrejas_gerenciador/`

Dentro de cada sistema:

- problemas em acompanhamento devem ficar em `acompanhamento/`
- relatórios PDF devem ficar em `relatorios/<data>/`
- cada pasta de data pode conter o relatório em Markdown, `documentos/` e `imagens/`
- a data da pasta representa a data final do relatório, ou seja, a data de entrega/conclusão
- o período completo do teste, incluindo data inicial e data final, deve ficar descrito dentro do relatório

Modelos reutilizáveis ficam na pasta `modelos/`.

## Exemplo

```text
testes_app_alumni/
  acompanhamento/
    erros_persistentes.md
    erros_corrigidos.md
  relatorios/
    2026-04-14/
      relatorio_de_testes_app_alumni_2026-04-14.md
      documentos/
        Relatório de Testes App Alumni - 2026-04-14.pdf
      imagens/
```

## Quando a data não estiver definida

Se você ainda não souber a data correta do relatório, pode usar:

- `relatorios/data_nao_informada/`

Depois, é só mover o arquivo para a pasta da data certa.

## Sobre a data da pasta

A data usada na pasta do relatório é a data de entrega ou conclusão do relatório.

Ela não precisa representar necessariamente o primeiro dia de teste. Se o teste começou em uma data e terminou em outra, esse intervalo deve aparecer no conteúdo do relatório em `.md` e no PDF.

Exemplo:

```text
relatorios/
  2026-04-14/
    relatorio_de_testes_app_alumni_2026-04-14.md
```

Nesse caso, `2026-04-14` indica a data final/de entrega do relatório.

## Padrão de cada relatório

```text
relatorios/
  AAAA-MM-DD/
    relatorio_nome_do_sistema_AAAA-MM-DD.md
    documentos/
      Relatório Nome do Sistema - AAAA-MM-DD.pdf
    imagens/
      imagem_ou_evidencia.png
```

Use o arquivo `.md` como versão editável e legível no GitHub. Use o PDF como versão final para compartilhar no Drive.

## Modelo de relatório

Use [modelo_relatorio_de_testes.md](modelos/modelo_relatorio_de_testes.md) como base para novos relatórios.

Esse modelo combina:

- `Informações Gerais` e `Resumo Executivo`, inspirados no relatório do App Alumni.
- Estrutura detalhada dos pontos, com `Título`, `Ambiente`, `Descrição`, `Passos para reproduzir`, `Resultado obtido`, `Impacto` e `Evidências`, inspirada no relatório do Sistema Igrejas.

## Acompanhamento de erros

Cada sistema pode ter uma pasta `acompanhamento/` com dois arquivos:

- `erros_persistentes.md`: problemas que ainda precisam ser acompanhados ou revalidados.
- `erros_corrigidos.md`: problemas que já foram confirmados como corrigidos em uma nova rodada de testes.

Quando um problema for corrigido, mova o item de `erros_persistentes.md` para `erros_corrigidos.md`, informando a data ou origem da confirmação. Os relatórios por data devem permanecer como histórico.
