# O Hangar — Compra de Naves

O Hangar é onde escolhes e compras a tua Nave NFT. Cada Nave tem um preço em USDC e características únicas.

## As 11 Naves

| # | Nome | Tier | Preço USDC | Preço $NVKE |
|---|------|------|-----------|------------|
| 0 | DRONE | TEST | $5 | — |
| 1 | VYRA | EXPLORER | $10 | — |
| 2 | KOMET | EXPLORER | $50 | — |
| 3 | NEX | EXPLORER | $100 | — |
| 4 | AXION | VANGUARD | $300 | — |
| 5 | PULSAR | VANGUARD | $500 | — |
| 6 | ASTRON | VANGUARD | $700 | — |
| 7 | KRYON | ELITE | $1.000 | — |
| 8 | VORTIS | ELITE | $1.500 | — |
| 9 | EXODUS | LEGENDARY | $2.500 | — |
| 10 | KRAKEN | LEGENDARY | $5.000 | — |

> **Regra de Ouro:** UMA NAVE = UMA EXPEDIÇÃO. Após a Expedição encerrar, a Nave fica RETIRED. O NFT permanece na tua wallet para colecionar.

## Como Comprar

### Pré-requisitos
1. Conta criada e sessão ativa no dApp
2. Wallet MetaMask conectada com saldo USDC na rede Base
3. LaunchGate aberto pelo Dante (Comandante Supremo)

### Fluxo Passo a Passo

**1.** Acede ao **Hangar** (`/hangar`) na sidebar

**2.** Escolhe a tua Nave — visualiza as stats: HULL, THRUST, RANGE, CARGO

**3.** Clica em **EMBARCAR**

**4.** O dApp pede ao backend um **voucher assinado** (EIP-191) com o preço, nonce e prazo

**5.** A tua MetaMask pede para aprovar o gasto de USDC:
   - Valor = preço da Nave + 2% fee de plataforma

**6.** A tua MetaMask pede para confirmar a transação `embark()` no contrato `NovaKTreasury`

**7.** A transação é confirmada na Base L2 (~2 segundos)

**8.** O backend regista a Nave no sistema e processa os bônus

**9.** A Nave aparece na tua frota como **DOCKED** (pronta para Expedição)

## Distribuição do USDC na Compra

Quando compras uma Nave de $1.000 USDC:

| Destino | % | Valor |
|---------|---|-------|
| Capital do utilizador (NovaKTreasury) | 91% | $910 |
| Split 1 | 0,5% | $5 |
| Split 2 | 0,5% | $5 |
| Split 3 | 2% | $20 |
| Split 4 | 2% | $20 |
| Platform fee | 4% | $40 |

> O teu capital ($910) fica guardado no contrato até saques/claims.

## Tiers e Visual

| Tier | Cor | Naves |
|------|-----|-------|
| TEST | Cinza | DRONE |
| EXPLORER | Verde | VYRA, KOMET, NEX |
| VANGUARD | Azul | AXION, PULSAR, ASTRON |
| ELITE | Roxo | KRYON, VORTIS |
| LEGENDARY | Dourado | EXODUS, KRAKEN |
