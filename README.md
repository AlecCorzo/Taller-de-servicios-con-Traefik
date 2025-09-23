# Taller-de-servicios-con-Traefik

## Integrantes
David Fernando Cifuentes Bohorquez - 202221101
Alec Fabian Corzo Salazar - 202220646

### 1) Topología y redes (Compose)
● Una red de aplicación única donde vivan: traefik, api (réplicas), neo4j.
● No publicar puertos del contenedor de Neo4j hacia el host (acceso solo
interno).
● Traefik con entrypoint web (:80).

![Imagen 1](imagen1)

Se modifica el Dockercompose



![Imagen 1](imagen2)

Evidencia de que ya no funciona sin los puertos

### 2) Rutas “estructuradas”
● API disponible en http: /api.localhost/ o
http: /api.localhost/v1/.
● Dashboard de Traefik disponible únicamente en:
○ http: /ops.localhost/dashboard/ y protegido por middleware
(ver punto 3)

![Imagen 3](imagen3)

Se muestra el curl con el status y que responde a 200-

![Imagen 4](imagen4)

solicita credenciales o es inaccesible si no pasa por el middleware de protección.


