# VitePress Setup

An installation guide for the VitePress can be found on the [official Getting Started guide](https://vitepress.dev/guide/getting-started).

# To build the site, the following commands can be used:

```
npm run ptk:dev    # for rapid development
npm run ptk:build    # building the site to publish
npm run ptk:preview    # to view the built site locally
```

# A few Notes about Cloudflare Pages Deployment

The following build configurations for the Cloudflare Pages project can be used:

```
Build command: npm run ptk:build
Build output directory: /protecttranskids/.vitepress/dist/
Root directory: /
```

where because `package.json` file is stored under the root directory, there is no need to alter the `Root directory` under `Build configurations`.

n.b., the default Node.js version used by Cloudflare is v12, we need v16. This entails [adding the environment variable](https://developers.cloudflare.com/pages/platform/build-configuration/) `NODE_VERSION` with value `16`.
