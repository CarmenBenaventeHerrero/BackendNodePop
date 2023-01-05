# NodePop

Inicializar: 

```sh
npm install 
``` 

Cargar la data a la base de datos: 

```sh
npm run init-db
``` 

Lanzar la aplicación en desarrollo: 

```sh
npm run dev
``` 

Lanzar la aplicación en producción: 

```sh
npm start
``` 

## Documentación API

Lista de anuncios: 

GET /api/anuncios

```objeto
{
    "anuncio": [
    {
        name: "silla", 
        venta: true, 
        price: 73, 
        photo: "foto3", 
        tags: "work"
    },
    {
        name: "iphone10", 
        venta: false,  
        price: 345, 
        photo: "foto2", 
        tags: "mobile"
        },

    {
        name: "bicletaElectrica",
        venta: true,  
        price: 500, 
        photo: "foto1", 
        tags: "motor"
    },

    {
        name: "sillon", 
        venta: true,  
        price: 200, 
        photo: "foto", 
        tags: "lifestyle"},
    ]
}
```

Ejemplos de filtros: 
- Filtro por nombre: http://localhost:3000/api/anuncios?name=silla

- Filtro por precio: http://localhost:3000/api/anuncios?price=73 

- Filtro por tag: http://localhost:3000/api/anuncios?tags=mobile

- Filtro por venta: http://localhost:3000/api/anuncios?venta=true

- Paginación: http://localhost:3000/api/anuncios?skip=2&limit=1

- Ordenación: http://localhost:3000/api/anuncios?sort=price

- Selección campos: http://localhost:3000/api/anuncios?fields=name

- Obtener imagenes: http://localhost:3000/images/sofa.jpeg

