# Laboratorio 1: Configuración de Router Inalámbrico y Clientes (Caso Natsumi)

## Objetivos
Establecer conexiones físicas y coaxiales para servicios de Internet y TV.
Configurar un Router Inalámbrico doméstico mediante interfaz GUI.
Implementar medidas de seguridad básicas (Cambio de credenciales y WPA2).
Verificar conectividad DHCP y acceso a Internet en clientes cableados e inalámbricos.

## Configuración Realizada

1. Conectividad Física: Se establecieron las conexiones utilizando el estándar del medio adecuado.
Coaxial: Conexión desde el Splitter hacia el Cable Modem y la TV.
Ethernet (Copper Straight-Through): * Módem (Puerto 1) ➔ Router (Puerto Internet). 
PC Oficina y PC Dormitorio ➔ Puertos LAN del Router.

2. Seguridad y Hardening del Router: Para proteger la red de Natsumi, se aplicaron los siguientes cambios de la GUI.
Acceso Administrativo: Se cambió la contraseña por defecto admin por MyPassword1! .
Limitación de DHCP: Se restringió el número máximo de usuarios a 10 para reducir la superficie de exposición.
Seguridad Inalámbrica (WLAN):
SSID: MyHome
Seguridad: WPA2 Personal (AES).
Passphrase: MyPassPhrase1!

3. Verificación de Resultados
DHCP: Todos los dispositivos (PCs y Laptop) recibieron direccionamientos dinámicos en el segmento 192.168.0.x.
Conectividad: Se validó el acceso exitoso al servidor externo skillsforall.srv desde todos los terminales.

Evidencia

<img width="1437" height="774" alt="Screenshot 2026-02-20 at 5 33 56 PM" src="https://github.com/user-attachments/assets/53e9fb26-c0ff-48b0-827c-ca3a187fc4be" />
<br
<img width="705" height="709" alt="Screenshot 2026-02-20 at 5 35 02 PM" src="https://github.com/user-attachments/assets/bf26eba5-bd76-4237-a25f-336cb87b927c" />
<br
<img width="706" height="710" alt="Screenshot 2026-02-20 at 5 29 41 PM" src="https://github.com/user-attachments/assets/822ee27d-3bd0-4639-88ac-d1e8474f90a7" />
<br
<img width="701" height="707" alt="Screenshot 2026-02-20 at 5 35 40 PM" src="https://github.com/user-attachments/assets/6d350546-87c4-4ab0-b9db-5cbaf5345430" />
<br
<img width="704" height="709" alt="Screenshot 2026-02-20 at 5 30 52 PM" src="https://github.com/user-attachments/assets/ef7c559a-d6e9-4eb8-b65e-11c1de16f0fd" />
<br
*En este laboratorio aprendí la importancia de cambiar las credenciales por defecto (admin/admin), ya que son la primera puerta de entrada para atacantes. Asimismo, el uso de WPA2 Personal garantiza que el tráfico inalámbrico esté cifrado, evitando ataques de "sniffing" en la red local de Natsumi.*

