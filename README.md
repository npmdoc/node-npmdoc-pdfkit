# api documentation for  [pdfkit (v0.8.0)](http://pdfkit.org/)  [![npm package](https://img.shields.io/npm/v/npmdoc-pdfkit.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-pdfkit) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-pdfkit.svg)](https://travis-ci.org/npmdoc/node-npmdoc-pdfkit)
#### A PDF generation library for Node.js

[![NPM](https://nodei.co/npm/pdfkit.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/pdfkit)

[![apidoc](https://npmdoc.github.io/node-npmdoc-pdfkit/build/screenCapture.buildCi.browser.apidoc.html.png)](https://npmdoc.github.io/node-npmdoc-pdfkit/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-pdfkit/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-pdfkit/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Devon Govett",
        "url": "http://badassjs.com/"
    },
    "browserify": {
        "transform": [
            "brfs"
        ]
    },
    "bugs": {
        "url": "http://github.com/devongovett/pdfkit/issues"
    },
    "dependencies": {
        "fontkit": "^1.0.0",
        "linebreak": "~0.1.0",
        "png-js": ">=0.1.0"
    },
    "description": "A PDF generation library for Node.js",
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
    "directories": {},
    "dist": {
        "shasum": "0b3f7c0c3b00cc4f7f69e46d85d2a7cbb3818af6",
        "tarball": "https://registry.npmjs.org/pdfkit/-/pdfkit-0.8.0.tgz"
    },
    "engine": [
        "node >= v0.10.0"
    ],
    "gitHead": "08ef766c00ee6cb377322f58f5c388aae0bf36bb",
    "homepage": "http://pdfkit.org/",
    "keywords": [
        "pdf",
        "pdf writer",
        "pdf generator",
        "graphics",
        "document",
        "vector"
    ],
    "main": "js/document",
    "maintainers": [
        {
            "name": "devongovett"
        }
    ],
    "name": "pdfkit",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/devongovett/pdfkit.git"
    },
    "scripts": {
        "postpublish": "make clean",
        "prepublish": "make js"
    },
    "version": "0.8.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module pdfkit](#apidoc.module.pdfkit)
1.  [function <span class="apidocSignatureSpan"></span>pdfkit (options1)](#apidoc.element.pdfkit.pdfkit)
1.  [function <span class="apidocSignatureSpan">pdfkit.</span>ReadableState (options, stream)](#apidoc.element.pdfkit.ReadableState)
1.  [function <span class="apidocSignatureSpan">pdfkit.</span>_fromList (n, state)](#apidoc.element.pdfkit._fromList)
1.  [function <span class="apidocSignatureSpan">pdfkit.</span>super_ ()](#apidoc.element.pdfkit.super_)
1.  [function <span class="apidocSignatureSpan">pdfkit.</span>toString ()](#apidoc.element.pdfkit.toString)
1.  object <span class="apidocSignatureSpan">pdfkit.</span>__super__



# <a name="apidoc.module.pdfkit"></a>[module pdfkit](#apidoc.module.pdfkit)

#### <a name="apidoc.element.pdfkit.pdfkit"></a>[function <span class="apidocSignatureSpan"></span>pdfkit (options1)](#apidoc.element.pdfkit.pdfkit)
- description and source-code
```javascript
function PDFDocument(options1) {
  var key, ref1, ref2, val;
  this.options = options1 != null ? options1 : {};
  PDFDocument.__super__.constructor.apply(this, arguments);
  this.version = 1.3;
  this.compress = (ref1 = this.options.compress) != null ? ref1 : true;
  this._pageBuffer = [];
  this._pageBufferStart = 0;
  this._offsets = [];
  this._waiting = 0;
  this._ended = false;
  this._offset = 0;
  this._root = this.ref({
    Type: 'Catalog',
    Pages: this.ref({
      Type: 'Pages',
      Count: 0,
      Kids: []
    })
  });
  this.page = null;
  this.initColor();
  this.initVector();
  this.initFonts();
  this.initText();
  this.initImages();
  this.info = {
    Producer: 'PDFKit',
    Creator: 'PDFKit',
    CreationDate: new Date()
  };
  if (this.options.info) {
    ref2 = this.options.info;
    for (key in ref2) {
      val = ref2[key];
      this.info[key] = val;
    }
  }
  this._write("%PDF-" + this.version);
  this._write("%\xFF\xFF\xFF\xFF");
  if (this.options.autoFirstPage !== false) {
    this.addPage();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pdfkit.ReadableState"></a>[function <span class="apidocSignatureSpan">pdfkit.</span>ReadableState (options, stream)](#apidoc.element.pdfkit.ReadableState)
- description and source-code
```javascript
function ReadableState(options, stream) {
  options = options || {};

  // object stream flag. Used to make read(n) ignore n and to
  // make all the buffer merging and length checks go away
  this.objectMode = !!options.objectMode;

  if (stream instanceof Stream.Duplex)
    this.objectMode = this.objectMode || !!options.readableObjectMode;

  // the point at which it stops calling _read() to fill the buffer
  // Note: 0 is a valid value, means "don't call _read preemptively ever"
  var hwm = options.highWaterMark;
  var defaultHwm = this.objectMode ? 16 : 16 * 1024;
  this.highWaterMark = (hwm || hwm === 0) ? hwm : defaultHwm;

  // cast to ints.
  this.highWaterMark = ~~this.highWaterMark;

  // A linked list is used to store data chunks instead of an array because the
  // linked list can remove elements from the beginning faster than
  // array.shift()
  this.buffer = new BufferList();
  this.length = 0;
  this.pipes = null;
  this.pipesCount = 0;
  this.flowing = null;
  this.ended = false;
  this.endEmitted = false;
  this.reading = false;

  // a flag to be able to tell if the onwrite cb is called immediately,
  // or on a later tick.  We set this to true at first, because any
  // actions that shouldn't happen until "later" should generally also
  // not happen before the first write call.
  this.sync = true;

  // whenever we return null, then we set a flag to say
  // that we're awaiting a 'readable' event emission.
  this.needReadable = false;
  this.emittedReadable = false;
  this.readableListening = false;
  this.resumeScheduled = false;

  // Crypto is kind of old and crusty.  Historically, its default string
  // encoding is 'binary' so we have to make this configurable.
  // Everything else in the universe uses 'utf8', though.
  this.defaultEncoding = options.defaultEncoding || 'utf8';

  // when piping, we only care about 'readable' events that happen
  // after read()ing all the bytes and not getting any pushback.
  this.ranOut = false;

  // the number of writers that are awaiting a drain event in .pipe()s
  this.awaitDrain = 0;

  // if true, a maybeReadMore has been scheduled
  this.readingMore = false;

  this.decoder = null;
  this.encoding = null;
  if (options.encoding) {
    if (!StringDecoder)
      StringDecoder = require('string_decoder').StringDecoder;
    this.decoder = new StringDecoder(options.encoding);
    this.encoding = options.encoding;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pdfkit._fromList"></a>[function <span class="apidocSignatureSpan">pdfkit.</span>_fromList (n, state)](#apidoc.element.pdfkit._fromList)
- description and source-code
```javascript
function fromList(n, state) {
  // nothing buffered
  if (state.length === 0)
    return null;

  var ret;
  if (state.objectMode)
    ret = state.buffer.shift();
  else if (!n || n >= state.length) {
    // read it all, truncate the list
    if (state.decoder)
      ret = state.buffer.join('');
    else if (state.buffer.length === 1)
      ret = state.buffer.head.data;
    else
      ret = state.buffer.concat(state.length);
    state.buffer.clear();
  } else {
    // read part of list
    ret = fromListPartial(n, state.buffer, state.decoder);
  }

  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pdfkit.super_"></a>[function <span class="apidocSignatureSpan">pdfkit.</span>super_ ()](#apidoc.element.pdfkit.super_)
- description and source-code
```javascript
function Stream() {
  EE.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pdfkit.toString"></a>[function <span class="apidocSignatureSpan">pdfkit.</span>toString ()](#apidoc.element.pdfkit.toString)
- description and source-code
```javascript
toString = function () {
    return toString;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
