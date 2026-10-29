# Skill: Converter artigo científico para o formato MDPI Land

> Skill de apoio editorial para reorganizar manuscritos conforme o template da revista *Land* (MDPI), preservando a integridade científica.

## Comece por aqui
- [Guia de uso](docs/GUIA_DE_USO.md)
- [Definição completa da skill](SKILL.md)
- [Mapa da estrutura editorial](docs/ESTRUTURA_EDITORIAL.md)
- [Checklist de qualidade](docs/CHECKLIST.md)
- [Prompt operacional](prompts/PROMPT_CONVERSAO.md)
- [Inventário dos artefatos](ARTIFACTS.md)
- [Histórico de alterações](CHANGELOG.md)

## Objetivo
Transformar um artigo científico existente em manuscrito organizado segundo o template da revista *Land* (MDPI). A skill orienta o mapeamento das seções, preservação de tabelas e figuras, normalização de citações e referências e verificação editorial final.

**A skill não substitui a avaliação dos autores nem as instruções oficiais vigentes da revista.** Informações ausentes devem ser confirmadas, nunca inventadas.

## Fluxo resumido
1. Disponibilize o artigo original, preferencialmente em DOCX, e o template DOT/DOCX.
2. Aplique as instruções de `SKILL.md`.
3. Reorganize o conteúdo mantendo dados, métodos, resultados, tabelas, figuras e citações.
4. Confira referências e declarações obrigatórias.
5. Revise o DOCX final e valide as instruções atuais do periódico.

## Estrutura
```text
.
├── README.md
├── SKILL.md
├── ARTIFACTS.md
├── CHANGELOG.md
├── LICENSE
├── docs/
├── prompts/
├── templates/
├── examples/
└── artifacts/
```

## Integridade científica
Preservar números, unidades, métodos e conclusões. Usar `[INFORMAÇÃO A CONFIRMAR PELOS AUTORES]` para lacunas. Não inventar DOI, financiamento, aprovação ética, contribuições CRediT, conflito de interesses ou referências bibliográficas.

## Formatos
- Entrada preferencial: DOCX.
- Template de referência: DOT/DOCX.
- Saída: DOCX editável; PDF opcional quando solicitado.
- Idioma original mantido por padrão; tradução somente quando solicitada.

## Exemplo de comando
> Use a skill deste repositório para converter o artigo anexado ao padrão editorial do template *Land* (MDPI). Preserve o conteúdo científico, confira as referências, aplique os estilos e entregue um DOCX editável, acompanhado de resumo das mudanças e pendências autorais.

Consulte [LICENSE](LICENSE). A licença deste repositório não concede automaticamente direitos sobre templates de terceiros ou artigos de exemplo.
