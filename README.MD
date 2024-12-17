# NLW NearBy - React Native

A React Native app that shows restaurantes/locations near the person and scans QRCode for coupons of discount of that location.

The API was given in course, with mock data - it was not "touched".
Only used the routes in app.

## API Documentation

#### Returns all categories

"Cinema, restaurant, gym, ..."

```http
  GET /categories
```

#### Returns Locations by Category

Shows Markets within the Category

```http
  GET /markets/category/:category_id
```

| Parâmetro | Tipo     | Descrição    |
| :-------- | :------- | :----------- |
| `id`      | `string` | **Required** |

#### Returns one Location/Market

```http
  GET markets/:id
```

| Parâmetro | Tipo     | Descrição    |
| :-------- | :------- | :----------- |
| `id`      | `string` | **Required** |

#### Update coupons

Finds the market (location) and then decrement the coupon by 1.
(Showing it was used)

```http
  PATCH /coupons/:market_id
```

| Parâmetro   | Tipo     | Descrição    |
| :---------- | :------- | :----------- |
| `market_id` | `string` | **Required** |

![Rockteseat Image for Nearby app](https://s3-figma-hubfile-images-production.figma.com/hub/file/carousel/img/62a5a655cbf76d891ba67ed9258981cc0d212974/bf5058de77dafa65aa6daee4d64e878dc681edfc)

## Autores

- [@Matheus Padilha](https://www.github.com/Padilha1)
- [@Rocketseat](https://www.github.com/rocketseat-education)
