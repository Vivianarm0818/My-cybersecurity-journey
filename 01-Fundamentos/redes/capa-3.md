# 📂 Módulo 7: Capa de Acceso a la Red (Ethernet)

En este módulo he profundizado en cómo funciona **Ethernet**, el estándar más utilizado en las redes LAN. Como analista de seguridad, entender esta capa es crítico para detectar ataques de red local.

## 🧠 Conceptos Clave Aprendidos

### 1. La Subcapa MAC y LLC
Ethernet divide la Capa 2 en dos:
- **LLC (Logical Link Control):** Se comunica con las capas superiores (Capa 3).
- **MAC (Media Access Control):** Se encarga del hardware y de colocar los datos en el cable.

### 2. El Switch: El cerebro de la LAN
Aprendí cómo un Switch construye su **Tabla de Direcciones MAC**:
- Cuando llega una trama, el switch anota la MAC de origen y el puerto por donde entró.
- Si no conoce la MAC de destino, hace un **"Flood"** (envía la trama por todos los puertos excepto por donde vino).

### 3. Métodos de Conmutación
- **Store-and-Forward:** El switch recibe toda la trama y verifica que no tenga errores antes de enviarla (Más seguro).
- **Cut-Through:** Envía la trama en cuanto lee la dirección de destino (Más rápido, pero puede enviar errores).

---

## 🛡️ Enfoque de Seguridad: ¿Qué puede fallar aquí?

Desde la perspectiva del **Blue Team**, he identificado dos riesgos importantes en esta capa:

1. **MAC Address Table Overflow:** Un atacante puede inundar el switch con miles de direcciones MAC falsas. Esto obliga al switch a actuar como un "Hub", enviando todo el tráfico a todos los puertos, permitiendo que el atacante intercepte datos de otros.
2. **ARP Spoofing:** Como los switches confían en las respuestas ARP, un atacante puede decir "Yo soy el router" y desviar el tráfico hacia su máquina.

---

## 🛠️ Práctica de Laboratorio (Packet Tracer)
En este módulo, configuré un switch 2960 y verifiqué su funcionamiento con los siguientes comandos:

- `show mac address-table`: Para ver qué dispositivos están conectados y en qué puertos.
- `ipconfig /all`: En las PCs para verificar sus direcciones físicas (MAC).

> **Reflexión:** El switch es el guardián de la red local. Si no configuramos "Port Security", cualquier persona puede conectar un dispositivo malicioso y comprometer toda la red.# 📂 Módulo 7: Capa de Acceso a la Red (Ethernet)

En este módulo he profundizado en cómo funciona **Ethernet**, el estándar más utilizado en las redes LAN. Como analista de seguridad, entender esta capa es crítico para detectar ataques de red local.

## 🧠 Conceptos Clave Aprendidos

### 1. La Subcapa MAC y LLC
Ethernet divide la Capa 2 en dos:
- **LLC (Logical Link Control):** Se comunica con las capas superiores (Capa 3).
- **MAC (Media Access Control):** Se encarga del hardware y de colocar los datos en el cable.

### 2. El Switch: El cerebro de la LAN
Aprendí cómo un Switch construye su **Tabla de Direcciones MAC**:
- Cuando llega una trama, el switch anota la MAC de origen y el puerto por donde entró.
- Si no conoce la MAC de destino, hace un **"Flood"** (envía la trama por todos los puertos excepto por donde vino).

### 3. Métodos de Conmutación
- **Store-and-Forward:** El switch recibe toda la trama y verifica que no tenga errores antes de enviarla (Más seguro).
- **Cut-Through:** Envía la trama en cuanto lee la dirección de destino (Más rápido, pero puede enviar errores).

---

## 🛡️ Enfoque de Seguridad: ¿Qué puede fallar aquí?

Desde la perspectiva del **Blue Team**, he identificado dos riesgos importantes en esta capa:

1. **MAC Address Table Overflow:** Un atacante puede inundar el switch con miles de direcciones MAC falsas. Esto obliga al switch a actuar como un "Hub", enviando todo el tráfico a todos los puertos, permitiendo que el atacante intercepte datos de otros.
2. **ARP Spoofing:** Como los switches confían en las respuestas ARP, un atacante puede decir "Yo soy el router" y desviar el tráfico hacia su máquina.

---

## 🛠️ Práctica de Laboratorio (Packet Tracer)
En este módulo, configuré un switch 2960 y verifiqué su funcionamiento con los siguientes comandos:

- `show mac address-table`: Para ver qué dispositivos están conectados y en qué puertos.
- `ipconfig /all`: En las PCs para verificar sus direcciones físicas (MAC).

> **Reflexión:** El switch es el guardián de la red local. Si no configuramos "Port Security", cualquier persona puede conectar un dispositivo malicioso y comprometer toda la red.
