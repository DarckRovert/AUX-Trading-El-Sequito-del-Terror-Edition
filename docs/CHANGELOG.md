# 📝 Changelog - AUX Trading System

**Por Elnazzareno (DarckRovert)**  
**El Séquito del Terror** 🔮

## [5.1.0] - 2026-03-23

### 🦾 Auditoría Completa Lua 5.0 (WoW 1.12)
- **100% Compatibilidad Estricta**: Reemplazo total de `ipairs` por bucles manuales `for i=1, getn(t)` en todo el proyecto.
- **Optimización de Métodos de String**: Sustitución de `string.gmatch` por `string.gfind` y uso extensivo de `string.find`/`string.sub` para compatibilidad máxima.
- **Seguridad Aritmética**: Reemplazo del operador `%` por `math.mod` en toda la lógica de paginación y formateo.

### 🔧 Infraestructura del Núcleo
- **Core Proxy Fix (package.lua)**: Corrección del sistema de módulos para permitir lectura/escritura en el entorno `M`. Previene errores de exportación `nil` en módulos complejos.
- **UX/UI Stability**: Corregido error crítico de "parent nil" en la pestaña de Oportunidades y Sniper.
- **Internal Registry**: Deduplicación y limpieza de `localization.lua` para acceso ultra-rápido a traducciones.

### 🎩 Mejoras en Trading
- **Gestión de Memoria Mejorada**: Optimización de `accounting.lua` y `log.lua` para escaneos de miles de items.
- **Validación de Datos**: Añadida protección contra datos corruptos en el historial de precios.

---

## [4.0.0] - 2026-01-17

### ✨ Nueva UI Profesional
- Rediseño completo de la interfaz de usuario
- Nuevo sidebar con navegación por iconos
- Esquema de colores oscuro profesional
- Indicadores visuales de selección de tabs

### 📊 Dashboard
- Tarjetas de estadísticas con colores distintivos
- Sección de actividad reciente
- Display de oro del jugador en header

### 📦 Sistema de Grupos
- Grupos predefinidos (Hierbas, Minerales, Encantamiento, etc.)
- Operaciones asignables a grupos
- Import/Export de grupos

### 🔍 Oportunidades
- Panel renovado con lista de items
- Botones de acción (Full Scan, Scan Rápido, Detener, Comprar)
- Columnas: Item, Precio, Mercado, Ganancia, %

### 🎯 Sniper
- Panel dedicado para monitoreo en tiempo real
- Configuración de % máximo
- Botón de inicio/parada

### 🔧 Mejoras Técnicas
- Compatibilidad con Lua 5.0 (WoW 1.12)
- Uso de `this` en lugar de closures
- Optimización de memoria
- Limpieza de archivos de backup

---

## [3.0.0] - 2026-01-15

### Añadido
- Sistema de Full Scan completo
- Cálculo estadístico de precios de mercado
- Módulo de Sniper básico
- Módulo de Vendor Search
- Sistema de notificaciones
- Tooltips avanzados

### Mejorado
- Rendimiento del escaneo
- Precisión de cálculos de mercado

---

## [2.0.0] - 2026-01-10

### Añadido
- Tab de Trading en la interfaz de AUX
- Búsqueda de oportunidades básica
- Sistema de tabs múltiples
- Integración con datos de mercado

### Mejorado
- Estructura del código
- Organización de módulos

---

## [1.0.0] - 2026-01-05

### Inicial
- Fork de aux-addon original
- Estructura base del sistema de trading
- Primeros módulos de análisis

---

## Leyenda

- ✨ **Añadido**: Nuevas funcionalidades
- 🔧 **Mejorado**: Mejoras en funcionalidades existentes
- 🐛 **Corregido**: Corrección de bugs
- 🗑️ **Eliminado**: Funcionalidades removidas
- ⚠️ **Deprecado**: Funcionalidades que serán removidas

---

*Desarrollado con ❤️ por Elnazzareno*  
*El Séquito del Terror* 🔮
