### Antes de empezar
---

### Requisitos previos
El equipo de IronIA le habrá suministrado un **API key** y un **API secret** para poder acceder al API.

### Usando el API
Url del servicio en función del entorno:
* Pruebas: https://api.iron-ia.com (actualmente https://open-api-dev-6dd675tf.ew.gateway.dev)
* Producción: https://api.ironia.tech

Formato de las peticiones:
Todas las peticiones deben incluir las siguiente cabeceras:
x-api-key
x-api-secret

La información de cada operación se transmitirá al servidor a través de variables en el cuerpo de la petición.

Ejemplo de petición:
```console
api@ironia:~$ curl -H 'Content-Type: application/json' -H "x-api-key: AIzaSyBymfe0Mbk3sJRkotaUzXI1RT1Bbhg9cEE" -H "afilliate-id: b1268t97-d1e3-4276-a9f9-b2c5729a68df" -H "secret-id: 123321" -X POST https://open-api-dev-6dd675tf.ew.gateway.dev/signup --data '{"user":"monxela@gmail.com","promotions":[{"code":444555666}]}'
```
