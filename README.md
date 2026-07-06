#  Seguidor Solar de Doble Eje Automático (Control Analógico sin Microcontrolador)

Este repositorio contiene el diseño, simulación y documentación técnica de un seguidor solar de dos ejes (acimut y elevación) automatizado. El objetivo del sistema es mantener un panel fotovoltaico perpendicular a la radiación solar para optimizar la captación de energía, logrando incrementar la eficiencia teórica hasta en un **21.2%** en comparación con sistemas fijos.

El núcleo del proyecto destaca por implementar una solución de control **100% analógica**, eliminando la dependencia de microcontroladores para reducir costos y complejidad operativa.

---

##  Desarrollo Colaborativo (PUCP)
Este proyecto fue diseñado e implementado en conjunto por estudiantes de **Ingeniería Electrónica de la Pontificia Universidad Católica del Perú (PUCP)**:
* Miguel Gálvez
* Gonzalo Mercado

---

##  Características Técnicas del Diseño

* **Acondicionamiento y Bloque Sensor:** Matriz de fotorresistencias (LDRs) desacopladas mediante técnicas de sombreado óptico (barreras físicas) para maximizar la sensibilidad diferencial ante variaciones de irradiancia.
* **Lógica de Control de Ventana (Analógica):** Implementación de circuitos comparadores con ventana de histéresis. Esto permite definir una "zona muerta" ajustable, evitando el desgaste mecánico de los motores por oscilaciones mínimas de luz o ruido eléctrico.
* **Etapa de Potencia:** Configuración de Puentes H discretos para la inversión de giro y control dinámico de los dos motorreductores CC encargados de los movimientos vertical y horizontal.
* **Validación:** Modelado y simulación completa del comportamiento del sistema en **Proteus**, asegurando la estabilidad del lazo de control antes de la implementación física.

---

## 📁 Estructura del Repositorio
* `Simulacion/` -> Archivos de simulación fuente en Proteus (`.pdsprj`).
* `Planos/` -> Diagramas esquemáticos del circuito analógico y etapas de potencia.
* `Documentos/` -> Informe técnico completo con formato académico IEEE.
