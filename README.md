# Deno project setup

## VS Code

- Instal [VS Code plugin](https://marketplace.visualstudio.com/items?itemName=denoland.vscode-deno)
- Make sure VS Code is using lates version of TypeScript. `npm install -g typescript@latest`
- If plugin seems to not work properly, you should edit your `settings.json` to refference valid version.

*Example for nvm:*
```
"typescript.tsdk": "somewhere/.nvm/versions/node/v12.18.0/lib/node_modules/typescript/lib"
```
*Example for node:*
```
//path to latest typescript
"typescript.tsdk": "/usr/local/lib/node_modules/typescript/lib/"
```
notice "somwhere" is place of your nvm

- run command
```
deno run --allow-net --importmap=import_map.json --unstable -c tsconfig.json server.ts
```