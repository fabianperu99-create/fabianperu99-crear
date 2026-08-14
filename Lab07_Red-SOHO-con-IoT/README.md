# Lab 7: Configuración de Red SOHO con Dispositivos IoT

## 1. Objetivo
Configurar una red SOHO con acceso a Internet, servicio DHCP 
y gestión de dispositivos IoT utilizando Cisco Packet Tracer,
simulando un entorno de hogar inteligente con control web.

## 2. Descripción de la Topología
La red está compuesta por un Home Gateway0 que se conecta a
Internet mediante un Cable Modem. El Gateway distribuye red 
LAN por cable y WiFi a los dispositivos: PC, Home-Tablet, 
Music Player y 2 Speakers. Los dispositivos IoT son controlados
desde la interfaz web del Gateway.

## 3. Desarrollo y Evidencias

### Evidencia 1: Configuración DHCP y Asignación de IP
Se configuró el servicio DHCP en el Home Gateway0. La Home-Tablet
obtuvo configuración IP automáticamente con Gateway `192.168.25.1`
y DNS `203.0.0.2`, confirmando que la red interna `192.168.25.0/24` 
funciona correctamente.
![Configuración DHCP](./evidencias/DHCP.png)
*Figura 1: Configuración WAN del Gateway e IP por DHCP en la Tablet*

### Evidencia 2: Prueba de Conectividad
Se realizó prueba de ping desde el PC hacia la dirección 
`192.168.25.100`. El resultado muestra 4 paquetes enviados,
4 recibidos y 0% de pérdida, lo que confirma la conectividad 
en la red LAN.
![Prueba de Ping](evidencias_PING.png)
*Figura 2: Ping exitoso desde PC a 192.168.25.100*

### Evidencia 3: Gestión de Dispositivos IoT
Se accedió a la interfaz web de administración del Home Gateway0
desde la Home-Tablet mediante la URL `http://192.168.25.1` utilizando
las credenciales `admin/admin`. Esta interfaz permite controlar
dispositivos IoT como el Music Player y los Speakers.
![Interfaz IoT](evidencias_IoT.png)
*Figura 3: Login a la interfaz web del Home Gateway0 para administración
IoT*

## 4. Conclusiones
1. Se implementó exitosamente una red SOHO con segmentación LAN y conexión
   WAN simulada.
2. El servicio DHCP del Home Gateway asignó direcciones IP correctamente
 a los dispositivos inalámbricos.
3. Se verificó la conectividad de la red mediante pruebas de ping con 0%
 de pérdida de paquetes.
4. Se demostró la administración de dispositivos IoT a través de una interfaz
  web, cumpliendo con el objetivo de hogar inteligente.
5. La topología cumple con los requerimientos de una red doméstica moderna
 con control centralizado.

# Conclusión 

En el desarrollo de esta práctica se logró configurar una red SOHO funcional
en Cisco Packet Tracer. 

Los puntos clave fueron:
- **Conectividad**: Se comprobó mediante ping que todos los dispositivos dentro
   de la red `192.168.25.0/24` se comunican correctamente.
- **DHCP**: El Home Gateway actuó como servidor DHCP, asignando IPs
  automáticamente y facilitando la conexión de la Tablet.
- **IoT**: Se implementó la gestión de dispositivos inteligentes mediante la
  interfaz web del Gateway, demostrando el concepto de hogar conectado.

Esta práctica permitió comprender la integración de redes tradicionales con 
dispositivos IoT, base fundamental para las redes domésticas actuales.
