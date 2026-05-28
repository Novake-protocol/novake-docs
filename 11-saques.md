# Saques e Spoils

## O que Podes Sacar

| Tipo | O que é | Quando |
|------|---------|--------|
| **Spoils** | Yield da Expedição Tripulante | Após a Expedição encerrar |
| **Capital** | USDC original investido na Nave | No aniversário do plano (data de unlock) |
| **Bônus de Embarque** | Comissão de indicação direta | Imediatamente após a compra do indicado |
| **Bônus Constelação** | Pontos convertidos via Pin | Via claim no dashboard |
| **Bônus Residual** | % do yield dos recrutas | Cap $300/dia, $3.000/mês |
| **Vesting $NVKE** | Tokens da presale | Conforme cronograma de vesting |

## Fee de Saque

Todos os saques e claims têm uma taxa de **4%** que vai para a `platformWallet`.

**Exemplo:** Vais sacar $1.000 de Spoils → recebes $960, $40 vão para o protocolo.

## Processo de Saque

1. Vai ao **Painel** → secção "Disponível para Saque"
2. Clica em **Sacar**
3. Se tens 2FA ativo → confirma o código
4. Confirma a transação na MetaMask
5. USDC chega à tua wallet em segundos (Base L2)

## Vesting $NVKE (Presale)

Se compraste $NVKE na presale, tens tokens em vesting:
- **12% TGE** — libertados no lançamento do token
- **1 mês de cliff** — sem libertação
- **7 meses de vesting** — libertação linear mensal

Na página `/vesting` vês o teu cronograma e podes fazer claim dos tokens disponíveis.

## Proteção On-Chain

O saque de capital das **Naves Presente** é **impossível** — o contrato reverte com `GiftedShipCannotWithdrawCapital`. Esta proteção existe na blockchain e não pode ser contornada.

## 2FA (Autenticação de Dois Fatores)

Para proteger os saques podes ativar 2FA em `/perfil` → Segurança. Após ativo, todos os saques requerem código TOTP.
