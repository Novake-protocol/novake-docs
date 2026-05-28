# Bônus Constelação

O Bônus Constelação são os **pontos binários** que acumulas a partir das Expedições da tua rede.

**Regra universal:** 1 ponto = $1

## Camada 1 — Expedição Tripulante

Quando qualquer recruta na tua linhagem lança uma Expedição Tripulante, **toda a linha acima** recebe pontos.

- **Distribuição:** infinita em profundidade
- **Requisito:** nenhum — qualquer pessoa acima recebe
- **Valor dos pontos:** igual ao lucro presumido da Expedição

**Cálculo dos pontos:**
```
Pontos = % sorteado × valor da Nave × (duração em meses)
```

**Exemplo:**
- Recruta D lança ASTRON $700, 90d, sorteou 11%
- Lucro presumido: 11% × 3 meses × $700 = $231
- Todos acima de D recebem **231 pontos** cada

## Camada 2 — Expedição Comandante

Quando um recruta lança uma Expedição Comandante, os pontos sobem pela linhagem mas com **gate**:

- **Distribuição:** infinita em profundidade
- **Gate:** só recebe quem tem Nave + Expedição Comandante **ativa**. Quem não tem = PULADO
- **Valor dos pontos:** % da tua Patente × valor da Nave do recruta

| Tua Patente | % dos pontos que capturas |
|---|---|
| Cadete | 20% |
| Sargento | 30% |
| Comandante | 40% |
| Supremo | 50% |

**Pontos perdidos:** a diferença entre o que capturaste e o máximo (50%) é **irrecuperável**.

**Exemplo:**
- Recruta E (na tua perna) lança KRAKEN $5.000 Comandante
- Tu és Sargento → capturas 30% × $5.000 = **1.500 pontos**
- O máximo seria Supremo (50%) = 2.500 pts
- Perdeste 1.000 pontos irrecuperáveis (eram teus se fosses Supremo)

## Conversão em USDC

```
Bônus USDC = Total de Pontos × Taxa do teu Pin
```

| Pin | Taxa |
|-----|------|
| Esmeralda | 15% |
| Safira | 16% |
| Rubi | 17% |
| Diamante | 18% |
| Black Diamond | 20% |

**Exemplo:**
- Acumulaste 5.000 pontos
- Tens Pin Black Diamond (20%)
- Recebes: 5.000 × 20% = **$1.000 USDC**
- Os restantes 80% ($4.000) vão para o treasury do protocolo

## Ver o Extrato

Na sidebar → **Spoils** → **Bônus Constelação** (`/bonus/contelacao`)

O extrato mostra:
- **Secção Comandante:** Piloto | Nave | Valor | Pts capturados ✅ | Pts perdidos 💸
- **Secção Tripulante:** Piloto | Nave | Plano | Lucro base | Pts recebidos ✅
