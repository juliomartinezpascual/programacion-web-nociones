<p align="center">
  <img src="./assets/logo-pascual-bravo.png" alt="Institución Universitaria Pascual Bravo" width="300" />
</p>

# Programación Web — Resumen de conceptos importantes

Institución Universitaria Pascual Bravo

## Mapa y orden de estudio

```mermaid
mindmap
  root((Programacion web))
    Fundamentos
      Internet vs Web
      URI URL URN
      Cliente servidor
      Capas 1 2 3 n-tier
    HTTP y servidores
      Protocolos
      Peticion y respuesta
      Servidor web
    APIs
      Contrato
      REST
      Otros estilos
    MongoDB
      Documentos y colecciones
      CRUD
    Seguridad
      AuthN y AuthZ
      HTTPS y amenazas
```

```mermaid
flowchart LR
    A["01 Fundamentos"] --> B["02 HTTP"]
    B --> C["03 APIs"]
    C --> D["04 MongoDB"]
    D --> E["05 Seguridad"]
    E --> F["06 Anexos"]
```

## Flujo de una petición

```mermaid
sequenceDiagram
    participant C as Cliente
    participant S as Servidor API
    participant DB as MongoDB

    C->>S: 1 Peticion HTTP o HTTPS
    S->>S: 2 AuthN AuthZ y logica
    S->>DB: 3 Consulta opcional
    DB-->>S: Datos
    S-->>C: 4 Respuesta HTTP
```

## Capítulos

| # | Archivo | Contenido |
|---|---------|-----------|
| 01 | [Fundamentos web](./01-fundamentos-web.md) | Internet vs Web, URI/URL, cliente-servidor, 1/2/3/n-tier |
| 02 | [HTTP, protocolos y servidores](./02-http-protocolos-y-servidores.md) | Protocolos, peticiones, respuestas, servidores web |
| 03 | [APIs](./03-apis.md) | Qué es una API, REST/RESTful, otros estilos y casos de uso |
| 04 | [MongoDB](./04-mongodb.md) | Documentos, colecciones, CRUD, modelado |
| 05 | [Seguridad](./05-seguridad.md) | AuthN/AuthZ, tipos de autenticación, amenazas básicas |
| 06 | [Anexos](./06-anexos.md) | Ejemplo integrado y glosario |
