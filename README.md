# Astro Boilerplate with <ins>Svelte</ins>, TypeScript and Tailwind CSS

> This is a fork from [ixartz/astro-boilerplate-components](https://github.com/ixartz/astro-boilerplate-components) that allows you to transform the React Components into Svelte Components.

### Getting started

Run the following command on your local environment:

```
git clone --depth=1 https://github.com/ixartz/Astro-boilerplate
cd my-project-name
npm install
```

Change the dependency from `astro-boilerplate-components` to `astro-boilerplate-components-svelte`

```
npm uninstall astro-boilerplate-components
npm install astro-boilerplate-components-svelte
```

Change the astro react adapter into a svelte adapter: 

```
npm uninstall @astrojs/react
npm install @astrojs/svelte
```

Now you can adjust the components in `/partials` like e.g. `BlogPost.tsx` by creating `BlogPost.svelte`. And referencing the components from this package.


Then, you can run locally in development mode with live reload:

```
npm run dev
```

Open http://localhost:3000 with your favorite browser to see your project.

### Contributions

Everyone is welcome to contribute to this project. Feel free to open an issue if you have question or found a bug.

### License

Licensed under the MIT License, Copyright © 2024
