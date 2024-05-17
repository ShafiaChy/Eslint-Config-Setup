# **Instruction**

**Step - 1:** Create an `eslint.config.mjs` and copy the code from: 
<br> 
[Eslint File](https://github.com/ShafiaChy/Eslint-Config-Setup/blob/main/eslint.config.mjs)
<br>

*Delete the files `eslintrc` and `.eslintignore`*

**Step - 2:** Copy/paste the following lines and paste inside `script` in `package.json` code from given in the package.json
```

    "lint": "npx eslint src --ignore-pattern .ts",
    "lint:fix": "npx eslint src --fix",
    "prettier": "prettier --ignore-path .gitignore --write \"./src/**/*.+(js|ts|json)\"",
    "prettier:fix": "npx prettier --write src",

```

<br>

**Step - 3:** Install the `prettier` package

```
    npm install --save-dev prettier
```

<br>

<br>

*If prettier does not work*, follow step 4:

**Step - 4:** Add the code below to the `settings.json` file:

```
      "editor.defaultFormatter": "esbenp.prettier-vscode",
      "editor.formatOnSave": true,
```

<br>
