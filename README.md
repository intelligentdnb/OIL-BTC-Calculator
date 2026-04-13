# ⚡ OILBTC Perpetual Calculator

Calculadora de posiciones para el contrato perpetuo **OIL-BTC** (WTI Crude Oil denominado en Satoshis).

## Features

- **Long/Short** con toggle visual
- **Leverage ×1 a ×10** con slider
- **P&L neto** en sats y USD (incluye fees + funding)
- **Precio BTC/USD en vivo** via Binance API pública (auto-refresh cada 60s)
- **Sats/USD** como input principal — sincronizado con BTC/USD
- **Precio WTI/barril** calculado automáticamente (10 bbl/contrato)
- **Funding rate** integrado al P&L con soporte multi-periodo
- **Ratio Riesgo/Recompensa** con semáforo visual
- **Precio de liquidación** estimado con distancia %
- **Tabla comparativa ×1-×10** con mismo margen
- **Paste directo** desde la plataforma (limpia comas automáticamente)
- **PWA instalable** — funciona como app nativa en desktop y mobile

## Uso

1. Abrí `index.html` en Chrome/Edge
2. El precio BTC se carga automáticamente
3. Pegá los datos desde Roxom (entrada, SL, TP, margen, funding rate)
4. Listo — todo se calcula en tiempo real

## Instalar como App (PWA)

**Chrome/Edge desktop:**
- Menú (⋮) → "Instalar OILBTC Calculator" → Instalar

**Android:**
- Chrome → Menú (⋮) → "Agregar a pantalla de inicio"

**iPhone:**
- Safari → Compartir → "Agregar a inicio"

## GitHub Pages

Si querés hostear online:
1. Settings → Pages → Source: main / root
2. Tu app queda en `https://tu-usuario.github.io/oilbtc-calculator/`

## Datos y privacidad

- **Cero datos sensibles** en el código
- No se guardan ni envían datos de trading
- Única conexión externa: Binance API pública (precio BTC/USDT)
- Los valores que ingresás viven solo en memoria del navegador
- Al cerrar se borran

## Contrato OIL-BTC

| Spec | Valor |
|---|---|
| Plataforma | Roxom |
| Subyacente | WTI Light Sweet Crude Oil |
| Tamaño | 10 × WTI price |
| Denominación | BTC (Satoshis) |
| Max Leverage | 10× |
| Funding | Cada 8h (00:00, 08:00, 16:00 UTC) |
| Fee Taker | 0.075% |
| Fee Maker | 0.025% |
