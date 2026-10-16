# Prompt — Classificação e preenchimento da ficha de triagem

## Objetivo
Orientar a IA a analisar um relato fictício, sugerir uma categoria usando a tabela de assuntos e produzir uma ficha de triagem administrativa preenchida.

## Arquivos de referência
- `apoio/clientes_ficticios.md`
- `apoio/tabela_assuntos.md`
- `saida/fichas_triagem/modelo_ficha.md`
- `docs/protocolo.md`

## Instrução enviada à IA

Leia os arquivos de referência acima. Utilize apenas o relato fictício selecionado em `apoio/clientes_ficticios.md` e compare-o com as categorias e regras descritas em `apoio/tabela_assuntos.md`.

Para o atendimento escolhido:

1. Identifique o código e o nome fictício do cliente.
2. Resuma o relato de forma neutra, sem acrescentar fatos que não estejam no arquivo.
3. Sugira a categoria que melhor corresponde à tabela de assuntos e explique brevemente o motivo.
4. Identifique informações ausentes que precisam ser confirmadas.
5. Avalie se há algum sinal de urgência com base somente nas informações disponíveis. Não invente prazo ou urgência.
6. Preencha todos os campos possíveis do modelo `saida/fichas_triagem/modelo_ficha.md`. Para dados não informados, escreva “Não informado — confirmar”.
7. Inclua uma recomendação de encaminhamento administrativo, indicando qual responsável deve revisar o caso.
8. Sinalize qualquer exceção que exija revisão humana.

Limites obrigatórios:
- A classificação é preliminar e administrativa, não um parecer jurídico.
- Não invente leis, prazos, documentos, fatos ou informações pessoais.
- Não declare que o escritório aceitou o caso.
- Não forneça orientação jurídica à pessoa atendida.
- A ficha final deve deixar claro que a classificação e o encaminhamento dependem da revisão de um advogado.
- Use apenas os dados fictícios do projeto.

## Atendimento escolhido para o teste
CLI-001 — Marina Exemplo.

## Onde registrar a saída
Salve a resposta produzida pela IA em `saida/fichas_triagem/triagem_CLI-001.md`. Depois, confira a resposta e registre a revisão humana em `evidencias/revisao_humana.md`.
