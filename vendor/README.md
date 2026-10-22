`tidecloak-js-0.14.41.mjs` is the official TideCloak browser SDK (`@tidecloak/js` 0.14.41 from npm), bundled into one ES module with esbuild:

```bash
npm install @tidecloak/js@0.14.41 esbuild
echo "export { IAMService } from '@tidecloak/js';" > entry.mjs
npx esbuild entry.mjs --bundle --format=esm --platform=browser --target=es2020 --minify --outfile=tidecloak-js-0.14.41.mjs
```

It is loaded only in Live mode. Licence: Tide Community Open Code License (see `LICENSE-tidecloak-js.txt`).
