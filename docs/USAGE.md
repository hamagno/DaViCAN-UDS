# Uso - DaViCAN-UDS

## Comandos Básicos

### Modo Normal (Monitoreo)
```
p         - Pausar/Reanudar
m0        - Ver todo
m1        - Solo UDS
m2        - Solo OBD
m3        - Solo stats

s0-s3     - Velocidades (125/250/500/1000 kbps)
sa        - Auto-detectar

f<ID>     - Filtrar ID
fn        - Quitar filtro

r         - Reset stats
```

## Modo UDS

```
u         - Entrar/Salir modo UDS
uh        - Ayuda UDS
```

### Comandos UDS
```
utester   - Tester Present
uvin      - Leer VIN
usec      - Security Access L1
usalevel <1-3> - Security Access
uraw <hex> - Comando raw
```

## Ejemplo: Sprinter 2026

```
1. p              # Activar
2. m1             # Solo UDS
3. u              # Modo UDS
4. uvin           # Verificar respuesta
5. usec           # Solicitar seed
6. usalevel 2     # Nivel 2
7. usalevel 3     # Nivel 3
```

**Respuestas:**
- Positiva (0x67): ✓ Implementado
- Negativa (0x7F): ✗ Rechazado
