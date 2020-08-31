# gatsby-plugin-intl

A customized gatsby-plugin-intl package with slug translation support.

## Repositories

- Original package: [wiziple/gatsby-plugin-intl](https://github.com/wiziple/gatsby-plugin-intl)
- Package with slug support: [Jno21/gatsby-plugin-intl](https://github.com/Jno21/gatsby-plugin-intl)


## Installation

1. Install the package:
    ```
    npm install --save https://github.com/bartosjiri/gatsby-plugin-intl/tarball/master
    ```
2. Add the plugin to the `gatsby-config.js` file:
    ```
    plugins: [
      {
        resolve: `gatsby-plugin-intl`,
        options: {
          path: `${__dirname}/src/intl`,
          languages: [`en`, `cs`],
          defaultLanguage: `cs`,
          redirect: true,
        },
      },
    ]
    ```
    
## Usage
1. Create a locale config file for each language (ex. `/src/intl/cs.json`) including translations for all pages:
    ```
    {
      "pages": {
        "404": "404",
        "index": "index",
        "page-2": "stranka-2"
      }
    }
    ```
2. Continue using other features from the [original package](https://github.com/wiziple/gatsby-plugin-intl).
