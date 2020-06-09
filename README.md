# Deno project setup

## VS Code

- Instal [VS Code plugin](https://marketplace.visualstudio.com/items?itemName=denoland.vscode-deno)


- run command
```bash
deno run --allow-net --importmap=import_map.json --unstable -c tsconfig.json server.ts
```
Done! 🔥💪🏼🚀👩🏽‍🚀

### Comon problems

### Plugin not working
It's posible TypeScript version deffrence between VS Code and Plugin
- Make sure VS Code is using lates version of TypeScript. `npm install -g typescript@latest`
- Edit your `settings.json` to refference latest valid version.


*Example for nvm:*
```json
"typescript.tsdk": "somewhere/.nvm/versions/node/v12.18.0/lib/node_modules/typescript/lib"
```
notice "somwhere" is place of your nvm


*Example for node:*
```ts
"typescript.tsdk": "/usr/local/lib/node_modules/typescript/lib/"
```

Done! 🔥💪🏼🚀👩🏽‍🚀