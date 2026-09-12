# 🚗 Proyecto: Urban Routes — Pruebas de Interfaz Web (UI/UX) y Funcionales

## 📌 Descripción del Producto
Urban Routes es una aplicación web interactiva diseñada para la reserva y personalización de rutas de transporte rápido. El sistema permite a los usuarios seleccionar puntos de origen y destino, calcular tarifas, personalizar servicios adicionales (como asientos para niños o selección de choferes) y gestionar métodos de pago.

---

## 🛠️ Herramientas y Entorno de Pruebas
* **Gestión de Pruebas y Defectos:** Jira.
* **Inspección Web y Consola:** Chrome DevTools (Inspección de elementos, red y consola de JavaScript).
* **Diseño de Pruebas:** Hojas de comprobación (Checklists) y Matrices de Casos de Prueba (Google Sheets).
* **Navegadores Probados:** Google Chrome (versión 146.0.7680.80), Mozilla Firefox.

---

## 🚀 Alcance y Metodología de Pruebas

### 1. Pruebas Exploratorias por Sesiones
Se realizaron sesiones de pruebas exploratorias estructuradas para auditar la aplicación bajo cuatro dimensiones clave:
* **Funcionalidad:** Verificación de flujos principales (ingreso de direcciones, selección de tarifas y confirmación de viaje).
* **Fiabilidad (Reliability):** Comportamiento del sistema ante entradas inválidas, refresco de pantalla e interrupción de sesiones.
* **Conveniencia (UX/UI):** Facilidad de uso, claridad de la interfaz y adaptabilidad en diferentes resoluciones de pantalla.
* **Rendimiento Visual (Performance):** Tiempos de carga de elementos gráficos e interacción con mapas interactivos.

---

## 📂 Archivos y Evidencias del Proyecto

* 📜 [Ver Checklist y Casos de Prueba de UI/UX](./Checklist-Urban-Routes.pdf) 
* 🐛 [Ver Reporte Consolidado de Defectos en Jira](./Bug-Reports-Urban-Routes.pdf)

---

## 🔍 Ejemplos de Defectos Identificados

#### Defecto 1: Inconsistencia visual en los pines de punto de partida y destino
* **Severidad:** Media / UI
* **Resultado Esperado:** El mapa debe mostrar el punto de partida con un circulo y el punto de destino con un circulo y un pin en color rojo.
* **Resultado Obtenido:** El mapa muestra los dos puntos con pines en color rojo y una letra al interior en color blanca.
* **Evidencia Visual:** 🔍 [Ver captura del error en Jira](./bug_ui_asiento_infantil.png)

---

#### Defecto 2: Fallo en la validación del formulario de número telefónico
* **Severidad:** Alta / Funcional
* **Resultado Esperado:** El campo de número telefónico debe solicitar un código de confirmación vía SMS antes de habilitar el botón "Siguiente".
* **Resultado Obtenido:** La aplicación permite avanzar en el flujo sin ingresar un número válido al presionar repetidamente la tecla `Enter`.
* **Evidencia Visual:** 🔍 [Ver captura del fallo de validación](./bug_validacion_telefono.png)

---

## 📊 Conclusiones del Testing
* Se ejecutaron más de 30 casos de prueba abarcando escenarios positivos, negativos y de límites.
* Se reportaron e ingresaron en Jira los defectos detectados con pasos claros para su reproducción, severidad asignada y capturas de pantalla/logs de la consola de DevTools.
* Las pruebas permitieron corregir inconsistencias en la interfaz web antes de la fase de despliegue final, mejorando la usabilidad general del producto.
