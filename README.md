# Ideahut Admin&nbsp;&nbsp;<img height="32" src="https://avatars.githubusercontent.com/u/146613481?v=4">&nbsp;<img height="32" src="https://avatars.githubusercontent.com/u/23064371?s=200&v=4">

* User Interface (UI) Admin untuk Framework __Ideahut__.
    * [<img height="16" src="https://github.com/ideahut-apps-team/Ideahut-Spring-Boot/blob/main/docs/assets/spring-boot.png?raw=true" alt="">&nbsp;Spring Boot](https://github.com/ideahut-apps-team/Ideahut-Spring-Boot/blob/main/docs/22-admin.md)
    * [<img height="16" src="https://github.com/ideahut-apps-team/Ideahut-Quarkus/blob/main/docs/assets/quarkus.png?raw=true" alt="">&nbsp;Quarkus](https://github.com/ideahut-apps-team/Ideahut-Quarkus/blob/main/docs/22-admin.md)
* Dibuat menggunakan Framework [<img height="16" src="https://avatars.githubusercontent.com/u/23064371?s=200&v=4">&nbsp;Quasar](https://quasar.dev/).

##

### Install

```bash
yarn
# or
npm install
```

### Lint

```bash
yarn lint
# or
npm run lint
```

### Format

```bash
yarn format
# or
npm run format
```

### Icon
```bash
icongenie generate -m spa -i icon-512x512.png
```

### Development

```bash
quasar dev
```

### Production

```bash
quasar build
```

### Customize

See [Configuring quasar.config.js](https://v2.quasar.dev/quasar-cli-vite/quasar-config-js).

### Environment

Edit file [env.js](./src/scripts/env.js)
* Eksternal
    ```js
    web: "",
    api: "http://localhost:5402/_/api", // Base URL admin di backend
    ```
    * Untuk mode development pakai setting ini.
* Internal
    ```js
    web: "/__admin__",
    api: "/_/api",
    ````
    * Hasil _build_ SPA (di folder dist), bisa digunakan sebagai static resource di backend.