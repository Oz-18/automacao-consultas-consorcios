# Arquitetura proposta para uma futura demonstração

Esta é uma proposta de organização, não uma descrição de implementação verificada. Ela deverá ser ajustada após a revisão do código original autorizado.

## Fluxo conceitual

```text
Entrada sintética
      ↓
Validação da entrada
      ↓
Navegação com Playwright em ambiente de demonstração
      ↓
Organização do resultado
      ↓
Revisão humana
```

## Responsabilidades sugeridas

| Etapa | Responsabilidade pretendida |
| --- | --- |
| Entrada | Receber somente identificadores fictícios na demonstração pública. |
| Validação | Identificar entradas incompletas ou inválidas antes da navegação. |
| Navegação | Executar ações em ambiente autorizado, com limites e tratamento de falhas. |
| Resultado | Organizar apenas os campos necessários, sem registrar dados sensíveis. |
| Revisão | Permitir que uma pessoa confira o resultado e as limitações. |

## Decisões ainda pendentes

- Formato de entrada e saída.
- Organização dos módulos e dependências.
- Estratégia de espera, repetição e recuperação de falhas.
- Forma de testar sem acessar sistemas privados.
- Necessidade de uma demonstração local inteiramente sintética.

Não há endereço de portal, seletor, credencial ou instrução de acesso a sistemas privados nesta proposta.
