# clipfloor — o piso de pagamento das campanhas de clipagem

Página pública e gratuita que responde, com dados medidos, a pergunta que todo clipador faz:
**quanto paga clipagem por 1000 visualizações?**

A resposta curta é que o CPM não decide nada. O que decide é o **piso**:

```
piso = pagamento_mínimo ÷ CPM × 1000
```

Quantas views UM post precisa para render o primeiro centavo. Abaixo do piso, o pagamento
arredonda para zero por mais clipes que se faça.

## O que tem aqui

- Uma **calculadora** do piso (roda no navegador, sem servidor).
- A tabela das **46 campanhas** que estavam no ar em 04/09/2026, com **118 faixas de
  pagamento** (campanha × rede) e o piso de cada uma já calculado.
- Os números: piso mediano de **1.429 views**; de 118 faixas, **uma** paga desde a primeira view.

## De onde vieram os dados

Das páginas públicas das próprias campanhas, lidas uma a uma. Nenhum número foi estimado —
campanha que não mostrava a tabela ficou de fora em vez de virar chute.

É um retrato de um dia. Campanhas mudam de tabela toda semana; refaça a conta na campanha que
você for pegar. A fórmula é que não muda.

## Aviso

Isto é uma calculadora, não uma promessa de renda. Ela diz quais campanhas são matematicamente
inviáveis para o tamanho de conta de hoje. Não gera views para ninguém.

## Estrutura

```
docs/index.html   página (estática, sem rastreador, sem cookie)
docs/dados.json   as 46 campanhas / 118 faixas
```
