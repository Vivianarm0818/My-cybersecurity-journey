# Lab 02: red local en Packet Tracer

Descripción
En este laboratorio configuré una red básica para entender cómo se comunican dos dispositivos en la misma subred.

Configuración
- PC-A: IP 192.168.1.1 / Máscara 255.255.255.0
- PC-B: IP 192.168.1.2 / Máscara 255.255.255.0
- PC-C: IP 192.168.1.2 / Máscara 255.255.255.0
- Conectividad: los tres conectados a un Switch 2960.

Resultados
Logré realizar un `ping` exitoso entre las tres máquinas. Con el comando `show mac address-table` pude observar qué dispositivos están conectados y en qué puertos desde la terminal del switch.

<img width="661" height="592" alt="Screenshot 2026-02-24 at 1 26 57 PM" src="https://github.com/user-attachments/assets/ebca330e-1d92-4063-a96a-5d581d1f4055" />

<img width="303" height="231" alt="Screenshot 2026-02-24 at 1 26 39 PM" src="https://github.com/user-attachments/assets/be0c9926-d294-4f3e-b464-ac4e145985c7" />

<img width="431" height="268" alt="Screenshot 2026-02-24 at 1 26 22 PM" src="https://github.com/user-attachments/assets/1f398482-ead3-488b-b77c-de766d4dbdd3" />
