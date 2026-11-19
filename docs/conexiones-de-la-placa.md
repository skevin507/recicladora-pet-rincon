# Conexiones de la placa

Esta fue mi otra gran dificultad: **ni el video ni las guías explicaban con claridad qué había que desconectar y qué conectar en la placa principal** de la Ender-3. Aquí reúno lo que se puede saber del video y lo que aprendí. El diagrama exacto está pendiente.

> ⚠️ **Antes de tocar cualquier cable:** desenchufa la máquina. El lado de corriente alterna (AC) de la fuente es peligroso. Si no estás seguro, pide ayuda a alguien con experiencia en electricidad.

## Qué se usa

La recicladora solo necesita **un calentador y un motor**, así que de toda la electrónica de la Ender-3 se usa poco:

| Elemento | ¿Se conecta? | Nota |
|---|---|---|
| Fuente de 24 V, lado AC | ✅ | Va al enchufe de corriente que se monta en la caja |
| Fuente de 24 V → placa | ✅ | Alimenta la placa principal |
| Calentador del hotend | ✅ | En su conector original de la placa |
| Termistor del hotend | ✅ | Para que la placa controle los 210 °C |
| Dos ventiladores | ✅ | El del hotend y el de enfriamiento |
| Un motor paso a paso | ✅ | Es el que mueve el bobinador |
| Pantalla LCD | ✅ | Para manejar la máquina |
| Cama caliente y su termistor | ❌ | Por eso la pantalla marca una temperatura negativa en la cama |
| Los demás motores (X, Y, Z) y los finales de carrera | ❌ | No se usan |

## Lo que todavía hay que documentar

- **En qué conector de la placa va el motor del bobinador.** Depende del archivo de impresión que mueve el motor. Hay que verificarlo con el archivo del diseño y en la placa real.
- **Una foto o un diagrama de la placa** con cada conector marcado.
- **Qué hacer con los cables que sobran**: retirarlos o aislarlos y amarrarlos.

Si sabes cómo completarlo, tu aporte es muy valioso: abre un Issue o un Pull Request (ver [CONTRIBUTING.md](../CONTRIBUTING.md)).
