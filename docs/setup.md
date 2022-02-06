
# Monorepo Setup
Install nx
```bash
npm i nx
```

install nx cli
```bash
npm install -g @nrwl/cli
```

Install seed
```bash
npx create-nx-workspace@latest nx-nestjs-react-starter
```

Add Nest
```bash
npm install -D @nrwl/nest
```

Add Nest app to nx workspace
```bash
npx nx g @nrwl/nest:app api --frontendProject=client
```

Test & lint all (packae.json)
```bash
"test": "npx nx run-many --all --target=test --parallel"
"lint": "nx workspace-lint && npx nx run-many --all --target=lint --parallel"
```

Build&run separately (packae.json)
```bash
"start:client": "nx run client:serve"
"start:api": "nx run api:serve"
```

## Empower Workspace

React
```bash
npm install --save-dev @nrwl/react
```
Nest
```bash
npm install --save-dev @nrwl/nest
```
Node
```bash
npm install --save-dev @nrwl/node
```

## Create App
```bash
nx g @nrwl/react:app my-app
```

## Create Library
```bash
nx g @nrwl/react:lib my-lib
```

# Run apps
```bash
nx serve client
```

```bash
nx serve api
```

