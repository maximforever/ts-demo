# TypeScript Demo

- `npm install -g typescript`
- run with `tsc -w` (the watch flag regenerates the JS every time you save). If server side, add this to your `npm run start` - I think you can just `command1 && command2` (I like [npm-run-all](https://www.npmjs.com/package/npm-run-all) for this)
-  any TS file you save is then compiled to a JS file in `/dist` and maintains the directories for you. The directory is specified in `tsconfig.json`
-  there's no `dist` folder right now because there are TS errors, and I've set `noEmitOnError` in tsconfig to `true`
- once it's generated, don't touch anything in `dist`; that's now generated automatically
- check the terminal for any typescript errors
- you'll need a little bit of setup for linting & autocomplete (TS calls this "intellisense"). In Sublime 4, install `LSP` and `LSP-typescript`. You might have to restart the app for this to take effect, but this should highlight errors and suggest TS types as you type.
- check out `tsconfig.json` for important config
- enjoy writing much better code and occasionally wanting to tear your hair out