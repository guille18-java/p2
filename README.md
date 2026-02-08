# Práctica 2 - API REST Carrito

API REST en Spring Boot que implementa CRUD para el recurso **Carrito** (cada carrito contiene un único producto).

## Modelo Carrito

- idCarrito (Long)
- idArticulo (Long)
- descripcion (String)
- unidades (Integer)
- precioFinal (Decimal)

## Endpoints

| Método | Ruta | Body | Descripción | Respuestas |
|-------:|------|------|-------------|------------|
| POST | /carritos | JSON Carrito (sin idCarrito) | Crea un carrito | 201, 400 |
| GET | /carritos | - | Lista todos los carritos | 200 |
| GET | /carritos/{id} | - | Obtiene un carrito por id | 200, 404 |
| PUT | /carritos/{id} | JSON Carrito | Actualiza un carrito existente | 200, 404 |
| DELETE | /carritos/{id} | - | Borra un carrito por id | 204, 404 |
