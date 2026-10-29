# Guia de uso

## Para que serve
A skill ajuda a adaptar a estrutura de um artigo científico para o modelo editorial de *Land* (MDPI), preservando conteúdo, dados e referências. É útil quando o texto original utiliza seções diferentes, como “Fundamentação Teórica” e “Área de Estudo”.

## Arquivos necessários
- Artigo original em DOCX, de preferência com tabelas e imagens incorporadas.
- Template editorial da revista em DOT ou DOCX.
- Preferências: idioma, tipo de manuscrito e necessidade de tradução ou apenas reorganização.

O template de referência deve ser conferido quanto à versão; não presumir que todo arquivo local seja a versão atual.

## Como executar
1. Use `SKILL.md` como instrução do agente ou do fluxo de trabalho.
2. Anexe o artigo e o template.
3. Use o [prompt operacional](../prompts/PROMPT_CONVERSAO.md).
4. Revise o DOCX gerado e as pendências com os autores.

## O que a skill deve fazer
- Inventariar seções, figuras, tabelas, equações e referências.
- Mapear as seções existentes para o destino editorial.
- Preservar teor científico e resultados.
- Ajustar abstract e keywords sem acrescentar resultados.
- Converter citações e referências após conferir cada associação.
- Aplicar estilos do template e remover exemplos instrucionais.
- Relatar mudanças e pendências.

## O que não deve fazer
- Inventar financiamento, aprovação ética, autoria, conflito de interesses ou DOI.
- Criar referências bibliográficas inexistentes.
- Alterar números para resolver divergências aparentes.
- Substituir figuras por ilustrações genéricas.
- Declarar o artigo pronto para submissão sem revisão humana.

## Marcadores para informações ausentes
Use `[INFORMAÇÃO A CONFIRMAR PELOS AUTORES]` e repita cada pendência no relatório final.

## Entregáveis esperados
- Manuscrito DOCX editável.
- Resumo das alterações estruturais.
- Lista de pendências.
- PDF de conferência, se solicitado.

## Revisão final
Compare a quantidade de figuras, tabelas e referências do original com a versão convertida. Inspecione as citações, o idioma, os termos técnicos, as quebras de página, as tabelas extensas e os objetos gráficos. Antes da submissão, consulte as instruções oficiais vigentes de *Land*.
