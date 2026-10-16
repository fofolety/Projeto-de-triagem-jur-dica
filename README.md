# Projeto 01 — Triagem administrativa de um escritório de advocacia

## Objetivo
Organizar o primeiro atendimento administrativo do escritório, registrando as informações essenciais, classificando o assunto em uma categoria predefinida e encaminhando o caso para análise de um advogado responsável.

A triagem é **administrativa e preliminar**. Não substitui consulta jurídica, análise documental, definição de estratégia ou orientação de advogado.

## Fluxo de atendimento
1. Receber a pessoa com cordialidade e explicar que o primeiro contato serve para registrar informações.
2. Coletar apenas os dados mínimos necessários, conforme `apoio/clientes_ficticios.md`.
3. Registrar o assunto em linguagem simples, sem formular conclusões jurídicas.
4. Consultar `apoio/tabela_assuntos.md` para sugerir uma categoria.
5. Verificar urgência, prazos, audiências, intimações e riscos imediatos.
6. Preencher uma ficha usando o modelo em `saida/fichas_triagem/modelo_ficha.md`.
7. Encaminhar ao advogado ou associado responsável. Nenhuma resposta jurídica ou confirmação de contratação deve ser dada pela equipe administrativa.

## Estrutura do repositório
```text
projeto-01-triagem-juridica/
├── README.md
├── apoio/
│   ├── clientes_ficticios.md
│   └── tabela_assuntos.md
├── docs/
│   ├── protocolo.md
│   └── registro.md
├── prompts/
│   └── consulta_triagem.md
├── evidencias/
│   ├── registro_execucao.md
│   └── revisao_humana.md
└── saida/
    └── fichas_triagem/
        ├── modelo_ficha.md
        └── triagem_CLI-001.md
```

## Regras essenciais
- Utilize dados fictícios em testes e exemplos.
- Não solicite nem registre senhas, códigos de autenticação ou dados que não sejam necessários ao primeiro atendimento.
- Não prometa resultados, não estime chances de êxito e não interprete documentos como se fosse advogado.
- Se houver prazo próximo, risco à integridade física, bloqueio de valores essenciais, ordem judicial, conflito de interesses ou situação fora da tabela, encaminhe imediatamente para revisão humana.
- Restrinja o acesso às fichas às pessoas autorizadas e siga as regras internas de sigilo e proteção de dados.
- Antes de compartilhar documentos ou informações, confirme a identidade da pessoa e a autorização para o compartilhamento, conforme o protocolo interno.

## Limites
A classificação gerada na triagem é apenas uma sugestão administrativa. O advogado responsável confirma a categoria, verifica conflitos de interesses, avalia documentos e decide o encaminhamento adequado.


## Demonstração do uso de IA
O prompt em `prompts/consulta_triagem.md` orienta a IA a consultar o relato fictício, comparar o caso com `apoio/tabela_assuntos.md` e gerar uma ficha preenchida. A ficha demonstrativa está em `saida/fichas_triagem/triagem_CLI-001.md`.

O registro em `evidencias/registro_execucao.md` deve ser preenchido com a ferramenta, data e ambiente realmente utilizados. Para comprovar uma execução real, anexe capturas de tela da interação e da ficha final. A classificação é preliminar e depende de revisão humana.
