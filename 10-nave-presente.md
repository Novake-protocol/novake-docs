# Nave Presente

A Nave Presente é uma Nave NFT oferecida gratuitamente pelo protocolo a utilizadores seleccionados.

## Para que Serve

- Activação de líderes e parceiros estratégicos
- Recompensa por performance ou missões especiais
- Teste real do protocolo sem capital do utilizador

## Como Funciona

A Nave Presente funciona como uma Nave normal, com algumas diferenças importantes:

| Comportamento | Nave Comprada | Nave Presente |
|---|---|---|
| Paga USDC para adquirir | ✅ Sim | ❌ Não (dada pelo admin) |
| Gera Bônus de Embarque para o sponsor | ✅ Sim | ❌ Não |
| Gera pontos de Constelação | ✅ Sim | ❌ Não |
| Pode sacar capital principal | ✅ Sim | ❌ Bloqueado on-chain |
| Saque máximo de Spoils | Ilimitado (yield real) | Cap por Patente |
| Após atingir cap | Continua ativa | Nave vai a RETIRED |

## Caps de Saque por Patente

| Patente do titular | Cap máximo de Spoils |
|---|---|
| Cadete | $200 |
| Sargento | $300 |
| Comandante | $400 |
| Supremo | $500 |

Quando o cap é atingido → a Nave vai automaticamente para **RETIRED** e a Expedição encerra. O NFT fica na wallet.

## Onde Ver

Se tens uma Nave Presente, aparece na sidebar um item especial **"Nave Presente"** que leva à página `/nave-presente`.

Lá vês:
- O estado da tua Nave GIFTED
- Spoils disponíveis para claim
- Quanto já retiraste vs cap disponível
- Opção de lançar Expedição (Tripulante — sem gerar bônus de rede)

## Proteção On-Chain

O contrato `NovaKTreasury` tem proteção explícita:

```solidity
error GiftedShipCannotWithdrawCapital();
```

Qualquer tentativa de sacar o capital principal de uma Nave Presente reverte na blockchain — impossível de contornar, mesmo com acesso direto ao contrato.
