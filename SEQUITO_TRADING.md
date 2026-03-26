# aux-addon — Guía de Trading Avanzado (Séquito del Terror)

## Descripción

Esta es la versión **"AUX Trading System"** del addon de Casa de Subastas, expandida masivamente para el Séquito del Terror. Sobre la base original de aux-addon, se han añadido 30+ módulos de trading avanzado.

## Módulos Disponibles

### Core de Trading (`tabs/trading/`)

| Módulo | Archivo | Descripción |
|---|---|---|
| Dashboard | `dashboard.lua` + `dashboard_ui.lua` | Panel principal con métricas de mercado |
| ML Patterns | `ml_patterns.lua` | Detección de patrones con machine learning básico |
| Sniper | `sniper.lua` | Compra automática de items subvalorados |
| Market Data | `market_data.lua` | Base de datos de precios históricos |
| Full Scan | `full_scan.lua` | Escaneo completo de la Casa de Subastas |
| Accounting | `accounting.lua` | Registro de transacciones y P&L |
| Monopoly | `monopoly.lua` + `monopoly_ui.lua` | Estrategia de control de mercado |
| Auctioning | `auctioning.lua` + `auctioning_ui.lua` | Publicación masiva de subastas |
| Dealfinding | `dealfinding.lua` | Búsqueda de deals rentables |
| Optimization | `optimization.lua` | Optimización de listings |
| Notifications | `notifications.lua` | Alertas de precio y mercado |
| Log | `log.lua` | Historial de operaciones |
| Item Tracker | `item_tracker.lua` + `item_tracker_ui.lua` | Seguimiento de items específicos |
| Crafting | `crafting.lua` + `crafting_ui.lua` | Análisis de rentabilidad de crafteo |
| Vendor | `vendor.lua` + `vendor_ui.lua` | Tracking de items de vendor |
| Price History | `price_history.lua` | Histórico de precios por item |
| Market Analysis | `market_analysis.lua` | Análisis estadístico del mercado |
| Automation | `automation.lua` | Automatización de operaciones repetitivas |
| Strategies | `strategies.lua` | Estrategias de inversión configurables |
| Alerts UI | `alerts_ui.lua` | Interfaz de alertas avanzadas |
| Config UI | `config_ui.lua` | Panel de configuración central |
| Groups | `groups.lua` | Agrupación de items por categoría |
| Scan Integration | `scan_integration.lua` | Integración con el escáner de AH |
| Tooltips | `tooltips_advanced.lua` | Tooltips con precio de mercado |

### Módulos Desactivados (comentados en TOC)

Estos módulos están en el código pero temporalmente desactivados:
- `icon_system.lua`, `sort_system.lua`, `search_system.lua`
- `filter_system.lua`, `export_system.lua`, `backup_system.lua`

## Variables Guardadas

```lua
SavedVariables: aux, AuxTradingMarketData, AuxTradingAccounting, AuxPriceHistory
```

## Comandos

```
/aux         — Abre la Casa de Subastas
/aux scan    — Inicia escaneo completo
/aux report  — Muestra reporte de P&L
```

## Integración con el Ecosistema

- **WCS_Brain**: los datos de mercado de aux pueden alimentar el sistema de economía del clan
- **pfUI**: el header de aux usa el tema pfUI si está disponible
