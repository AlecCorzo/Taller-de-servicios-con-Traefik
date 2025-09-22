# Taller-de-servicios-con-Traefik

##Integrantes
David Fernando Cifuentes Bohorquez - 202221101
Alec Fabian Corzo Salazar - 202220646

### 1) Topología y redes (Compose)
● Una red de aplicación única donde vivan: traefik, api (réplicas), neo4j.
● No publicar puertos del contenedor de Neo4j hacia el host (acceso solo
interno).
● Traefik con entrypoint web (:80).


![Imagen 1](ruta)
