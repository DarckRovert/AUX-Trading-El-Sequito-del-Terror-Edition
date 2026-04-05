# Arquitectura — aux-addon Sequito 🏗️

mermaid
graph TD
    CORE[aux Core]
    CACHE[Price Cache]
    SCAN[AH Scanner]
    UI[Custom Search UI]

    SCAN --> CACHE
    CACHE --> CORE
    CORE --> UI


## Componentes
- **core/**: Lógica central de comunicación con la API de subastas de WoW.
- **gui/**: Definición de frames y elementos visuales personalizados.
- **util/**: Librerías de ayuda para formateo de moneda y strings.
