---
name: converter-artigo-mdpi-land
description: Converte artigos científicos existentes para a estrutura editorial do template da revista Land (MDPI), preservando conteúdo, dados, citações, tabelas, figuras e referências sem inventar informações.
---

# Skill: Converter artigo científico para o formato MDPI Land

## Objetivo
Transformar um artigo científico fornecido pelo usuário em manuscrito organizado segundo o template da revista **Land (MDPI)**, usando `land-template.dot` como referência de formatação e o artigo-fonte como fonte primária do conteúdo. A tarefa é adaptar a estrutura editorial, não resumir o artigo nem reescrever livremente seus resultados.

## Entradas
- Artigo-fonte, preferencialmente DOCX. PDF também pode ser aceito, mas tabelas, equações e figuras podem exigir inspeção visual.
- Template MDPI Land em DOT ou DOCX.
- Preferências opcionais: idioma final, tipo de artigo, autores correspondentes, limites editoriais e instruções específicas.

Se faltar um arquivo essencial, solicite-o. Se houver vários artigos, identifique o documento principal antes de editar.

## Princípios obrigatórios
1. **Fidelidade ao original:** não inventar dados, métodos, resultados, referências, DOI, financiamento, aprovação ética ou declarações de autoria.
2. **Lacunas explícitas:** usar `[INFORMAÇÃO A CONFIRMAR PELOS AUTORES]` onde informações obrigatórias estiverem ausentes.
3. **Preservação:** manter números, unidades, variáveis, datas, estatísticas, software, fontes de dados e limitações.
4. **Citações rastreáveis:** converter para estilo numérico apenas após associar cada citação à entrada bibliográfica correta. Sinalizar correspondências ambíguas.
5. **Objetos gráficos:** preservar tabelas, figuras, mapas e equações; não inventar valores de elementos ilegíveis.
6. **Separar edição de ciência:** melhorar gramática, clareza e coesão sem alterar interpretação científica não autorizada.
7. **Idioma:** manter o idioma original por padrão. Traduzir somente quando solicitado.
8. **Rastreabilidade:** listar mudanças estruturais relevantes e pendências editoriais.

## Estrutura editorial de referência
A estrutura deve se ajustar ao tipo de manuscrito e às regras oficiais vigentes.

### Elementos iniciais
- Tipo de artigo (Article, Review, Communication etc.).
- Título.
- Autores, afiliações numeradas e autor correspondente.
- Afiliações e e-mails disponíveis.
- Academic Editor, Received, Revised, Accepted e Published: não inventar; manter campos de modelo apenas quando apropriado à etapa editorial.
- Abstract em parágrafo único, com até cerca de 200 palavras conforme o template de referência.
- Keywords: de 3 a 10 termos pertinentes.

### Corpo do artigo
1. **Introduction** — contexto, relevância, estado da arte, lacuna, objetivo e contribuição.
2. **Materials and Methods** — área de estudo, dados, período, variáveis, equipamentos, software, procedimentos, parâmetros e validação, quando aplicáveis.
3. **Results** — resultados observados, números, tabelas, figuras e métricas, sem interpretação não demonstrada.
4. **Discussion** — interpretação, relação com hipóteses e literatura, implicações, limitações e perspectivas.
5. **Conclusions** — síntese apoiada nos resultados e recomendações proporcionais às evidências.
6. **Patents** — somente quando aplicável.
7. **Supplementary Materials** — somente materiais existentes e seus identificadores.
8. **Author Contributions** — taxonomia CRediT baseada em contribuições confirmadas.
9. **Funding** — somente financiamento documentado.
10. **Institutional Review Board Statement / Informed Consent Statement** — somente quando aplicável; não inferir aprovação.
11. **Data Availability Statement** — repositório, DOI, URL ou restrições confirmadas.
12. **Acknowledgments** — agradecimentos fornecidos pelos autores. Declarar uso de IA quando exigido e correspondente ao uso real.
13. **Conflicts of Interest** — declaração fornecida ou pendência para confirmação.
14. **Abbreviations** — quando necessário.
15. **Appendices** — opcionais; garantir chamadas no texto.
16. **References** — numeradas pela ordem de primeira ocorrência, por exemplo `[1]`, `[2,3]`, `[4–6]`; DOI apenas se conhecido e confirmado.
17. **Disclaimer/Publisher’s Note** — somente se exigido e apropriado à versão do manuscrito.

## Mapeamento de seções
| Conteúdo original | Destino sugerido |
|---|---|
| Introdução, problema, justificativa, lacuna e objetivos | 1. Introduction |
| Fundamentação teórica / revisão de literatura | Integrar à Introduction ou organizar em subseções, sem perder argumentos e citações |
| Área de estudo | 2. Materials and Methods, como subseção |
| Materiais, dados, variáveis, software e procedimentos | 2. Materials and Methods |
| Resultados quantitativos, mapas, tabelas e testes | 3. Results |
| Interpretação, comparação com literatura e implicações | 4. Discussion |
| Conclusões, recomendações e trabalhos futuros | 5. Conclusions |
| Resumo e palavras-chave | Abstract e Keywords |
| Referências autor-data | Referências numéricas, após conferência das correspondências |
| Resumos em outros idiomas | Manter apenas se solicitado ou exigido no destino editorial |

Não deslocar conteúdo de modo a mudar seu sentido. Se resultados e discussão estiverem misturados, separar somente quando essa distinção puder ser feita com segurança; caso contrário, registrar a pendência.

## Citações e referências
- Numerar pela ordem de primeira ocorrência no manuscrito final.
- Manter o mesmo número para a mesma fonte em todas as ocorrências.
- Agrupar citações múltiplas de acordo com o padrão numérico do periódico.
- Conferir referências citadas sem entrada e entradas não citadas.
- Não inventar DOI, volume, número, páginas, editora, URL ou data de acesso.
- Só realizar complementação bibliográfica por pesquisa externa quando autorizada, registrando o que foi verificado.
- Incluir citações em legendas e tabelas na ordem correta de ocorrência.

## Figuras, tabelas, mapas e equações
- Posicionar perto da primeira chamada no texto, quando viável.
- Numerar sequencialmente: Figure 1, Table 1, Equations (1), etc.
- Preservar legendas, painéis (a), (b), fontes, notas, unidades, símbolos, casas decimais e significância estatística.
- Não substituir figuras do estudo por imagens genéricas.
- Registrar objetos que não puderem ser recuperados e não deixar marcadores ou imagens quebradas.

## Aplicação do template DOT/DOCX
1. Inspecionar o template e os estilos disponíveis.
2. Usar o template como base quando o ambiente permitir. Se DOT não puder ser aplicado diretamente, trabalhar com uma cópia DOCX convertida, preservando os estilos visuais relevantes.
3. Aplicar os estilos do template a título, autores, afiliações, abstract, keywords, títulos, corpo, legendas, tabelas e referências.
4. Remover instruções de preenchimento, figuras de exemplo e tabelas fictícias.
5. Não remover conteúdo científico para fazer o artigo caber em exemplos visuais.
6. Não tratar DOI provisório nem metadados editoriais de exemplo como definitivos.
7. Entregar DOCX editável; gerar PDF adicional somente se solicitado.

## Fluxo de trabalho
### 1. Diagnóstico
Ler o artigo completo, inspecionar o template e inventariar seções, tabelas, figuras, equações, referências e metadados.

### 2. Plano de conversão
Mapear seções antigas e novas; identificar campos ausentes, citações ambíguas, referências incompletas e objetos sem chamada. Prosseguir com marcadores explícitos onde possível.

### 3. Reorganização
Aplicar a estrutura recomendada, integrar fundamentação teórica quando fizer sentido e mover área de estudo para métodos quando apropriado, sem inventar resultados.

### 4. Ajuste editorial
Revisar título e subtítulos sem mudar escopo; preparar abstract fiel ao conteúdo; selecionar 3–10 keywords; converter citações depois de validar correspondências.

### 5. Formatação
Aplicar estilos; preservar objetos; remover instruções de modelo; registrar inconsistências sem modificar dados.

### 6. Controle de qualidade
- [ ] Título, autores e afiliações preservados.
- [ ] Nenhuma seção científica omitida sem registro.
- [ ] Abstract fiel e próximo do limite recomendado.
- [ ] Figuras e tabelas numeradas e citadas.
- [ ] Citações correspondem à lista de referências.
- [ ] Numeração das referências segue a primeira ocorrência.
- [ ] Valores, unidades, fórmulas e métricas preservados.
- [ ] Nenhum DOI ou declaração foi inventado.
- [ ] Pendências claramente marcadas.
- [ ] DOCX abre corretamente, sem páginas em branco ou objetos quebrados.
- [ ] Documento permanece editável e visualmente consistente.

## Entregáveis
1. Manuscrito DOCX editável.
2. Resumo das mudanças estruturais.
3. Lista de pendências autorais: funding, CRediT, conflito de interesses, disponibilidade de dados, autor correspondente, DOI e dados bibliográficos ausentes.
4. PDF de revisão se solicitado.

## Prompt operacional
“Converta o artigo fornecido para o padrão editorial da revista Land (MDPI), usando o template disponibilizado. Preserve o conteúdo científico, dados, unidades, figuras, tabelas, equações, citações e referências. Reorganize as seções pelo significado, converta citações para numeração MDPI após conferir suas correspondências e aplique os estilos do template. Não invente metadados ou declarações. Marque informações ausentes como `[INFORMAÇÃO A CONFIRMAR PELOS AUTORES]`. Remova instruções e exemplos do template. Faça a verificação final e entregue DOCX editável, resumo de mudanças e pendências.”
