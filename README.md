# My ESLint config

## Whats included?

- Standard config base;
- React plugin;
- Next plugin;
- Node plugin;
- React Hooks plugin;
- JSX a11y plugin;
- Prettier;
- Import Helpers to Next.js projects

## Setup

1. Install the dependencies
```
npm i -D eslint @brunopavese/eslint-config
```

2. Create a `.eslintrc.json` file extending the config:
```
{
  "extends": "@brunopavese/eslint-config/react"  //For React projects
  "extends": "@brunopavese/eslint-config/next"   //For Next projects
  "extends": "@brunopavese/eslint-config/node"   //For Node projects
}
```

3. If you are using Visual Studio Code as your IDE, add these settings to your IDE's settings.json file:
```
{
  "diffEditor.ignoreTrimWhitespace": false,
  "editor.tabSize": 2,
  "editor.formatOnSave": false,
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true,
    "source.addMissingImports": true
  } 
  "eslint.enable": true,
}
```