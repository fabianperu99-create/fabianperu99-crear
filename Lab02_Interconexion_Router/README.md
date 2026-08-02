# LAB 02: Enrutador de Interconexión

## Objetivo
Configurar un Router en Cisco Packet Tracer para interconectar
2 redes LAN distintas y verificar la comunicación entre 
dispositivos de redes diferentes.

## Materiales Utilizados
- 1 Router-PT
- 2 Switch-PT
- 4 PC-PT
- Cable Consola y Cable Directo

## Topología de Red
Se implementaron 2 redes LAN conectadas por un Router.
- **Red 1**: 192.168.1.0
- **Red 2**: 192.168.2.0

## Direccionamiento IP

| Dispositivo | Interfaz | Dirección IP | Máscara | Gateway |
| --- | --- | --- | --- | --- |
| Router0 | Fa0/0 | 192.168.1.1 | 255.255.255.0 | N/A |
| Router0 | Fa1/0 | 192.168.2.1 | 255.255.255.0 | N/A |
| PC0 | NIC | 192.168.1.10 | 255.255.255.0 | 192.168.1.1 |
| PC1 | NIC | 192.168.1.11 | 255.255.255.0 | 192.168.1.1 |
| PC2 | NIC | 192.168.2.10 | 255.255.255.0 | 192.168.2.1 |
| PC3 | NIC | 192.168.2.11 | 255.255.255.0 | 192.168.2.1 |

## Procedimiento
1. Conectar los dispositivos según la topología.
2. Configurar las interfaces del Router con sus respectivas IPs.
3. Asignar IP y Gateway a cada PC.
4. Realizar pruebas de conectividad con el comando `ping`.

![Evidencia Lab02](Lab02_Topologia.png)
