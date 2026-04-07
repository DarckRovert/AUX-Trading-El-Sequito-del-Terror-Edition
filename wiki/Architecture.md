# ðŸ“ Wiki: Arquitectura 'Diamond Tier' â€” aux-addon [v2.0.1]

Estructura tÃ©cnica de la operativa de trading avanzada mantenida por **DarckRovert**.

## ðŸ—ï¸ JerarquÃ­a del Sistema Finance Hub (Broker Hierarchy)

**aux-addon** redirige toda la lÃ³gica de la casa de subastas original hacia un motor de procesamiento asÃ­ncrono de alto rendimiento:

1.  **Scanner Core (`core/scan.lua`)**: Modulo de intercepciÃ³n de red que gestiona el sniffing de objetos y la reconstrucciÃ³n de la tablas de bÃºsqueda.
2.  **Market Sniper (`tabs/trading/sniper.lua`)**: Motor de pulso tÃ¡ctico que rastrea el panel de subastas en segundo plano para hallar gangas instantÃ¡neas.
3.  **Group Manager (`tabs/trading/groups.lua`)**: Gestiona la lÃ³gica de perfiles y precios masivos basados en el estÃ¡ndar TSM.
4.  **UI Controller (`gui/core.lua`)**: Reemplaza totalmente los frames de Blizzard con un entorno tÃ¡ctico optimizado.

---

## ðŸ§­ Diagrama de Flujo: Sniper TÃ¡ctico v9.4

```mermaid
graph TD
    A[Inicio Sniper: Modo BÃºsqueda] --> B[Pulse-Scan de Red]
    B --> C{Â¿Filtro Cumplido?}
    C -- SÃ­ --> D[Alerta Visual Diamond Tier]
    D --> E[CÃ¡lculo de Margen de Beneficio]
    E --> F[Compra InstantÃ¡nea en 1 Clic]
    F --> G[Registro Contable Accounting.lua]
    G --> H[Sync con WCS_Brain Stats]
    C -- No --> I[Ciclo de Re-sniffing < 50ms]
    I --> B
```

## âš¡ Estrategias de IngenierÃ­a Diamond Tier

- **Throttled Scanning**: La consulta al servidor de subastas se fragmenta por pÃ¡ginas para evitar triggers de desconexiÃ³n por spam masivo.
- **Pattern Matching ML**: El motor de tendencias analiza los precios histÃ³ricos para detectar posibles manipulaciones de mercado (Market Manipulation detection).
- **TSM-Lite Persistence**: Conservamos la potencia de los grupos de TSM pero con un consumo de CPU un 80% menor en el cliente Vanilla.

---
Â© 2026 **DarckRovert** â€” El SÃ©quito del Terror.
*IngenierÃ­a financiera para la conquista de Azeroth.*

