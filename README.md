# Simulador-de-sEMG-a-partir-de-registros-reales
Simulador de señales de electromiografía de superficie (sEMG) de 8 bits utilizando registros reales de PhysioNet y un DAC en ESP32
##  Características
- **Base de datos:** PhysioNet (GRABMyo, Participante 1, Canal F12).
- **Secuencia:** 15 segundos (Reposo -> Cierre de mano -> Extensión de índice).
- **Resolución:** Escalado lineal de 8 bits (0-255).
- **Hardware:** ESP32-WROOM (DAC en GPIO25).

##  Estructura del Repositorio
- `colab/`: Código en Python para procesamiento, escalado y visualización.
- `src/`: Firmware en C++ para Arduino IDE y archivo de cabecera `semg.h`.

##  Requisitos
- ESP32 Dev Module
- Arduino IDE con soporte para ESP32
- Python 3 / Google Colab (`wfdb`, `numpy`, `matplotlib`)
