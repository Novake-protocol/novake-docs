# Constelação — Árvore Binária

A Constelação é a tua rede de recrutas organizada numa árvore binária de pagamento.

## Como Funciona a Árvore Binária

Cada posição na árvore tem **2 slots**: Esquerdo (LEFT) e Direito (RIGHT).

```
              [TU]
            /      \
        [A]          [B]
       /   \        /   \
     [C]   [D]   [E]   [F]
```

- **A** está no teu lado Esquerdo
- **B** está no teu lado Direito
- **C, D** estão na perna esquerda (abaixo de A)
- **E, F** estão na perna direita (abaixo de B)

### Spillover

Quando os teus 2 slots estão ocupados, novos recrutas vão para o primeiro slot livre **abaixo de ti** — isso chama-se spillover. O sistema alterna LEFT/RIGHT automaticamente para balancear.

> O teu **sponsor** (quem te convidou) pode ser diferente do teu **placement parent** (onde estás na árvore). Isso é normal.

## Dois Tipos de Pontos

### Pontos Tripulante
Gerados quando alguém na tua linhagem lança uma **Expedição Tripulante**.

- **Quando são gerados:** no momento do lançamento da Expedição
- **Quem recebe:** TODOS os níveis acima na árvore — sem limite de profundidade
- **Quantidade:** igual ao lucro presumido da Expedição
- **Requisito para receber:** nenhum (qualquer pessoa acima recebe)

**Exemplo:** O teu recruta C lança uma Expedição KRYON $1.000 por 120d com 14% → gera **$560 em pontos Tripulante** para ti e para todos acima de ti.

### Pontos Comandante
Gerados quando alguém na tua linhagem lança uma **Expedição Comandante**.

- **Quando são gerados:** no momento do lançamento
- **Quem recebe:** só quem tem Nave + Expedição Comandante ativa (se não tens → és PULADO)
- **Quantidade:** depende da tua Patente

| A tua Patente | % dos pontos que capturas |
|---|---|
| Cadete | 20% do valor da Nave |
| Sargento | 30% do valor da Nave |
| Comandante | 40% do valor da Nave |
| Supremo | 50% do valor da Nave |

**Pontos perdidos:** se não tens o requisito, os pontos são IRRECUPERÁVEIS e passam para o próximo que tem.

## Conversão de Pontos em USDC

Os pontos acumulados são convertidos via o teu **Pin** (Plano de Carreira):

```
Bônus USDC = Pontos × Taxa do Pin
```

| Pin | Taxa de Conversão |
|-----|-----------------|
| Esmeralda | 15% |
| Safira | 16% |
| Rubi | 17% |
| Diamante | 18% |
| Black Diamond | 20% |

**Exemplo:** 1.000 pontos + Pin Black Diamond = 1.000 × 20% = **$200 USDC**

O restante (80%) vai para o treasury do protocolo.

## Visualizar a Constelação

Na página **Constelação** (`/constellation`) vês:
- A tua posição na árvore
- Os membros de cada perna
- Pontos acumulados por secção
- Extrato de bônus recebidos

Na página **Árvore** (`/tree`) — apenas owner/admin — vês a árvore completa com profundidade 10.
