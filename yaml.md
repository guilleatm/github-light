# YAML

## Introducción

*YAML* es un formato de serialización de datos legible por humanos, ampliamente utilizado para definir configuraciones debido a su simplicidad. No es un lenguaje de marcas, sino una forma de codificar datos de formato legible.

En ese sentido es parecido al formato `.json` aunque tiene una sintaxis completamente diferente.

A continuación un documento `.yaml`

```yaml
name: CI Pipeline

on:
  push:
  pull_request:

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout repository
        uses: actions/checkout@v2

      - name: Set up Node.js
        uses: actions/setup-node@v2

      - name: Install dependencies
        run: npm install

      - name: Run tests
        run: npm test
```

Y su correspondiente en `.json`

```json
{
  "name": "CI Pipeline",
  "on": {
    "push": {},
    "pull_request": {}
  },
  "jobs": {
    "build": {
      "runs-on": "ubuntu-latest",
      "steps": [
        {
          "name": "Checkout repository",
          "uses": "actions/checkout@v2"
        },
        {
          "name": "Set up Node.js",
          "uses": "actions/setup-node@v2"
        },
        {
          "name": "Install dependencies",
          "run": "npm install"
        },
        {
          "name": "Run tests",
          "run": "npm test"
        }
      ]
    }
  }
}
```

> La extensión de los *YAML* puede ser `.yaml` o `.yml`. En github es recomenddable usar `.yml`.

## Sintaxi

No vamos a profundizar en exceso en YAML aunque sí que hemos de saber lo básico. Si quieres profundizar un poco más o ves algo que no entiendes, puedes echarle un ojo a este [Tutorial de YAML](https://learnxinyminutes.com/docs/yaml/).

Como conceptos básicos tenemos los diccionarios y los arrays. Un diccionario es una lista de pares `llave` y `valor`. (`key`, `value`).

```yaml
key: value
another_key: "another_value"
numver: 289
boolean: true
```

Un array es una lista de valores.

```yaml
my_array:
    - element
    - 0.5
    - true
```

Obviamente podemos anidar nuestros diccionarios o arrays

```yaml
is_github_free: more_or_less
github_features:
    - gh-pages
    - gh-actions
    - gh-projects
github_options:
    free: access_to_repos
    paid: access_to_stats
    super_paid:
        - access_to_repos
        - access_to_stats
        - all_other_features
```

> Ir a **[Github Actions](github-actions.md)**