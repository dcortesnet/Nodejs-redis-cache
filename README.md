# Nodejs Redis cache &middot; ![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)

Proyecto de laboratorio para realizar una comparación objetiva de los tiempos de respuesta de una aplicación utilizando Redis.
En la aplicación se utiliza una API de terceros como fuente de información llamada SpaceX.

## Tabla comparativa resultados

* API utilizadada SpaceX: ```https://api.spacexdata.com/v3/rockets```
* URL Solicitudes con redis ```http://localhost:3000/with-redis-rockets```
* URL Solicitudes sin redis ```http://localhost:3000/without-redis-rockets```

NOTA: Por cada endpoint se realizarón X peticiones (30 en este ejemplo), estas fueron promediadas dando los siguientes resultados.

| Con redis promedio | Sin redis promedio |
| -- | --  |
| 6 ms | 236 ms

|Resultado y conclusiones |

Con Redis la respuesta es 95.76% más rápida.

## Instalación

Ejecutar comando

```
$ npm install
```

## Levantar proyecto

```
$ docker run --name rdb -p 6379:6379 redis
$ npm run dev
```

## Equipo

Desarrollado por Diego Cortés

* dcortes.net@gmail.com
