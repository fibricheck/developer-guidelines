---
description: >-
  In our frontend projects we are striving to use React in combination with
  Typescript. This for creating a better harmony between code en developers
---

# Typescript

### Tsconfig

For React Typescript projects, we are using this `tsconfig` configuration

```typescript
{
  "compilerOptions": {
    "allowJs": true,
    "baseUrl": ".",
    "forceConsistentCasingInFileNames": true,
    "importHelpers": true,
    "jsx": "react",
    "lib": [
      "es6",
      "dom"
    ],
    "module": "ESNext",
    "moduleResolution": "node",
    "noImplicitAny": true,
    "noImplicitThis": true,
    "noUnusedLocals": true,
    "noUnusedParameters": true,
    "outDir": "dist",
    "removeComments": true,
    "sourceMap": true,
    "strictNullChecks": true,
    "suppressImplicitAnyIndexErrors": true,
    "target": "es5",
    "skipLibCheck": true,
    "esModuleInterop": true,
    "allowSyntheticDefaultImports": true,
    "strict": true,
    "resolveJsonModule": true,
    "isolatedModules": true,
    "noEmit": true
  },
  "exclude": [
    "acceptance-tests",
    "build",
    "dist",
    "jest",
    "node_modules",
    "scripts",
    "webpack"
  ],
  "include": [
    "src"
  ]
}
```

### Type Declarations

We also need a `global.d.ts` in our root for the correct usage of images and json files

```typescript
declare module '*.svg';
declare module '*.png';
declare module '*.jpg';
declare module '*.jpeg';
declare module '*.gif';
declare module '*.bmp';
declare module '*.tiff';
declare module '*.json' {
  const value: any;
  export default value;
}
```

