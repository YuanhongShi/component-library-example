# What is this package?

## This is an example of how to publish a typescript package to npm library

-   \*scripts inside of package.json -- Windows

```
        "clean": "rd /s /q dist",
        "build": "rd /s /q dist && prettier --write src/ & npm run build:esm && npm run build:cjs ",
        "build:esm": "tsc",
        "build:cjs": "tsc --module CommonJS --outDir dist/cjs"
```

-   \*scripts inside of package.json -- Mac or Linux

```
        "clean": "rm -f dist/",
        "build": "rm -f dist/ && prettier --write src/ & npm run build:esm && npm run build:cjs ",
        "build:esm": "tsc",
        "build:cjs": "tsc --module CommonJS --outDir dist/cjs"
```

## Instruction for publishing

```
<!-- login to npm first -->
npm login
```

```
<!-- publish to npm library -->
npm publish
```
