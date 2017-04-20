# npmdoc-pdfkit

#### api documentation for  [pdfkit (v0.8.0)](http://pdfkit.org/)  [![npm package](https://img.shields.io/npm/v/npmdoc-pdfkit.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-pdfkit) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-pdfkit.svg)](https://travis-ci.org/npmdoc/node-npmdoc-pdfkit)

#### A PDF generation library for Node.js

[![NPM](https://nodei.co/npm/pdfkit.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/pdfkit)

- [https://npmdoc.github.io/node-npmdoc-pdfkit/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-pdfkit/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-pdfkit/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-pdfkit/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-pdfkit/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-pdfkit/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "pdfkit",
    "description": "A PDF generation library for Node.js",
    "keywords": [
        "pdf",
        "pdf writer",
        "pdf generator",
        "graphics",
        "document",
        "vector"
    ],
    "version": "0.8.0",
    "homepage": "http://pdfkit.org/",
    "author": {
        "name": "Devon Govett",
        "url": "http://badassjs.com/"
    },
    "repository": {
        "type": "git",
        "url": "https://github.com/devongovett/pdfkit.git"
    },
    "bugs": "http://github.com/devongovett/pdfkit/issues",
    "devDependencies": {
        "blob-stream": "^0.1.2",
        "brace": "^0.2.1",
        "brfs": "~1.0.1",
        "browserify": "^3.39.0",
        "codemirror": "~3.20.0",
        "coffee-script": ">=1.0.1",
        "coffeeify": "^0.6.0",
        "exorcist": "^0.1.5",
        "iconv-lite": "^0.4.13",
        "jade": "~1.1.5",
        "markdown": "~0.5.0"
    },
    "dependencies": {
        "fontkit": "^1.0.0",
        "linebreak": "~0.1.0",
        "png-js": ">=0.1.0"
    },
    "scripts": {
        "prepublish": "make js",
        "postpublish": "make clean"
    },
    "main": "js/document",
    "browserify": {
        "transform": [
            "brfs"
        ]
    },
    "engine": [
        "node >= v0.10.0"
    ]
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
