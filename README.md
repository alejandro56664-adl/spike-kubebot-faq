# spike-kubebot-faq
Kubebot-faq es un bot para slack que ayuda a entender y resolver problemas con despliegues en kubernetes. Es un spike para explorar el potencial de la herramienta Neo4j con base de datos de conocimiento.

# Contenido

- 1. Introducción
- 2. Instalación
- 

# Introducción

TODO: introducción
Responder a las preguntas: 

- ¿Por que surge la idea?
- ¿Qué problema resuelve?
- ¿Por qué es importante resolverlo?
- ¿Qué causa el problema?
- ¿Qué consecuencias tiene?


# Instalación

## Creación aplicación en Slack

## Ejecución en ambiente local

Una vez clonado el proyecto instale las dependencias:

```sh
npm install
```

Para ejecutar las pruebas automatizadas:
```sh
npm run test
````

Para ejecutar el lint (configurado con el estilo standard):

```sh
npm run lint
```

Se recomienda instalar _neo4j_ usando Docker:

TODO: crear un archivo docker-compose

```sh
docker run -p7474:7474 -p7687:7687 -e NEO4J_AUTH=neo4j/s3cr3t neo4j
````

Para hacer las pruebas remotas con la API de Slack, se usa ngrok, si no lo tiene instalado, lo puede instalar usando el siguiente comando:

```sh
npm install -g ngrok
```

## Arquitectura 

### Atributos de calidad

- TODO: listar los *ality mas importantes para este producto.

### Vista lógica
- diagrama de clases
- diagrama de estado

#### Modelo de datos (Grafo de conocimiento)

### Vista de proceso
- diagrama de secuencia
- diagrama de comunicación

### Vista de desarrollo
- diagrama de componentes

### Vista física
- diagrama de despliegue asociado a terraform.

### Vista de escenarios

- casos de uso
- user journy map

### Evaluación arquitectura con ATAM

Hacer un pequeño analisis de atam, responder con los patrones:
- Serverless en AWS (well architected framework) con nodejs (escalabilidad) modelo de concurrencia (basado en eventos)
- Base de datos NoSQL tipo grafos, que ventajas da, que se pierde

## Conclusión

TODO: que aporta este spike a la comunidad.

## Fuentes/Referencias
