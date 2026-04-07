# 🛠️ Wiki: Guía de API — Professional Trading Hub (aux)

aux-addon expone métodos avanzados para que otros AddOns del ecosistema **Séquito del Terror** puedan automatizar compras o alertas económicas.

## 📡 Funciones de Trading (Broker API)

### `aux_GetMarketValue(itemID)`
Obtiene el valor de mercado calculado por los algoritmos de aux para un objeto.
- **`itemID`**: ID numérica de Turtle WoW.
- **Retorno**: Valor en cobre (market-trend aware).

### `aux_RegisterSniperCallback(func)`
Permite que un script externo se suscriba a las alertas del Sniper.
- **`func`**: Función que recibirá los datos del objeto detectado.

## 📎 Integración con Ecosistema Gravity

- **Neural Re-gearing**: **WCS_Brain** utiliza la API de aux para monitorear en tiempo real si el equipo "Best-in-Slot" se ha puesto a la venta en la subasta por debajo de su precio de mercado usual.
- **Profit Alert**: **TerrorMeter** puede emitir una alerta sonora de clan si un objeto épico es detectado por el Sniper de un miembro del grupo.

---
© 2026 **DarckRovert** — El Séquito del Terror.
*Ingeniería financiera para la conquista de Azeroth.*
