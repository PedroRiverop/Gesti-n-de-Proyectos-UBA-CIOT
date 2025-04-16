# Análisis estratégico de alcance, costos y complejidad

## Contexto del proyecto

El presente proyecto propone el desarrollo de un sistema de monitoreo acústico mediante tecnologías IoT, orientado a su aplicación tanto en entornos cerrados (como oficinas, hospitales, aulas) mediante conectividad Wi-Fi, como en pequeñas zonas urbanas (por ejemplo, plazas o parques) utilizando conectividad LoRa.

Este documento presenta un análisis detallado sobre el uso, utilidad, complejidad y costos del sistema bajo distintos escenarios, evaluando su escalabilidad hacia una futura integración con herramientas de inteligencia artificial.

---

## Etapa 1: Desarrollo del prototipo IoT

En la etapa inicial se plantea una implementación acotada, que permita:

- Validar el funcionamiento del sistema en campo
- Evaluar sensores, microcontroladores y comunicación inalámbrica
- Implementar monitoreo en tres puntos dentro de una pequeña zona urbana (ej. parque)

### Beneficios de esta configuración:

- Cobertura espacial realista sin necesidad de complejidad excesiva
- Identificación de focos localizados de contaminación acústica
- Visualización mediante dashboards o mapas térmicos
- Base sólida para escalar posteriormente

Se concluye que tres nodos en un mismo entorno representan un escenario **útil, demostrativo y viable** para el propósito de la especialización.

---

## Etapa 2: Expansión con inteligencia artificial

En una segunda fase, pensada para la especialización en Inteligencia Artificial, se proyecta escalar el sistema hacia una red distribuida de nodos en distintos puntos de una ciudad.

### Capacidades potenciales mediante IA:

- **Predicción de picos de ruido** a partir de patrones históricos
- **Identificación automática de fuentes acústicas** mediante aprendizaje automático
- **Detección de anomalías** o eventos acústicos inusuales
- **Recomendaciones inteligentes** para mitigación sonora en zonas sensibles

Esta expansión requiere una arquitectura modular y escalable, que permita el funcionamiento independiente de cada nodo y conserve la integración mediante MQTT, independientemente de si la red es Wi-Fi o LoRa.

---

## Comparación de escenarios

| Configuración               | N° de nodos | Cobertura      | Complejidad | Costo estimado (USD) |
|----------------------------|-------------|----------------|-------------|-----------------------|
| Parque con 3 nodos         | 3           | Zona puntual   | Baja        | 200–250               |
| Ciudad con 1 nodo por zona | 10 o más    | Amplia         | Alta        | 600–800+              |

> **Nota:** La expansión urbana implica mayores desafíos logísticos, energéticos y de infraestructura, pero ofrece un valor significativo para proyectos de IA y políticas públicas.

---

## Conclusión

Se considera adecuada la implementación inicial de tres nodos como estrategia didáctica y técnica, que permite validar el sistema, demostrar utilidad real y sentar las bases para su evolución futura con técnicas de inteligencia artificial.
