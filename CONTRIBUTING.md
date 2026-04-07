# Contributing to aux (Professional Trading Hub) 🏹💼

¡Gracias por contribuir a la maquinaria financiera del **Séquito del Terror**! Para mantener el estándar **Diamond Tier** de **DarckRovert**, todas las contribuciones deben centrarse en la estabilidad de red y el rendimiento asíncrono.

---

## 🛡️ Estándares Técnicos (Finance Core)

Este AddOn está optimizado para **Turtle WoW** (WoW v1.12.1). Las contribuciones DEBEN cumplir con:

1.  **Sniping Latency**: Las nuevas lógicas de rastreo no deben añadir más de 5ms de overhead al ciclo principal de red.
2.  **No Lua 5.1+**: El motor es Lua 5.0. Prohibido el operador `#` (usa `table.getn`).
3.  **Group Sync Stability**: La estructura de grupos debe ser compatible con los formatos existentes de TSM. No rompas la retro-compatibilidad de `AuxTradingAccounting`.
4.  **UI Apex Standard**: La interfaz de **aux** es compleja; cualquier cambio visual debe seguir los perfiles de diseño de pfUI.

## 📐 Arquetipo de Desarrollo

Si deseas contribuir:
- **`core/scan.lua`**: Es el corazón del sniper y el buscador. Requiere auditoría de rendimiento estricta.
- **`tabs/trading/`**: Contiene los módulos avanzados de análisis de mercado y sniping agregados por el Séquito.
- **`util/persistence.lua`**: Gestión de las bases de datos masivas de precios internacionales.

## 💎 Proceso de Pull Request

1.  **Fork & Branch**: Trabaja en ramas descriptivas (`fix/sniper-lag`, `feature/accounting-export`).
2.  **Documentación**: Actualiza `CHANGELOG.md` antes de enviar el PR.
3.  **Branding**: Mantén los enlaces institucionales oficiales de **DarckRovert**.

---
© 2026 **DarckRovert** — El Séquito del Terror.
*Ingeniería financiera para la conquista de Azeroth.*