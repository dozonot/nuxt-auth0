# nuxt-auth0

> My laudable Nuxt.js project

## Setup

- Replace YOUR_DOMAIN, and YOUR_CLIENT_ID in nuxt.config.js

```javascript
export default {
  mode: 'spa',
  auth: {
    strategies: {
      auth0: {
        domain: 'YOUR_DOMAIN',
        client_id: 'YOUR_CLIENT_ID'
      }
    },
    redirect: {
      login: '/login',
      logout: '/logout',
      callback: '/callback',
      home: '/profile'
    }
  },
```

## Build Setup

``` bash
# install dependencies
$ yarn install

# serve with hot reload at localhost:3000
$ yarn dev

# build for production and launch server
$ yarn build
$ yarn start

# generate static project
$ yarn generate
```

For detailed explanation on how things work, check out [Nuxt.js docs](https://nuxtjs.org).
