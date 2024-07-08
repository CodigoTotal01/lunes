# Full Stack E-Commerce + Dashboard & CMS: Next.js 13 App Router, React, Tailwind, Prisma, Postgresql

Este es un repositorio para un Full Stack E-Commerce + Dashboard & CMS: Next.js 13 App Router, React, Tailwind, Prisma, MySQL

Características principales:

- ¡Vamos a utilizar Shadcn UI para el Admin!
- ¡Nuestro panel de control de administración va a servir como CMS, Admin y API!
- ¡Usted será capaz de controlar múltiples vendedores / tiendas a través de este único CMS! (Por ejemplo, usted puede tener una "tienda de ropa" y una "tienda de zapatos" y una "tienda de trajes", y nuestro CMS generará rutas API para todos ellos individualmente).
- Podrá crear, actualizar y eliminar categorías.
- Podrá crear, actualizar y eliminar productos.
- ¡Podrás subir múltiples imágenes para los productos, y cambiarlas cuando quieras!
- Podrá crear, actualizar y eliminar filtros como "Color" y "Talla", y luego hacerlos coincidir en el formulario de creación de "Producto".
- Podrá crear, actualizar y eliminar "Carteles", que son esos grandes textos que aparecen en la parte superior de la página. Podrá adjuntarlos a una sola categoría, o utilizarlos de forma independiente (¡Nuestro Admin genera API para todos esos casos!)
- Podrá buscar en todas las categorías, productos, tallas, colores y carteles con paginación incluida.
- ¡Usted será capaz de controlar qué productos son "destacados" para que se muestren en la página principal!
- Podrá ver sus pedidos, ventas, etc.
- Podrá ver gráficos de sus ingresos, etc.
- Aprenderá la autenticación de clientes.
- Creación de pedidos
- Pago con Stripe
- Webhooks de Stripe
- MySQL + Prisma + PlanetScale
### Prerrequisitos

**Nodo versión 14.x

### Instalar paquetes

```shell
npm i
```

### Setup .env file

```js
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/

# Esto fue insertado por `prisma init`:
# Las variables de entorno declaradas en este archivo se ponen automáticamente a disposición de Prisma.
# Ver la documentación para más detalles: https://pris.ly/d/prisma-schema#accessing-environment-variables-from-the-schema

# Prisma soporta el formato nativo de cadena de conexión para PostgreSQL, MySQL, SQLite, SQL Server, MongoDB y CockroachDB.
# Ver la documentación para todas las opciones de cadena de conexión: https://pris.ly/d/connection-strings

DATABASE_URL=''
NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME=""
STRIPE_SECRET_KEY=
FRONTEND_STORE_URL=http://localhost:3001
STRIPE_WEBHOOK_SECRET=
```

### Conectar a PlanetScale y Push Prisma

```shell
npx prisma generate
npx prisma db push
```

### Iniciar la aplicación

```shell
npm run dev
```

## Comandos disponibles

Ejecutar comandos con npm `npm run [command]`

| comando | descripción |
| :------ | :--------------------------------------- |
| `dev` | Inicia una instancia de desarrollo de la aplicación |
