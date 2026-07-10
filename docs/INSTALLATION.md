# Instalación - DaViCAN-UDS

## Requisitos
- Python 3.7+
- PlatformIO CLI o VSCode + extensión
- ESP32-S3 DevKit
- Transceptor CAN (SN65HVD230 recomendado)

## Instalación PlatformIO

```bash
pip install platformio
```

## Compilar y cargar

```bash
cd DaViCAN-UDS
pio run
pio run -t upload
pio device monitor -b 115200
```

## Conexionado

```
ESP32-S3  →  SN65HVD230  →  CAN Bus
GPIO6     →  D (TX)
GPIO7     →  R (RX)
GND       →  GND
3.3V      →  VCC
                  CANH      →  CANH
                  CANL      →  CANL
```
