# Network Operations

Bienvenidos a la guía de introducion de redes orientada a Ciberseguridad

Esta guía esta realizada gracias a los conceptos adquiridos mediante el programa de Google de Ciberseguridad:

https://www.coursera.org/professional-certificates/google-cybersecurity



## Network Protocols o Protocolos de redes

Son conjuntos de reglas que rigen la forma en que los dispositivos de una red se comunican entre sí. Aseguran que los datos se entreguen de forma correcta y eficiente.

- **Tipos de protocolos de red:**

  - **Protocolos de comunicación:** Gestionan el intercambio de información, la transmisión de datos y la recuperación de datos perdidos. Algunos ejemplos son:

    ***TCP:** Este protocolo garantiza una transmisión de datos fiable entre dispositivos.*

    ***UDP:** Este protocolo es un protocolo sin conexión que no establece una conexión entre dispositivos antes de una transmisión.*

    ***HTTP:** Este protocolo es un protocolo de capa de aplicación que proporciona un método de comunicación entre clientes y servidores de sitios web. Puerto 80*

    **DNS:**Este protocolo traduce los nombres de dominio de Internet en direcciones IP. Suele utilizar UDP en el puerto 53. Sin embargo, si la respuesta DNS a una solicitud es grande, cambiará a utilizar el protocolo TCP*

  - **Protocolos de gestión:** Supervisan y gestionan la actividad de la red, incluidos los informes de errores y la optimización del rendimiento. Algunos ejemplos son:

    ***SNMP:** Este protocolo se utiliza para supervisar y gestionar dispositivos en una red. SNMP puede restablecer una contraseña en un dispositivo de red o cambiar su configuración de línea base.*

     ***(ICMP):** Este protocolo se utiliza para que los dispositivos se informen mutuamente sobre los errores de transmisión de datos en la red. ICMP es utilizado por un dispositivo receptor para enviar un informe al dispositivo emisor sobre la transmisión de datos.(Usado en comando ping)*

  - **Protocolos de seguridad:** Garantizan la transmisión segura de datos mediante algoritmos de cifrado. Algunos ejemplos son

    ***Hypertext Transfer Protocol Secure:** Es un protocolo de red que proporciona un método seguro de comunicación entre clientes y servidores web. HTTPS es una versión segura de HTTP que utiliza el cifrado de capa de sockets seguros/seguridad de la capa de transporte (SSL/TLS) en todas las transmisiones para que no se pueda leer la información contenida. HTTPS utiliza el puerto 443.*

    ***Secure File Transfer Protocol:** Es un protocolo seguro que se utiliza para transferir archivos de un dispositivo a otro a través de una red. SFTP utiliza Secure Shell (SSH), normalmente a través del puerto TCP 22*

Otros protocolos a tener en cuenta:

- **Traducción de direcciones de red (NAT):** Permite que los dispositivos en una red privada se comuniquen con la internet pública utilizando una única dirección IP pública.
- **Protocolo de configuración dinámica de host (DHCP):** Asigna direcciones IP y otra información de configuración de red a los dispositivos en una red.
- **Protocolo de resolución de direcciones (ARP):** Traduce las direcciones IP a direcciones MAC, que se utilizan para comunicarse con dispositivos en la misma red.
- **Telnet:** Un protocolo de capa de aplicación utilizado para conectarse con un sistema remoto. Envía toda la información en texto claro y no es tan seguro como SSH.
- **Secure Shell (SSH):** Proporciona una conexión segura con un sistema remoto utilizando comunicación cifrada.
- **Protocolo de oficina postal (POP):** Se usa para administrar y recuperar correo electrónico de un servidor de correo.
- **Protocolo de acceso a mensajes de internet (IMAP):** Se utiliza para el correo electrónico entrante. Descarga los encabezados y el contenido de los correos electrónicos y los mantiene en el servidor de correo electrónico, lo que permite a los usuarios acceder a su correo electrónico desde múltiples dispositivos.
- **Protocolo simple de transferencia de correo (SMTP):** Se usa para transmitir y enrutar el correo electrónico desde el remitente a la dirección del destinatario.

## Wireless Protocols o Protocolos de seguridad inalámbrica

Las comunicaciones Wi-Fi están aseguradas por protocolos de redes inalámbricas.

Tipos de protocolos inalámbricos

- **WEP (Privacidad Equivalente a Cableado)**: El WEP es un protocolo de seguridad inalámbrica diseñado para proporcionar a los usuarios el mismo nivel de privacidad en conexiones de red inalámbricas que en conexiones de red cableadas. Desarrollado en 1999, es el más antiguo de los estándares de seguridad inalámbrica.

- **WPA (Acceso Protegido por Wi-Fi)**: El WPA se desarrolló en 2003 para mejorar y reemplazar el WEP, abordando los problemas de seguridad que presentaba. WPA siempre estuvo destinado a ser una medida transitoria para establecer compatibilidad con hardware más antiguo.

  WPA a evolucionado hasta su tercera versión WPA3 mejorando la seguridad ante ataques y su encriptación

## Elementos de Seguridad

**Firewall o Cortafuegos:** Es un dispositivo de seguridad de red que supervisa el tráfico hacia y desde su red y lo permite o bloquea en función de un conjunto definido de reglas de seguridad.

Tipos:

- **Cortafuegos de hardware:** Un dispositivo físico que inspecciona cada paquete de datos antes de que se le permita entrar en la red.

- **Cortafuegos de software:** Un programa de software instalado en un ordenador o servidor que realiza las mismas funciones que un cortafuegos de hardware.

- **Cortafuegos basado en la nube:** Un cortafuegos de software alojado por un proveedor de servicios en la nube que protege todo el tráfico entrante antes de que llegue a la red local de la organización.

Cortafuegos con estado vs. sin estado:

- **Cortafuegos con estado o Statefull:** Realiza un seguimiento de la información que pasa por él y filtra proactivamente las amenazas.
- **Cortafuegos sin estado o Stateless:** Funciona según reglas predefinidas y no realiza un seguimiento de la información de los paquetes de datos.

***Cortafuegos de próxima generación (NGFW):** Ofrecen aún más seguridad que los cortafuegos con estado al realizar una inspección profunda de los paquetes y protección contra intrusiones.*

------

**VPNS o Red Privada Virtual**: es una herramienta de seguridad que crea una conexión segura entre su dispositivo y un servidor VPN. Esta conexión cifra sus datos y oculta su dirección IP, lo que le permite navegar por Internet de forma más privada y segura

**Beneficios de usar una VPN:**

- **Privacidad:** Una VPN oculta su dirección IP real, lo que dificulta que los sitios web y los anunciantes rastreen su actividad en línea.
- **Seguridad:** Una VPN cifra sus datos, lo que los protege de ser interceptados por hackers o fisgones.
- **Acceso a contenido bloqueado:** Una VPN puede ayudarlo a acceder a contenido que está bloqueado en su país o región.
- **Evitar la censura:** Una VPN puede ayudarlo a evitar la censura gubernamental o corporativa.

**Cómo funciona una VPN:**

- *Usted se conecta a un servidor VPN.*
- *El servidor VPN asigna una nueva dirección IP.*
- *Su tráfico de Internet se enruta a través del servidor VPN.*
- *El servidor VPN cifra sus datos.*
- *Sus datos se envían a su destino.*

**Ejemplos de uso de una VPN:**

- *Usar una red Wi-Fi pública de forma segura.*
- *Acceder a contenido bloqueado en su país.*
- *Evitar la censura gubernamental.*
- *Proteger su privacidad en línea.*

------

**Security Zones**

**Que son las zonas de seguridad y que realizan**

- Segmentos de una red que protegen la red interna de Internet.
- Parte de la segmentación de la red, que divide la red en segmentos con diferentes permisos de acceso y reglas de seguridad.
- Controlan quién puede acceder a las diferentes partes de la red.
- Actúan como una barrera para las redes internas, mantienen la privacidad y evitan que los problemas se propaguen.



Tipos de zonas de seguridad:

- **Zona no controlada:** Cualquier red fuera del control de la organización (por ejemplo, Internet).
- **Zona controlada:** Subred que protege la red interna de la zona no controlada.
  - ***Zona desmilitarizada (DMZ):** Servicios públicos accesibles desde Internet (servidores web, servidores proxy, servidores DNS, servidores de correo electrónico, servidores de archivos).*
  - ***Red interna:** Servidores y datos privados que requieren protección.*
  - ***Zona restringida:** Información altamente confidencial accesible solo para personal autorizado.*

------

**Proxy Servers**

Un servidor dedicado que se encuentra entre Internet y el resto de la red, actuando como intermediario para todo el tráfico entrante y saliente

- Beneficios de los servidores proxy:
  - **Seguridad:** Oculta la dirección IP de la red privada de los actores maliciosos y filtra los sitios web no seguros.
  - **Rendimiento:** Almacena datos que son solicitados regularmente por servidores externos, reduciendo el contacto con el servidor interno.

- Tipos de servidores proxy:
  - **Servidor proxy de reenvío:** Regula y restringe el acceso de una persona a Internet, ocultando la dirección IP del usuario y aprobando todas las solicitudes salientes.
  - **Servidor proxy inverso:** Regula y restringe el acceso a Internet a un servidor interno, aceptando el tráfico de partes externas y reenviándolo a los servidores internos.
  - **Servidor proxy de correo electrónico:** Filtra el correo electrónico no deseado verificando la dirección del remitente, reduciendo el riesgo de ataques de phishing.

Diferencias entre el de reenvio y el inverso

| Característica | Servidor proxy de reenvío                                    | Servidor proxy inverso                                     |
| :------------- | :----------------------------------------------------------- | :--------------------------------------------------------- |
| Función        | Regula el acceso del usuario a Internet                      | Regula el acceso a un servidor interno                     |
| Ubicación      | Entre el cliente y el servidor externo                       | Entre el servidor interno y el cliente externo             |
| Objetivo       | Ocultar la dirección IP del usuario y aprobar solicitudes salientes | Aceptar tráfico externo y reenviarlo a servidores internos |
| Ejemplo        | Empleado accediendo a Internet                               | Servidor web protegiendo su dirección IP                   |