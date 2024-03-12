<h1 align="center">
  <br>
  <a href="https://htmlhint.com"><img src="https://raw.githubusercontent.com/htmlhint/HTMLHint/master/website/static/img/htmlhint.png" alt="Logo HTMLHint" width="170"></a>
  <br>
  HTMLHint
  <br>
</h1>

<h4 align="center">The static code analysis tool you need for HTML.</h4>


<p align="center">
  <a href="#-installation-and-usage">How To Use</a> • <a href="#contributing">Contributing</a> • <a href="https://htmlhint.com">Website</a>
</p>

## Table of Contents

- **[Installation and Usage](#-installation-and-usage)**
  - **[Local Installation and Usage](#local-installation-and-usage)**
  - **[Global Installation and Usage](#global-installation-and-usage)**
- **[Example output](#-example-output)**
- **[Configuration](#-configuration)**
- **[Docs](#-docs)**

## 📟 Installation and Usage

There are two ways to install HTMLHint: globally and locally.

### Local Installation and Usage

In case you want to include HTMLHint as part of your project, you can install it locally using npm:

```
$ npm install htmlhint --save-dev
```

After that, You can run HTMLHint on any file or directory like this:

```
$ ./node_modules/.bin/htmlhint www/index.html
$ ./node_modules/.bin/htmlhint www/**/*.html
```

### Global Installation and Usage

If you want to make HTMLHint available to tools that run across all of your projects, you can install HTMLHint globally using npm:

```
$ npm install htmlhint -g
```

After that, you can run HTMLHint on any file like this:

```
$ htmlhint www/index.html
$ htmlhint www/**/*.html
```

You can even launch HTMLHint to analyze an URL:

```
$ htmlhint https://htmlhint.com/
```

## 📃 Example output

## 🔧 Configuration

Search `.htmlhintrc` file in current directory and all parent directories:

```
$ htmlhint
$ htmlhint test.html
```

Custom config file:

```
$ htmlhint --config htmlhint.conf test.html
```

Custom rules:

```
$ htmlhint --rules tag-pair,id-class-value=underline index.html
```

Inline rules in `test.html`:

```html
<!--htmlhint tag-pair,id-class-value:underline -->
<html>
  <head>
    ...
  </head>
</html>
```

## 📙 Docs

1. [How to use](https://htmlhint.com/docs/user-guide/usage/cli)
2. [All Rules](https://htmlhint.com/docs/user-guide/list-rules)
3. [How to Develop](CONTRIBUTING.md)


