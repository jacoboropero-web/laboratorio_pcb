# ECAD PCB Design Laboratory - KiCad

**Curso:** Electrónica Asistida por Computador (ECAD)  
**Estudiantes:**
- Jacobo Ropero Ramírez — jacobo.ropero@autonoma.edu.co
- Santiago Rueda Muriel — santiago.ruedam@autonoma.edu.co
- Juan José Noriega — juanj.noriegal@autonoma.edu.co - Desertó

---

## Descripción del Proyecto

Este repositorio contiene los archivos de proyecto de KiCad desarrollados para las tres tareas del laboratorio de diseño de PCB:

### 1. Tarea 1: Linterna LED (`/Tarea_1_Linterna_LED`)
* Circuito básico alimentado por batería de botón CR2032 (3V).
* Incluye pulsador táctil (SW1), resistor limitador de 1kΩ (0805) y LED rojo de 5mm.
* Ancho de pista: 0.4 mm (16 mils).
* Borde de placa personalizado en `Edge.Cuts` (65 mm x 25 mm aproximadamente) con esquinas redondeadas.

### 2. Tarea 2: ESP32-S3 Mini (`/Tarea_2_ESP32_S3_Mini`)
* Placa de desarrollo basada en el módulo ESP32-S3 WROOM.
* Alimentación regulada a 3.3V mediante LDO AMS1117 con capacitores de desacoplo de 10 µF.
* Cumplimiento de regla RF: antena del módulo posicionada fuera del plano de masa en el borde de la placa.

### 3. Tarea 3: ESP32 con USB-C y CP2102 (`/Tarea_3_ESP32_USBC_CP2102`)
* Interfaz USB Tipo-C con resistencias de 5.1 kΩ independientes en pines CC1 y CC2, e integración de diodo de protección ESD (USBLC6-2SC6).
* Conversor USB a UART CP2102N y circuito de auto-reset/flashing mediante dos transistores NPN (S8050/BC817) conectados a DTR y RTS.
* Ruteo de par diferencial de datos USB D+/D- ajustado a 90 Ω de impedancia característica y plano de tierra continuo.

---

## Estructura de Archivos por Carpeta
Cada carpeta de proyecto contiene:
* `.kicad_pro`: Archivo de proyecto principal.
* `.kicad_sch`: Esquemático del circuito.
* `.kicad_pcb`: Layout de la placa de circuito impreso.
* `/Gerbers`: Archivos de fabricación Gerber y archivos de taladrado Excellon.

## Requisitos de Software
* **KiCad EDA v7.0 / v8.0 / v10.0**
