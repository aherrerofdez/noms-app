# noms-app

Created with Svelte (https://kit.svelte.dev/docs)

The icons used have been taken from "Material Design" (https://materialdesignicons.com/)

---

## Developing

Once you've downloaded the project and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server:

```bash
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```

## Building

Before creating a production version of your app, install an [adapter](https://kit.svelte.dev/docs#adapters) for your target environment. Then:

```bash
npm run build
```

> You can preview the built app with `npm run preview`, regardless of whether you installed an adapter. This should _not_ be used to serve your app in production.


---

**Current Limitations:**
1. Current "daily-recommendations" screen is not automated, and requires a svelte component for each recipe to be linked, which is not an efficient-coding practice.
2. The search function only works for exact matches, meaning if user inputs "avo" nothing will show, but if the user inputs "avocado" recipes with avocado will appear. However, it is not case sensitive, meaning if the user inputs "Avocado" or "avoCado" or any other variant, it will still show all the recipes that contain avocado.
      - Some filters could be added to improve the experience, such as "vegan" and "max number of recipes shown".
4. There is no filter for the bundles, and they are not linked to the recipes.
5. Series are only filtered by theme, but inside each theme, there is no way to filter the recipes. For instance, in "no-cook" series, all "no-cook series" recipes are displayed without any filtering.
