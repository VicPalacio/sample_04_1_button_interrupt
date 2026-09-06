## Implementación componentes oficiales o de terceros

Para desarrollar este tema se trabajó el siguiente proyecto

### Directorio:

C:\Users\WINDOWS 10\Documents\ESP32_2026\sample_04_1_button_interrupt\main

### Recursos en [developer link](https://developer.espressif.com/blog/2026/02/component-introduction-button/#key-features)

Este ejemplo realiza la lectura de un botón y tiene como propósito mostrar el
paso para agregar componentes (librerías a un proyecto) esto aplica para
componentes desarrollados por terceros o por espressif, en este caso este
componente fue desarrollado por espressif, ya que como se observa en el nombre
del componente aparece primero espressif y luego el nombre (espressif/button)
El procedimiento es exactamente igual al ejemplo mostrado en el ejemplo:
“Procedimiento para incluir un Componente (librería) Ejemplo₁”, para descargar
este componente se usa el comando:

```{C}
idf.py add-dependency "espressif/button=\*"
```

En el enlace mostrado en el [Recurso](https://developer.espressif.com/blog/2026/02/component-introduction-button/#key-features)
se saltan el paso en el que se debe correr el comando:

```{C}
“Run idf.py reconfigure Task”
```

por lo demás es exactamente igual, en este mismo enlace está toda la
documentación de lo que hace el ejemplo, a continuación, solo mencionaré lo que
hace el ejemplo:

### El componente de botón ofrece varias funciones potentes:

- Múltiples tipos de botones:

* Compatibilidad con botones GPIO y matrices de botones ADC.

- Detección de eventos:

* Gestión integral de eventos, incluyendo pulsación, liberación, pulsación prolongada y pulsación repetida.

- Eliminación de rebotes:

* Eliminación de rebotes por software integrada para eliminar falsos disparos.

- Soporte de bajo consumo:

* Optimizado para aplicaciones alimentadas por batería.

- Sistema de devolución de llamada:

* Mecanismo de devolución de llamada fácil de usar para eventos de botones.

- Seguro para subprocesos:

* seguro para usar en aplicaciones multiproceso.

- Tipos de eventos enriquecidos :

* Admite 11 eventos de botón diferentes, entre ellos: + Botón pulsado, + Suelto + pulsar + Repetir

- Detección de clic
  - único
  - doble
  - múltiples
  - Iniciar
  - mantener pulsado
  - soltar eventos
  - Pulsa repetir hecho
  - pulsa finalizar notificaciones
