# React JS setup with ESLint and Prettier

## Step 01:
Create react app with the following command
```
npx create-react-app my-app
```
Then go to the project folder using the following command
```
cd my-app/
```

## Step 02:
Open git bash in the root directory of your project and use the following command to install dependencies
```
npm i -D eslint eslint-config-prettier eslint-plugin-prettier prettier
```

## Step 03:
Create `.eslintrc` config file in the root directory of project by using the following command
```
touch .eslintrc
```
Then open `.eslintrc` file and paste the following settings:
```
{
  "parserOptions": {
    "ecmaVersion": 12,
    "sourceType": "module",
    "ecmaFeatures": {
      "jsx": true
    }
  },
  "extends": ["plugin:prettier/recommended"],

  "plugins": ["prettier"],

  "rules": {
    "prettier/prettier": [
      "error",
      {
        "endOfLine": "auto"
      }
    ]
  }
}
```

## Step 04:
Create `.prettierrc` config file in the root directory of project by using the following command
```
touch .prettierrc
```
Then open `.prettierrc` file and paste the following settings:
```
{
  "printWidth": 80,
  "tabWidth": 2,
  "semi": true,
  "singleQuote": true,
  "trailingComma": "es5",
  "bracketSpacing": true,
  "jsxBracketSameLine": false
}
```

## Step 05:
Look for `formatOnSave` and check the checkbox, or add this line to `settings.json`:
```
"editor.formatOnSave": true,
```

## Step 06:
Start your react app by the following command
```
npm start
```
#### If you're having trouble try restarting Visual studio code or clone the git repository and replace the files with your project files.

#### Now restart VScode and start your react app agian.

#### Main post link: https://dev.to/chgldev/getting-prettier-eslint-and-vscode-to-work-together-3678

#### Happy coding :)
