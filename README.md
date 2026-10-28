# React CRUD Sprint

React (Vite) + Tailwind CSS app that performs all four CRUD operations against the
[DummyJSON Products API](https://dummyjson.com/docs/products).

| Operation | Endpoint | Where in the app |
|-----------|----------|------------------|
| GET    | `GET https://dummyjson.com/products?limit=10` | Product list loads on page open |
| POST   | `POST https://dummyjson.com/products/add`     | "Add Product" form |
| PUT    | `PUT https://dummyjson.com/products/:id`      | "Update" → edit → "Save" |
| DELETE | `DELETE https://dummyjson.com/products/:id`   | "Delete" button |

DummyJSON only simulates writes (nothing is saved on the server), so the app updates
React state after each successful request to make the change visible.

## Run locally

```bash
npm install
npm run dev
```

Open http://localhost:5173

## Tech

- React 19 + Vite
- Tailwind CSS v4 (`@tailwindcss/vite` plugin)
- Native `fetch` for API calls (`src/api.js`)
