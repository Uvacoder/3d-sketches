# 3D Sketches

### Canvas Sketch

```sh
cd 3d-sketches
$ npm install
$ npm start sketches/sketch_name.js
```

## Gallery App

### Get started

Install the dependencies...

```bash
cd 3d-sketches
$ npm install
```

...then start [Rollup](https://rollupjs.org):

```bash
npm run app:dev
```

Navigate to [localhost:5000](http://localhost:5000). You should see your app running. Edit a component file in `src`, save it, and reload the page to see your changes.

By default, the server will only respond to requests from localhost. To allow connections from other computers, edit the `sirv` commands in package.json to include the option `--host 0.0.0.0`.


## Building and running in production mode

To create an optimised version of the app:

```bash
npm run app:build
```

You can run the newly built app with `npm run app:start`. This uses [sirv](https://github.com/lukeed/sirv), which is included in your package.json's `dependencies` so that the app will work when you deploy to platforms like [Heroku](https://heroku.com).


## Single-page app mode

By default, sirv will only respond to requests that match files in `public`. This is to maximise compatibility with static fileservers, allowing you to deploy your app anywhere.

If you're building a single-page app (SPA) with multiple routes, sirv needs to be able to respond to requests for *any* path. You can make it so by editing the `"app:start"` command in package.json:

```js
"app:start": "sirv public --single"
```
