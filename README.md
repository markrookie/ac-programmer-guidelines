# Please carefully read this guideline before writing your code.
## 1. Install eslint
Before starting the project development, it's essential to install eslint. You can do this by running the following command in the root directory of your project:

```npm install eslint --save-dev```

Or, if you're using yarn:

```yarn add eslint --dev```

## 2. Install Airbnb JavaScript Code Style
We recommend using the Airbnb JavaScript code style because it's widely adopted and helps maintain code consistency and readability. To install the Airbnb JavaScript code style, you can run the following command:

```npx install-peerdeps --dev eslint-config-airbnb```

Or, if you're using yarn:

```yarn add eslint-config-airbnb --dev```

## 3.  Eslint rule
The following eslint rule is required. Please copy and paste it into the ESLint configuration file of your project. it is json style rule if you use js style rule file, you need to convert it to js style.
```
"rules": {
    "indent": ["error", 4, { "SwitchCase": 1,"flatTernaryExpressions": true }],
    "max-len": ["error", { "code": 120, "ignoreUrls": true }],
    "react/jsx-indent": ["error", 4],
    "react/jsx-indent-props": ["error", 4],
    "react/jsx-filename-extension": ["warn", { "extensions": [".js",".jsx"] }],
    "react/prop-types": "off",
    "no-unused-expressions": ["error", { "allowShortCircuit": true }],
    "no-underscore-dangle": 0,
    "no-console": ["error", { "allow": ["log", "warn"] }],
    "react/jsx-props-no-spreading": ["error", { "custom": "ignore" }],
    "class-methods-use-this": "off",
    "import/no-cycle": 0,
    "radix": ["error", "always"],
    "no-restricted-syntax": ["error", "ForInStatement"],
    "react/jsx-tag-spacing": ["error", {"beforeSelfClosing": "never"}],
    "react/function-component-definition": [2, { "namedComponents": "arrow-function" }],
    "import/prefer-default-export": "off"
  }
```

## 4. Use eslint
Install an eslint plugin in your editor to check code style in real-time while writing code. Most mainstream editors have eslint plugins available, such as Visual Studio Code, Atom, Sublime Text, etc.

During project development, ensure that you follow the code style to maintain clear and readable code. Before committing code changes, run eslint to check code style and fix any issues reported by [eslint](https://eslint.org/).

## 5. FAQ
How to name folders, file names, class names, and variables. If you are unsure about the rules, please refer to the guidelines in the [Airbnb JavaScript Code Style](https://github.com/airbnb/javascript)
