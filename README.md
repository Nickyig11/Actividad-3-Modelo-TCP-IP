# Modelo TCP/IP

## Actividad 1.1: Expresar la IP 192.168.0.1 en formato binario. Puedes usar la calculadora.
11000000.10101000.00000000.00000001


## Actividad 1.2: Expresar la MAC 94:DE:80:80:72:AF en formato binario. Puedes usar la calculadora.
10010100.11011110.10000000.10000000.01110010.10101111

## Actividad 1.3: Describir un envío de correo electrónico a través de las capas del modelo TCP-IP
- Capa de Aplicación: Usuario redacta un correo electrónico.
- Capa de Transporte: El cliente divide el correo en paquetes y los pasa a SMTP.
- Capa de Internet: Los paquetes se envían a través de la red usando direcciones IP.
- Capa de Acceso a la Red: Los paquetes viajan a través de dispositivos de red.
- Capa Física: Los bits viajan físicamente a través de cables u otros medios.

## Actividad 1.4: ¿Cómo influye el cambio del protocolo IPv4 a IPv6 en el protocolo TCP?
IPv6 ofrece un espacio de direcciones más grande, pero no es un cambio notorio por el usuario, esto se hizo porque internet se estaba quedando sin espacio de direcciones.

## Actividad 1.5: Si navegando por internet no nos muestra la página web en nuestro navegador ¿en qué capa del modelo TCP/IP se está produciendo el problema?
Problema puede estar en la capa de Aplicación si hay un problema con el navegador o en la capa de Internet si hay problemas con la resolución DNS o conectividad IP.

## Actividad 1.6: ¿Cómo puedo saber la IP del servidor web www.ieslafuensanta.es?
Se puede saber con el comando nslookup en el cmd que nos da 217.160.0.19

## Actividad 1.7: Si enviamos un ping a un equipo y este no responde ¿Qué capa del nivel TPC/IP está fallando?
Dependiendo de la capa

- Capa de Aplicación: el protocolo web no permite ver el equipo
- Capa de Transporte: El cliente divide el correo en paquetes pero estos fallan al reunisrse
- Capa de Internet: hay un firewall que no permite el acceso.
- Capa de Acceso a la Red: Los paquetes se pierden.
- Capa Física: Algunos de los cables esta mal montado.

## Actividad 1.8: ¿Qué conexiones tenemos abiertas desde nuestro equipo?
Con el comando "netstat" se puede ver:
```
  Proto  Dirección local        Dirección remota       Estado
  TCP    127.0.0.1:11300        1119PC17:54198         ESTABLISHED
  TCP    127.0.0.1:54198        1119PC17:11300         ESTABLISHED
  TCP    192.168.119.29:7680    pc110901:50415         TIME_WAIT
  TCP    192.168.119.29:7680    win-3gjsms9clad:27649  TIME_WAIT
  TCP    192.168.119.29:7680    pc112000:53767         TIME_WAIT
  TCP    192.168.119.29:7680    departamento02:56995   TIME_WAIT
  TCP    192.168.119.29:54119   20.54.36.229:https     ESTABLISHED
  TCP    192.168.119.29:55655   wh-in-f188:5228        ESTABLISHED
  TCP    192.168.119.29:55876   20.42.65.84:https      ESTABLISHED
  TCP    192.168.119.29:55884   iniciarte:https        ESTABLISHED
  TCP    192.168.119.29:55896   a23-58-159-137:https   ESTABLISHED
  TCP    192.168.119.29:55897   20.189.173.24:https    ESTABLISHED
  TCP    192.168.119.29:55898   152.199.19.161:https   ESTABLISHED
  TCP    192.168.119.29:55899   4.150.240.254:https    ESTABLISHED
  TCP    192.168.119.29:55900   13.107.246.43:https    ESTABLISHED
  TCP    192.168.119.29:55901   204.79.197.222:https   ESTABLISHED
  TCP    [fe80::1dc3:febc:6719:51ca%9]:1521  1119PC17:49691         ESTABLISHED
  TCP    [fe80::1dc3:febc:6719:51ca%9]:49691  1119PC17:1521          ESTABLISHED

```

## Actividad 1.9: ¿Podría navegar por internet sin DNS?
No puedes visitar un sitio web sin acceder a un servidor de nombres de dominio.

## Actividad 1.10: ¿Cómo puedo saber la MAC de un equipo de mi red con IP 192.168.0.10?
arp -a" para consultar la tabla ARP.

## Actividad 1.11: ¿Por qué al configurar manualmente la IP en muchos dispositivos cuando escribimos la IP 222.222.222.222 nos sugiere la máscara 255.255.255.0 y en cambio cuando escribimos la IP 22.22.22.22 nos sugiere la máscara 255.0.0.0?
La sugerencia de máscara depende de la clase de dirección IP y del rango de direcciones que se desee incluir en la misma red.

## Actividad 1.12: En una típica red privada con un router que tiene la IP 192.168.0.1 y máscara /24 (255.255.255.0) ¿Cuántos dispositivos entre sobremesas, portátiles, móviles, etc. podemos conectar?
Con una máscara de /24, se pueden conectar hasta 254 dispositivos.


## Actividad 1.13: ¿Es correcto identificar una red con 10.0.0.1/8?
No

## Actividad 1.14: Resume lo máximo posible las siguientes direcciones IPv6 2000:0002:2000:0002:2000:0002:2000:0002 0000:0000:0000:0000:0000:0000:0000:000A
- 2000:2:2000:2:2000:2:2000:2
- ::A

## Actividad 1.15: Detalla con todos los caracteres las siguientes IPv6 2::A000 2222:0:0:2::A0C
- 0002:0000:0000:0000:0000:0000:0000:A000
- 2222:0000:0000:0000:0000:0000:0002:A0C

## Actividad 1.16: Reflexiona sobro cómo afectará el internet de las cosas al direccionamiento (Internet of things, consiste en conectar los objetos cotidianos como electrodomésticos, coches, semáforos, alarmas, etc. a internet para poderlos controlar desde cualquier lugar. Esto supondrá en 2020 que unos 50.000 millones de dispositivos se conectarán a Internet).
El Internet de las cosas requerirá un direccionamiento más escalable y eficiente, lo que lo hace apto para IPv6. Este protocolo ofrece un espacio de direcciones suficientemente grande para asignar una dirección única a cada dispositivo IoT, facilitando su gestión y conectividad.






