# api documentation for  [pdfkit (v0.8.0)](http://pdfkit.org/)  [![npm package](https://img.shields.io/npm/v/npmdoc-pdfkit.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-pdfkit) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-pdfkit.svg)](https://travis-ci.org/npmdoc/node-npmdoc-pdfkit)
#### A PDF generation library for Node.js

[![NPM](https://nodei.co/npm/pdfkit.png?downloads=true)](https://www.npmjs.com/package/pdfkit)

[![apidoc](https://npmdoc.github.io/node-npmdoc-pdfkit/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-pdfkit_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-pdfkit/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-pdfkit/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Devon Govett",
        "email": "devongovett@gmail.com",
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
            "name": "devongovett",
            "email": "devongovett@gmail.com"
        }
    ],
    "name": "pdfkit",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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
1.  [function <span class="apidocSignatureSpan">pdfkit.</span>ReadableState (options, stream)](#apidoc.element.pdfkit.ReadableState)
1.  [function <span class="apidocSignatureSpan">pdfkit.</span>_fromList (n, state)](#apidoc.element.pdfkit._fromList)
1.  [function <span class="apidocSignatureSpan">pdfkit.</span>data (data)](#apidoc.element.pdfkit.data)
1.  [function <span class="apidocSignatureSpan">pdfkit.</span>font ()](#apidoc.element.pdfkit.font)
1.  [function <span class="apidocSignatureSpan">pdfkit.</span>image ()](#apidoc.element.pdfkit.image)
1.  [function <span class="apidocSignatureSpan">pdfkit.</span>line_wrapper (document, options)](#apidoc.element.pdfkit.line_wrapper)
1.  [function <span class="apidocSignatureSpan">pdfkit.</span>object ()](#apidoc.element.pdfkit.object)
1.  [function <span class="apidocSignatureSpan">pdfkit.</span>page (document, options)](#apidoc.element.pdfkit.page)
1.  [function <span class="apidocSignatureSpan">pdfkit.</span>path ()](#apidoc.element.pdfkit.path)
1.  [function <span class="apidocSignatureSpan">pdfkit.</span>reference (document, id, data)](#apidoc.element.pdfkit.reference)
1.  [function <span class="apidocSignatureSpan">pdfkit.</span>super_ ()](#apidoc.element.pdfkit.super_)
1.  object <span class="apidocSignatureSpan">pdfkit.</span>__super__
1.  object <span class="apidocSignatureSpan">pdfkit.</span>data.prototype
1.  object <span class="apidocSignatureSpan">pdfkit.</span>font.prototype
1.  object <span class="apidocSignatureSpan">pdfkit.</span>gradient
1.  object <span class="apidocSignatureSpan">pdfkit.</span>line_wrapper.prototype
1.  object <span class="apidocSignatureSpan">pdfkit.</span>page.prototype
1.  object <span class="apidocSignatureSpan">pdfkit.</span>reference.prototype

#### [module pdfkit.data](#apidoc.module.pdfkit.data)
1.  [function <span class="apidocSignatureSpan">pdfkit.</span>data (data)](#apidoc.element.pdfkit.data.data)

#### [module pdfkit.data.prototype](#apidoc.module.pdfkit.data.prototype)
1.  [function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>byteAt (index)](#apidoc.element.pdfkit.data.prototype.byteAt)
1.  [function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>read (bytes)](#apidoc.element.pdfkit.data.prototype.read)
1.  [function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>readBool ()](#apidoc.element.pdfkit.data.prototype.readBool)
1.  [function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>readByte ()](#apidoc.element.pdfkit.data.prototype.readByte)
1.  [function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>readInt ()](#apidoc.element.pdfkit.data.prototype.readInt)
1.  [function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>readInt16 ()](#apidoc.element.pdfkit.data.prototype.readInt16)
1.  [function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>readInt32 ()](#apidoc.element.pdfkit.data.prototype.readInt32)
1.  [function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>readLongLong ()](#apidoc.element.pdfkit.data.prototype.readLongLong)
1.  [function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>readShort ()](#apidoc.element.pdfkit.data.prototype.readShort)
1.  [function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>readString (length)](#apidoc.element.pdfkit.data.prototype.readString)
1.  [function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>readUInt16 ()](#apidoc.element.pdfkit.data.prototype.readUInt16)
1.  [function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>readUInt32 ()](#apidoc.element.pdfkit.data.prototype.readUInt32)
1.  [function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>slice (start, end)](#apidoc.element.pdfkit.data.prototype.slice)
1.  [function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>stringAt (pos, length)](#apidoc.element.pdfkit.data.prototype.stringAt)
1.  [function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>write (bytes)](#apidoc.element.pdfkit.data.prototype.write)
1.  [function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>writeBool (val)](#apidoc.element.pdfkit.data.prototype.writeBool)
1.  [function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>writeByte (byte)](#apidoc.element.pdfkit.data.prototype.writeByte)
1.  [function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>writeInt (val)](#apidoc.element.pdfkit.data.prototype.writeInt)
1.  [function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>writeInt16 (val)](#apidoc.element.pdfkit.data.prototype.writeInt16)
1.  [function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>writeInt32 (val)](#apidoc.element.pdfkit.data.prototype.writeInt32)
1.  [function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>writeLongLong (val)](#apidoc.element.pdfkit.data.prototype.writeLongLong)
1.  [function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>writeShort (val)](#apidoc.element.pdfkit.data.prototype.writeShort)
1.  [function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>writeString (val)](#apidoc.element.pdfkit.data.prototype.writeString)
1.  [function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>writeUInt16 (val)](#apidoc.element.pdfkit.data.prototype.writeUInt16)
1.  [function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>writeUInt32 (val)](#apidoc.element.pdfkit.data.prototype.writeUInt32)

#### [module pdfkit.font](#apidoc.module.pdfkit.font)
1.  [function <span class="apidocSignatureSpan">pdfkit.</span>font ()](#apidoc.element.pdfkit.font.font)
1.  [function <span class="apidocSignatureSpan">pdfkit.font.</span>open (document, src, family, id)](#apidoc.element.pdfkit.font.open)

#### [module pdfkit.font.prototype](#apidoc.module.pdfkit.font.prototype)
1.  [function <span class="apidocSignatureSpan">pdfkit.font.prototype.</span>embed ()](#apidoc.element.pdfkit.font.prototype.embed)
1.  [function <span class="apidocSignatureSpan">pdfkit.font.prototype.</span>encode (text)](#apidoc.element.pdfkit.font.prototype.encode)
1.  [function <span class="apidocSignatureSpan">pdfkit.font.prototype.</span>finalize ()](#apidoc.element.pdfkit.font.prototype.finalize)
1.  [function <span class="apidocSignatureSpan">pdfkit.font.prototype.</span>lineHeight (size, includeGap)](#apidoc.element.pdfkit.font.prototype.lineHeight)
1.  [function <span class="apidocSignatureSpan">pdfkit.font.prototype.</span>ref ()](#apidoc.element.pdfkit.font.prototype.ref)
1.  [function <span class="apidocSignatureSpan">pdfkit.font.prototype.</span>widthOfString (text)](#apidoc.element.pdfkit.font.prototype.widthOfString)

#### [module pdfkit.gradient](#apidoc.module.pdfkit.gradient)
1.  [function <span class="apidocSignatureSpan">pdfkit.gradient.</span>PDFGradient (doc)](#apidoc.element.pdfkit.gradient.PDFGradient)
1.  [function <span class="apidocSignatureSpan">pdfkit.gradient.</span>PDFLinearGradient (doc, x1, y1, x2, y2)](#apidoc.element.pdfkit.gradient.PDFLinearGradient)
1.  [function <span class="apidocSignatureSpan">pdfkit.gradient.</span>PDFRadialGradient (doc, x1, y1, r1, x2, y2, r2)](#apidoc.element.pdfkit.gradient.PDFRadialGradient)

#### [module pdfkit.image](#apidoc.module.pdfkit.image)
1.  [function <span class="apidocSignatureSpan">pdfkit.</span>image ()](#apidoc.element.pdfkit.image.image)
1.  [function <span class="apidocSignatureSpan">pdfkit.image.</span>open (src, label)](#apidoc.element.pdfkit.image.open)

#### [module pdfkit.line_wrapper](#apidoc.module.pdfkit.line_wrapper)
1.  boolean <span class="apidocSignatureSpan">pdfkit.line_wrapper.</span>usingDomains
1.  [function <span class="apidocSignatureSpan">pdfkit.</span>line_wrapper (document, options)](#apidoc.element.pdfkit.line_wrapper.line_wrapper)
1.  [function <span class="apidocSignatureSpan">pdfkit.line_wrapper.</span>EventEmitter ()](#apidoc.element.pdfkit.line_wrapper.EventEmitter)
1.  [function <span class="apidocSignatureSpan">pdfkit.line_wrapper.</span>init ()](#apidoc.element.pdfkit.line_wrapper.init)
1.  [function <span class="apidocSignatureSpan">pdfkit.line_wrapper.</span>listenerCount (emitter, type)](#apidoc.element.pdfkit.line_wrapper.listenerCount)
1.  number <span class="apidocSignatureSpan">pdfkit.line_wrapper.</span>defaultMaxListeners
1.  object <span class="apidocSignatureSpan">pdfkit.line_wrapper.</span>__super__

#### [module pdfkit.line_wrapper.prototype](#apidoc.module.pdfkit.line_wrapper.prototype)
1.  [function <span class="apidocSignatureSpan">pdfkit.line_wrapper.prototype.</span>constructor (document, options)](#apidoc.element.pdfkit.line_wrapper.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">pdfkit.line_wrapper.prototype.</span>eachWord (text, fn)](#apidoc.element.pdfkit.line_wrapper.prototype.eachWord)
1.  [function <span class="apidocSignatureSpan">pdfkit.line_wrapper.prototype.</span>nextSection (options)](#apidoc.element.pdfkit.line_wrapper.prototype.nextSection)
1.  [function <span class="apidocSignatureSpan">pdfkit.line_wrapper.prototype.</span>wordWidth (word)](#apidoc.element.pdfkit.line_wrapper.prototype.wordWidth)
1.  [function <span class="apidocSignatureSpan">pdfkit.line_wrapper.prototype.</span>wrap (text, options)](#apidoc.element.pdfkit.line_wrapper.prototype.wrap)

#### [module pdfkit.object](#apidoc.module.pdfkit.object)
1.  [function <span class="apidocSignatureSpan">pdfkit.</span>object ()](#apidoc.element.pdfkit.object.object)
1.  [function <span class="apidocSignatureSpan">pdfkit.object.</span>convert (object)](#apidoc.element.pdfkit.object.convert)

#### [module pdfkit.page](#apidoc.module.pdfkit.page)
1.  [function <span class="apidocSignatureSpan">pdfkit.</span>page (document, options)](#apidoc.element.pdfkit.page.page)

#### [module pdfkit.page.prototype](#apidoc.module.pdfkit.page.prototype)
1.  [function <span class="apidocSignatureSpan">pdfkit.page.prototype.</span>end ()](#apidoc.element.pdfkit.page.prototype.end)
1.  [function <span class="apidocSignatureSpan">pdfkit.page.prototype.</span>maxY ()](#apidoc.element.pdfkit.page.prototype.maxY)
1.  [function <span class="apidocSignatureSpan">pdfkit.page.prototype.</span>write (chunk)](#apidoc.element.pdfkit.page.prototype.write)

#### [module pdfkit.path](#apidoc.module.pdfkit.path)
1.  [function <span class="apidocSignatureSpan">pdfkit.</span>path ()](#apidoc.element.pdfkit.path.path)
1.  [function <span class="apidocSignatureSpan">pdfkit.path.</span>apply (doc, path)](#apidoc.element.pdfkit.path.apply)

#### [module pdfkit.reference](#apidoc.module.pdfkit.reference)
1.  [function <span class="apidocSignatureSpan">pdfkit.</span>reference (document, id, data)](#apidoc.element.pdfkit.reference.reference)
1.  [function <span class="apidocSignatureSpan">pdfkit.reference.</span>WritableState (options, stream)](#apidoc.element.pdfkit.reference.WritableState)
1.  [function <span class="apidocSignatureSpan">pdfkit.reference.</span>super_ ()](#apidoc.element.pdfkit.reference.super_)
1.  object <span class="apidocSignatureSpan">pdfkit.reference.</span>__super__

#### [module pdfkit.reference.prototype](#apidoc.module.pdfkit.reference.prototype)
1.  [function <span class="apidocSignatureSpan">pdfkit.reference.prototype.</span>_write (chunk, encoding, callback)](#apidoc.element.pdfkit.reference.prototype._write)
1.  [function <span class="apidocSignatureSpan">pdfkit.reference.prototype.</span>constructor (document, id, data)](#apidoc.element.pdfkit.reference.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">pdfkit.reference.prototype.</span>end (chunk)](#apidoc.element.pdfkit.reference.prototype.end)
1.  [function <span class="apidocSignatureSpan">pdfkit.reference.prototype.</span>finalize ()](#apidoc.element.pdfkit.reference.prototype.finalize)
1.  [function <span class="apidocSignatureSpan">pdfkit.reference.prototype.</span>initDeflate ()](#apidoc.element.pdfkit.reference.prototype.initDeflate)
1.  [function <span class="apidocSignatureSpan">pdfkit.reference.prototype.</span>toString ()](#apidoc.element.pdfkit.reference.prototype.toString)



# <a name="apidoc.module.pdfkit"></a>[module pdfkit](#apidoc.module.pdfkit)

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

#### <a name="apidoc.element.pdfkit.data"></a>[function <span class="apidocSignatureSpan">pdfkit.</span>data (data)](#apidoc.element.pdfkit.data)
- description and source-code
```javascript
function Data(data) {
  this.data = data != null ? data : [];
  this.pos = 0;
  this.length = this.data.length;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pdfkit.font"></a>[function <span class="apidocSignatureSpan">pdfkit.</span>font ()](#apidoc.element.pdfkit.font)
- description and source-code
```javascript
function PDFFont() {
  throw new Error('Cannot construct a PDFFont directly.');
}
```
- example usage
```shell
...
doc = new PDFDocument

# Pipe its output somewhere, like to a file or HTTP response
# See below for browser usage
doc.pipe fs.createWriteStream('output.pdf')

# Embed a font, set the font size, and render some text
doc.font('fonts/PalatinoBold.ttf')
.fontSize(25)
.text('Some text with an embedded font!', 100, 100)

# Add another page
doc.addPage()
.fontSize(25)
.text('Here is some vector graphics...', 100, 100)
...
```

#### <a name="apidoc.element.pdfkit.image"></a>[function <span class="apidocSignatureSpan">pdfkit.</span>image ()](#apidoc.element.pdfkit.image)
- description and source-code
```javascript
function PDFImage() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pdfkit.line_wrapper"></a>[function <span class="apidocSignatureSpan">pdfkit.</span>line_wrapper (document, options)](#apidoc.element.pdfkit.line_wrapper)
- description and source-code
```javascript
function LineWrapper(document, options) {
  var ref;
  this.document = document;
  this.indent = options.indent || 0;
  this.characterSpacing = options.characterSpacing || 0;
  this.wordSpacing = options.wordSpacing === 0;
  this.columns = options.columns || 1;
  this.columnGap = (ref = options.columnGap) != null ? ref : 18;
  this.lineWidth = (options.width - (this.columnGap * (this.columns - 1))) / this.columns;
  this.spaceLeft = this.lineWidth;
  this.startX = this.document.x;
  this.startY = this.document.y;
  this.column = 1;
  this.ellipsis = options.ellipsis;
  this.continuedX = 0;
  this.features = options.features;
  if (options.height != null) {
    this.height = options.height;
    this.maxY = this.startY + options.height;
  } else {
    this.maxY = this.document.page.maxY();
  }
  this.on('firstLine', (function(_this) {
    return function(options) {
      var indent;
      indent = _this.continuedX || _this.indent;
      _this.document.x += indent;
      _this.lineWidth -= indent;
      return _this.once('line', function() {
        _this.document.x -= indent;
        _this.lineWidth += indent;
        if (options.continued && !_this.continuedX) {
          _this.continuedX = _this.indent;
        }
        if (!options.continued) {
          return _this.continuedX = 0;
        }
      });
    };
  })(this));
  this.on('lastLine', (function(_this) {
    return function(options) {
      var align;
      align = options.align;
      if (align === 'justify') {
        options.align = 'left';
      }
      _this.lastLine = true;
      return _this.once('line', function() {
        _this.document.y += options.paragraphGap || 0;
        options.align = align;
        return _this.lastLine = false;
      });
    };
  })(this));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pdfkit.object"></a>[function <span class="apidocSignatureSpan">pdfkit.</span>object ()](#apidoc.element.pdfkit.object)
- description and source-code
```javascript
function PDFObject() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pdfkit.page"></a>[function <span class="apidocSignatureSpan">pdfkit.</span>page (document, options)](#apidoc.element.pdfkit.page)
- description and source-code
```javascript
function PDFPage(document, options) {
  var dimensions;
  this.document = document;
  if (options == null) {
    options = {};
  }
  this.size = options.size || 'letter';
  this.layout = options.layout || 'portrait';
  if (typeof options.margin === 'number') {
    this.margins = {
      top: options.margin,
      left: options.margin,
      bottom: options.margin,
      right: options.margin
    };
  } else {
    this.margins = options.margins || DEFAULT_MARGINS;
  }
  dimensions = Array.isArray(this.size) ? this.size : SIZES[this.size.toUpperCase()];
  this.width = dimensions[this.layout === 'portrait' ? 0 : 1];
  this.height = dimensions[this.layout === 'portrait' ? 1 : 0];
  this.content = this.document.ref();
  this.resources = this.document.ref({
    ProcSet: ['PDF', 'Text', 'ImageB', 'ImageC', 'ImageI']
  });
  Object.defineProperties(this, {
    fonts: {
      get: (function(_this) {
        return function() {
          var base;
          return (base = _this.resources.data).Font != null ? base.Font : base.Font = {};
        };
      })(this)
    },
    xobjects: {
      get: (function(_this) {
        return function() {
          var base;
          return (base = _this.resources.data).XObject != null ? base.XObject : base.XObject = {};
        };
      })(this)
    },
    ext_gstates: {
      get: (function(_this) {
        return function() {
          var base;
          return (base = _this.resources.data).ExtGState != null ? base.ExtGState : base.ExtGState = {};
        };
      })(this)
    },
    patterns: {
      get: (function(_this) {
        return function() {
          var base;
          return (base = _this.resources.data).Pattern != null ? base.Pattern : base.Pattern = {};
        };
      })(this)
    },
    annotations: {
      get: (function(_this) {
        return function() {
          var base;
          return (base = _this.dictionary.data).Annots != null ? base.Annots : base.Annots = [];
        };
      })(this)
    }
  });
  this.dictionary = this.document.ref({
    Type: 'Page',
    Parent: this.document._root.data.Pages,
    MediaBox: [0, 0, this.width, this.height],
    Contents: this.content,
    Resources: this.resources
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pdfkit.path"></a>[function <span class="apidocSignatureSpan">pdfkit.</span>path ()](#apidoc.element.pdfkit.path)
- description and source-code
```javascript
function SVGPath() {}
```
- example usage
```shell
...
.lineTo(100, 250)
.lineTo(200, 250)
.fill("#FF3300")

# Apply some transforms and render an SVG path with the 'even-odd' fill rule
doc.scale(0.6)
.translate(470, -380)
.path('M 250,75 L 323,301 131,161 369,161 177,301 z')
.fill('red', 'even-odd')
.restore()

# Add some text with annotations
doc.addPage()
.fillColor("blue")
.text('Here is a link!', 100, 100)
...
```

#### <a name="apidoc.element.pdfkit.reference"></a>[function <span class="apidocSignatureSpan">pdfkit.</span>reference (document, id, data)](#apidoc.element.pdfkit.reference)
- description and source-code
```javascript
function PDFReference(document, id, data) {
  this.document = document;
  this.id = id;
  this.data = data != null ? data : {};
  this.finalize = bind(this.finalize, this);
  PDFReference.__super__.constructor.call(this, {
    decodeStrings: false
  });
  this.gen = 0;
  this.deflate = null;
  this.compress = this.document.compress && !this.data.Filter;
  this.uncompressedLength = 0;
  this.chunks = [];
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



# <a name="apidoc.module.pdfkit.data"></a>[module pdfkit.data](#apidoc.module.pdfkit.data)

#### <a name="apidoc.element.pdfkit.data.data"></a>[function <span class="apidocSignatureSpan">pdfkit.</span>data (data)](#apidoc.element.pdfkit.data.data)
- description and source-code
```javascript
function Data(data) {
  this.data = data != null ? data : [];
  this.pos = 0;
  this.length = this.data.length;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.pdfkit.data.prototype"></a>[module pdfkit.data.prototype](#apidoc.module.pdfkit.data.prototype)

#### <a name="apidoc.element.pdfkit.data.prototype.byteAt"></a>[function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>byteAt (index)](#apidoc.element.pdfkit.data.prototype.byteAt)
- description and source-code
```javascript
byteAt = function (index) {
  return this.data[index];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pdfkit.data.prototype.read"></a>[function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>read (bytes)](#apidoc.element.pdfkit.data.prototype.read)
- description and source-code
```javascript
read = function (bytes) {
  var buf, i, j, ref;
  buf = [];
  for (i = j = 0, ref = bytes; 0 <= ref ? j < ref : j > ref; i = 0 <= ref ? ++j : --j) {
    buf.push(this.readByte());
  }
  return buf;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pdfkit.data.prototype.readBool"></a>[function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>readBool ()](#apidoc.element.pdfkit.data.prototype.readBool)
- description and source-code
```javascript
readBool = function () {
  return !!this.readByte();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pdfkit.data.prototype.readByte"></a>[function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>readByte ()](#apidoc.element.pdfkit.data.prototype.readByte)
- description and source-code
```javascript
readByte = function () {
  return this.data[this.pos++];
}
```
- example usage
```shell
...
};

Data.prototype.byteAt = function(index) {
  return this.data[index];
};

Data.prototype.readBool = function() {
  return !!this.readByte();
};

Data.prototype.writeBool = function(val) {
  return this.writeByte(val ? 1 : 0);
};

Data.prototype.readUInt32 = function() {
...
```

#### <a name="apidoc.element.pdfkit.data.prototype.readInt"></a>[function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>readInt ()](#apidoc.element.pdfkit.data.prototype.readInt)
- description and source-code
```javascript
readInt = function () {
  return this.readInt32();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pdfkit.data.prototype.readInt16"></a>[function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>readInt16 ()](#apidoc.element.pdfkit.data.prototype.readInt16)
- description and source-code
```javascript
readInt16 = function () {
  var int;
  int = this.readUInt16();
  if (int >= 0x8000) {
    return int - 0x10000;
  } else {
    return int;
  }
}
```
- example usage
```shell
...

Data.prototype.stringAt = function(pos, length) {
  this.pos = pos;
  return this.readString(length);
};

Data.prototype.readShort = function() {
  return this.readInt16();
};

Data.prototype.writeShort = function(val) {
  return this.writeInt16(val);
};

Data.prototype.readLongLong = function() {
...
```

#### <a name="apidoc.element.pdfkit.data.prototype.readInt32"></a>[function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>readInt32 ()](#apidoc.element.pdfkit.data.prototype.readInt32)
- description and source-code
```javascript
readInt32 = function () {
  var int;
  int = this.readUInt32();
  if (int >= 0x80000000) {
    return int - 0x100000000;
  } else {
    return int;
  }
}
```
- example usage
```shell
...
  this.writeByte((low >> 24) & 0xff);
  this.writeByte((low >> 16) & 0xff);
  this.writeByte((low >> 8) & 0xff);
  return this.writeByte(low & 0xff);
};

Data.prototype.readInt = function() {
  return this.readInt32();
};

Data.prototype.writeInt = function(val) {
  return this.writeInt32(val);
};

Data.prototype.slice = function(start, end) {
...
```

#### <a name="apidoc.element.pdfkit.data.prototype.readLongLong"></a>[function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>readLongLong ()](#apidoc.element.pdfkit.data.prototype.readLongLong)
- description and source-code
```javascript
readLongLong = function () {
  var b1, b2, b3, b4, b5, b6, b7, b8;
  b1 = this.readByte();
  b2 = this.readByte();
  b3 = this.readByte();
  b4 = this.readByte();
  b5 = this.readByte();
  b6 = this.readByte();
  b7 = this.readByte();
  b8 = this.readByte();
  if (b1 & 0x80) {
    return ((b1 ^ 0xff) * 0x100000000000000 + (b2 ^ 0xff) * 0x1000000000000 + (b3 ^ 0xff) * 0x10000000000 + (b4 ^ 0xff) * 0x100000000
 + (b5 ^ 0xff) * 0x1000000 + (b6 ^ 0xff) * 0x10000 + (b7 ^ 0xff) * 0x100 + (b8 ^ 0xff) + 1) * -1;
  }
  return b1 * 0x100000000000000 + b2 * 0x1000000000000 + b3 * 0x10000000000 + b4 * 0x100000000 + b5 * 0x1000000 + b6 * 0x10000 +
b7 * 0x100 + b8;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pdfkit.data.prototype.readShort"></a>[function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>readShort ()](#apidoc.element.pdfkit.data.prototype.readShort)
- description and source-code
```javascript
readShort = function () {
  return this.readInt16();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pdfkit.data.prototype.readString"></a>[function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>readString (length)](#apidoc.element.pdfkit.data.prototype.readString)
- description and source-code
```javascript
readString = function (length) {
  var i, j, ref, ret;
  ret = [];
  for (i = j = 0, ref = length; 0 <= ref ? j < ref : j > ref; i = 0 <= ref ? ++j : --j) {
    ret[i] = String.fromCharCode(this.readByte());
  }
  return ret.join('');
}
```
- example usage
```shell
...
    results.push(this.writeByte(val.charCodeAt(i)));
  }
  return results;
};

Data.prototype.stringAt = function(pos, length) {
  this.pos = pos;
  return this.readString(length);
};

Data.prototype.readShort = function() {
  return this.readInt16();
};

Data.prototype.writeShort = function(val) {
...
```

#### <a name="apidoc.element.pdfkit.data.prototype.readUInt16"></a>[function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>readUInt16 ()](#apidoc.element.pdfkit.data.prototype.readUInt16)
- description and source-code
```javascript
readUInt16 = function () {
  var b1, b2;
  b1 = this.readByte() << 8;
  b2 = this.readByte();
  return b1 | b2;
}
```
- example usage
```shell
...
Data.prototype.writeUInt16 = function(val) {
  this.writeByte((val >> 8) & 0xff);
  return this.writeByte(val & 0xff);
};

Data.prototype.readInt16 = function() {
  var int;
  int = this.readUInt16();
  if (int >= 0x8000) {
    return int - 0x10000;
  } else {
    return int;
  }
};
...
```

#### <a name="apidoc.element.pdfkit.data.prototype.readUInt32"></a>[function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>readUInt32 ()](#apidoc.element.pdfkit.data.prototype.readUInt32)
- description and source-code
```javascript
readUInt32 = function () {
  var b1, b2, b3, b4;
  b1 = this.readByte() * 0x1000000;
  b2 = this.readByte() << 16;
  b3 = this.readByte() << 8;
  b4 = this.readByte();
  return b1 + b2 + b3 + b4;
}
```
- example usage
```shell
...
  this.writeByte((val >> 16) & 0xff);
  this.writeByte((val >> 8) & 0xff);
  return this.writeByte(val & 0xff);
};

Data.prototype.readInt32 = function() {
  var int;
  int = this.readUInt32();
  if (int >= 0x80000000) {
    return int - 0x100000000;
  } else {
    return int;
  }
};
...
```

#### <a name="apidoc.element.pdfkit.data.prototype.slice"></a>[function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>slice (start, end)](#apidoc.element.pdfkit.data.prototype.slice)
- description and source-code
```javascript
slice = function (start, end) {
  return this.data.slice(start, end);
}
```
- example usage
```shell
...
};

Data.prototype.writeInt = function(val) {
  return this.writeInt32(val);
};

Data.prototype.slice = function(start, end) {
  return this.data.slice(start, end);
};

Data.prototype.read = function(bytes) {
  var buf, i, j, ref;
  buf = [];
  for (i = j = 0, ref = bytes; 0 <= ref ? j < ref : j > ref; i = 0 <= ref ? ++j : --j) {
    buf.push(this.readByte());
...
```

#### <a name="apidoc.element.pdfkit.data.prototype.stringAt"></a>[function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>stringAt (pos, length)](#apidoc.element.pdfkit.data.prototype.stringAt)
- description and source-code
```javascript
stringAt = function (pos, length) {
  this.pos = pos;
  return this.readString(length);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pdfkit.data.prototype.write"></a>[function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>write (bytes)](#apidoc.element.pdfkit.data.prototype.write)
- description and source-code
```javascript
write = function (bytes) {
  var byte, j, len, results;
  results = [];
  for (j = 0, len = bytes.length; j < len; j++) {
    byte = bytes[j];
    results.push(this.writeByte(byte));
  }
  return results;
}
```
- example usage
```shell
...
}

PDFPage.prototype.maxY = function() {
  return this.height - this.margins.bottom;
};

PDFPage.prototype.write = function(chunk) {
  return this.content.write(chunk);
};

PDFPage.prototype.end = function() {
  this.dictionary.end();
  this.resources.end();
  return this.content.end();
};
...
```

#### <a name="apidoc.element.pdfkit.data.prototype.writeBool"></a>[function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>writeBool (val)](#apidoc.element.pdfkit.data.prototype.writeBool)
- description and source-code
```javascript
writeBool = function (val) {
  return this.writeByte(val ? 1 : 0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pdfkit.data.prototype.writeByte"></a>[function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>writeByte (byte)](#apidoc.element.pdfkit.data.prototype.writeByte)
- description and source-code
```javascript
writeByte = function (byte) {
  return this.data[this.pos++] = byte;
}
```
- example usage
```shell
...
};

Data.prototype.readBool = function() {
  return !!this.readByte();
};

Data.prototype.writeBool = function(val) {
  return this.writeByte(val ? 1 : 0);
};

Data.prototype.readUInt32 = function() {
  var b1, b2, b3, b4;
  b1 = this.readByte() * 0x1000000;
  b2 = this.readByte() << 16;
  b3 = this.readByte() << 8;
...
```

#### <a name="apidoc.element.pdfkit.data.prototype.writeInt"></a>[function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>writeInt (val)](#apidoc.element.pdfkit.data.prototype.writeInt)
- description and source-code
```javascript
writeInt = function (val) {
  return this.writeInt32(val);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pdfkit.data.prototype.writeInt16"></a>[function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>writeInt16 (val)](#apidoc.element.pdfkit.data.prototype.writeInt16)
- description and source-code
```javascript
writeInt16 = function (val) {
  if (val < 0) {
    val += 0x10000;
  }
  return this.writeUInt16(val);
}
```
- example usage
```shell
...
};

Data.prototype.readShort = function() {
  return this.readInt16();
};

Data.prototype.writeShort = function(val) {
  return this.writeInt16(val);
};

Data.prototype.readLongLong = function() {
  var b1, b2, b3, b4, b5, b6, b7, b8;
  b1 = this.readByte();
  b2 = this.readByte();
  b3 = this.readByte();
...
```

#### <a name="apidoc.element.pdfkit.data.prototype.writeInt32"></a>[function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>writeInt32 (val)](#apidoc.element.pdfkit.data.prototype.writeInt32)
- description and source-code
```javascript
writeInt32 = function (val) {
  if (val < 0) {
    val += 0x100000000;
  }
  return this.writeUInt32(val);
}
```
- example usage
```shell
...
};

Data.prototype.readInt = function() {
  return this.readInt32();
};

Data.prototype.writeInt = function(val) {
  return this.writeInt32(val);
};

Data.prototype.slice = function(start, end) {
  return this.data.slice(start, end);
};

Data.prototype.read = function(bytes) {
...
```

#### <a name="apidoc.element.pdfkit.data.prototype.writeLongLong"></a>[function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>writeLongLong (val)](#apidoc.element.pdfkit.data.prototype.writeLongLong)
- description and source-code
```javascript
writeLongLong = function (val) {
  var high, low;
  high = Math.floor(val / 0x100000000);
  low = val & 0xffffffff;
  this.writeByte((high >> 24) & 0xff);
  this.writeByte((high >> 16) & 0xff);
  this.writeByte((high >> 8) & 0xff);
  this.writeByte(high & 0xff);
  this.writeByte((low >> 24) & 0xff);
  this.writeByte((low >> 16) & 0xff);
  this.writeByte((low >> 8) & 0xff);
  return this.writeByte(low & 0xff);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pdfkit.data.prototype.writeShort"></a>[function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>writeShort (val)](#apidoc.element.pdfkit.data.prototype.writeShort)
- description and source-code
```javascript
writeShort = function (val) {
  return this.writeInt16(val);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pdfkit.data.prototype.writeString"></a>[function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>writeString (val)](#apidoc.element.pdfkit.data.prototype.writeString)
- description and source-code
```javascript
writeString = function (val) {
  var i, j, ref, results;
  results = [];
  for (i = j = 0, ref = val.length; 0 <= ref ? j < ref : j > ref; i = 0 <= ref ? ++j : --j) {
    results.push(this.writeByte(val.charCodeAt(i)));
  }
  return results;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pdfkit.data.prototype.writeUInt16"></a>[function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>writeUInt16 (val)](#apidoc.element.pdfkit.data.prototype.writeUInt16)
- description and source-code
```javascript
writeUInt16 = function (val) {
  this.writeByte((val >> 8) & 0xff);
  return this.writeByte(val & 0xff);
}
```
- example usage
```shell
...
  }
};

Data.prototype.writeInt16 = function(val) {
  if (val < 0) {
    val += 0x10000;
  }
  return this.writeUInt16(val);
};

Data.prototype.readString = function(length) {
  var i, j, ref, ret;
  ret = [];
  for (i = j = 0, ref = length; 0 <= ref ? j < ref : j > ref; i = 0 <= ref ? ++j : --j) {
    ret[i] = String.fromCharCode(this.readByte());
...
```

#### <a name="apidoc.element.pdfkit.data.prototype.writeUInt32"></a>[function <span class="apidocSignatureSpan">pdfkit.data.prototype.</span>writeUInt32 (val)](#apidoc.element.pdfkit.data.prototype.writeUInt32)
- description and source-code
```javascript
writeUInt32 = function (val) {
  this.writeByte((val >>> 24) & 0xff);
  this.writeByte((val >> 16) & 0xff);
  this.writeByte((val >> 8) & 0xff);
  return this.writeByte(val & 0xff);
}
```
- example usage
```shell
...
  }
};

Data.prototype.writeInt32 = function(val) {
  if (val < 0) {
    val += 0x100000000;
  }
  return this.writeUInt32(val);
};

Data.prototype.readUInt16 = function() {
  var b1, b2;
  b1 = this.readByte() << 8;
  b2 = this.readByte();
  return b1 | b2;
...
```



# <a name="apidoc.module.pdfkit.font"></a>[module pdfkit.font](#apidoc.module.pdfkit.font)

#### <a name="apidoc.element.pdfkit.font.font"></a>[function <span class="apidocSignatureSpan">pdfkit.</span>font ()](#apidoc.element.pdfkit.font.font)
- description and source-code
```javascript
function PDFFont() {
  throw new Error('Cannot construct a PDFFont directly.');
}
```
- example usage
```shell
...
doc = new PDFDocument

# Pipe its output somewhere, like to a file or HTTP response
# See below for browser usage
doc.pipe fs.createWriteStream('output.pdf')

# Embed a font, set the font size, and render some text
doc.font('fonts/PalatinoBold.ttf')
.fontSize(25)
.text('Some text with an embedded font!', 100, 100)

# Add another page
doc.addPage()
.fontSize(25)
.text('Here is some vector graphics...', 100, 100)
...
```

#### <a name="apidoc.element.pdfkit.font.open"></a>[function <span class="apidocSignatureSpan">pdfkit.font.</span>open (document, src, family, id)](#apidoc.element.pdfkit.font.open)
- description and source-code
```javascript
open = function (document, src, family, id) {
  var font;
  if (typeof src === 'string') {
    if (StandardFont.isStandardFont(src)) {
      return new StandardFont(document, src, id);
    }
    font = fontkit.openSync(src, family);
  } else if (Buffer.isBuffer(src)) {
    font = fontkit.create(src, family);
  } else if (src instanceof Uint8Array) {
    font = fontkit.create(new Buffer(src), family);
  } else if (src instanceof ArrayBuffer) {
    font = fontkit.create(new Buffer(new Uint8Array(src)), family);
  }
  if (font == null) {
    throw new Error('Not a supported font format or standard PDF font.');
  }
  return new EmbeddedFont(document, font, id);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.pdfkit.font.prototype"></a>[module pdfkit.font.prototype](#apidoc.module.pdfkit.font.prototype)

#### <a name="apidoc.element.pdfkit.font.prototype.embed"></a>[function <span class="apidocSignatureSpan">pdfkit.font.prototype.</span>embed ()](#apidoc.element.pdfkit.font.prototype.embed)
- description and source-code
```javascript
embed = function () {
  throw new Error('Must be implemented by subclasses');
}
```
- example usage
```shell
...
  return this.dictionary != null ? this.dictionary : this.dictionary = this.document.ref();
};

PDFFont.prototype.finalize = function() {
  if (this.embedded || (this.dictionary == null)) {
    return;
  }
  this.embed();
  return this.embedded = true;
};

PDFFont.prototype.embed = function() {
  throw new Error('Must be implemented by subclasses');
};
...
```

#### <a name="apidoc.element.pdfkit.font.prototype.encode"></a>[function <span class="apidocSignatureSpan">pdfkit.font.prototype.</span>encode (text)](#apidoc.element.pdfkit.font.prototype.encode)
- description and source-code
```javascript
encode = function (text) {
  throw new Error('Must be implemented by subclasses');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pdfkit.font.prototype.finalize"></a>[function <span class="apidocSignatureSpan">pdfkit.font.prototype.</span>finalize ()](#apidoc.element.pdfkit.font.prototype.finalize)
- description and source-code
```javascript
finalize = function () {
  if (this.embedded || (this.dictionary == null)) {
    return;
  }
  this.embed();
  return this.embedded = true;
}
```
- example usage
```shell
...
};

PDFReference.prototype.end = function(chunk) {
  PDFReference.__super__.end.apply(this, arguments);
  if (this.deflate) {
    return this.deflate.end();
  } else {
    return this.finalize();
  }
};

PDFReference.prototype.finalize = function() {
  var chunk, i, len, ref;
  this.offset = this.document._offset;
  this.document._write(this.id + " " + this.gen + " obj");
...
```

#### <a name="apidoc.element.pdfkit.font.prototype.lineHeight"></a>[function <span class="apidocSignatureSpan">pdfkit.font.prototype.</span>lineHeight (size, includeGap)](#apidoc.element.pdfkit.font.prototype.lineHeight)
- description and source-code
```javascript
lineHeight = function (size, includeGap) {
  var gap;
  if (includeGap == null) {
    includeGap = false;
  }
  gap = includeGap ? this.lineGap : 0;
  return (this.ascender + gap - this.descender) / 1000 * size;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pdfkit.font.prototype.ref"></a>[function <span class="apidocSignatureSpan">pdfkit.font.prototype.</span>ref ()](#apidoc.element.pdfkit.font.prototype.ref)
- description and source-code
```javascript
ref = function () {
  return this.dictionary != null ? this.dictionary : this.dictionary = this.document.ref();
}
```
- example usage
```shell
...
};

PDFFont.prototype.widthOfString = function(text) {
  throw new Error('Must be implemented by subclasses');
};

PDFFont.prototype.ref = function() {
  return this.dictionary != null ? this.dictionary : this.dictionary = this.document.ref();
};

PDFFont.prototype.finalize = function() {
  if (this.embedded || (this.dictionary == null)) {
    return;
  }
  this.embed();
...
```

#### <a name="apidoc.element.pdfkit.font.prototype.widthOfString"></a>[function <span class="apidocSignatureSpan">pdfkit.font.prototype.</span>widthOfString (text)](#apidoc.element.pdfkit.font.prototype.widthOfString)
- description and source-code
```javascript
widthOfString = function (text) {
  throw new Error('Must be implemented by subclasses');
}
```
- example usage
```shell
...
        return _this.lastLine = false;
      });
    };
  })(this));
}

LineWrapper.prototype.wordWidth = function(word) {
  return this.document.widthOfString(word, this) + this.characterSpacing + this.wordSpacing;
};

LineWrapper.prototype.eachWord = function(text, fn) {
  var bk, breaker, fbk, l, last, lbk, shouldContinue, w, word, wordWidths;
  breaker = new LineBreaker(text);
  last = null;
  wordWidths = Object.create(null);
...
```



# <a name="apidoc.module.pdfkit.gradient"></a>[module pdfkit.gradient](#apidoc.module.pdfkit.gradient)

#### <a name="apidoc.element.pdfkit.gradient.PDFGradient"></a>[function <span class="apidocSignatureSpan">pdfkit.gradient.</span>PDFGradient (doc)](#apidoc.element.pdfkit.gradient.PDFGradient)
- description and source-code
```javascript
function PDFGradient(doc) {
  this.doc = doc;
  this.stops = [];
  this.embedded = false;
  this.transform = [1, 0, 0, 1, 0, 0];
  this._colorSpace = 'DeviceRGB';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pdfkit.gradient.PDFLinearGradient"></a>[function <span class="apidocSignatureSpan">pdfkit.gradient.</span>PDFLinearGradient (doc, x1, y1, x2, y2)](#apidoc.element.pdfkit.gradient.PDFLinearGradient)
- description and source-code
```javascript
function PDFLinearGradient(doc, x1, y1, x2, y2) {
  this.doc = doc;
  this.x1 = x1;
  this.y1 = y1;
  this.x2 = x2;
  this.y2 = y2;
  PDFLinearGradient.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pdfkit.gradient.PDFRadialGradient"></a>[function <span class="apidocSignatureSpan">pdfkit.gradient.</span>PDFRadialGradient (doc, x1, y1, r1, x2, y2, r2)](#apidoc.element.pdfkit.gradient.PDFRadialGradient)
- description and source-code
```javascript
function PDFRadialGradient(doc, x1, y1, r1, x2, y2, r2) {
  this.doc = doc;
  this.x1 = x1;
  this.y1 = y1;
  this.r1 = r1;
  this.x2 = x2;
  this.y2 = y2;
  this.r2 = r2;
  PDFRadialGradient.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.pdfkit.image"></a>[module pdfkit.image](#apidoc.module.pdfkit.image)

#### <a name="apidoc.element.pdfkit.image.image"></a>[function <span class="apidocSignatureSpan">pdfkit.</span>image ()](#apidoc.element.pdfkit.image.image)
- description and source-code
```javascript
function PDFImage() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pdfkit.image.open"></a>[function <span class="apidocSignatureSpan">pdfkit.image.</span>open (src, label)](#apidoc.element.pdfkit.image.open)
- description and source-code
```javascript
open = function (src, label) {
  var data, match;
  if (Buffer.isBuffer(src)) {
    data = src;
  } else if (src instanceof ArrayBuffer) {
    data = new Buffer(new Uint8Array(src));
  } else {
    if (match = /^data:.+;base64,(.*)$/.exec(src)) {
      data = new Buffer(match[1], 'base64');
    } else {
      data = fs.readFileSync(src);
      if (!data) {
        return;
      }
    }
  }
  if (data[0] === 0xff && data[1] === 0xd8) {
    return new JPEG(data, label);
  } else if (data[0] === 0x89 && data.toString('ascii', 1, 4) === 'PNG') {
    return new PNG(data, label);
  } else {
    throw new Error('Unknown image format.');
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.pdfkit.line_wrapper"></a>[module pdfkit.line_wrapper](#apidoc.module.pdfkit.line_wrapper)

#### <a name="apidoc.element.pdfkit.line_wrapper.line_wrapper"></a>[function <span class="apidocSignatureSpan">pdfkit.</span>line_wrapper (document, options)](#apidoc.element.pdfkit.line_wrapper.line_wrapper)
- description and source-code
```javascript
function LineWrapper(document, options) {
  var ref;
  this.document = document;
  this.indent = options.indent || 0;
  this.characterSpacing = options.characterSpacing || 0;
  this.wordSpacing = options.wordSpacing === 0;
  this.columns = options.columns || 1;
  this.columnGap = (ref = options.columnGap) != null ? ref : 18;
  this.lineWidth = (options.width - (this.columnGap * (this.columns - 1))) / this.columns;
  this.spaceLeft = this.lineWidth;
  this.startX = this.document.x;
  this.startY = this.document.y;
  this.column = 1;
  this.ellipsis = options.ellipsis;
  this.continuedX = 0;
  this.features = options.features;
  if (options.height != null) {
    this.height = options.height;
    this.maxY = this.startY + options.height;
  } else {
    this.maxY = this.document.page.maxY();
  }
  this.on('firstLine', (function(_this) {
    return function(options) {
      var indent;
      indent = _this.continuedX || _this.indent;
      _this.document.x += indent;
      _this.lineWidth -= indent;
      return _this.once('line', function() {
        _this.document.x -= indent;
        _this.lineWidth += indent;
        if (options.continued && !_this.continuedX) {
          _this.continuedX = _this.indent;
        }
        if (!options.continued) {
          return _this.continuedX = 0;
        }
      });
    };
  })(this));
  this.on('lastLine', (function(_this) {
    return function(options) {
      var align;
      align = options.align;
      if (align === 'justify') {
        options.align = 'left';
      }
      _this.lastLine = true;
      return _this.once('line', function() {
        _this.document.y += options.paragraphGap || 0;
        options.align = align;
        return _this.lastLine = false;
      });
    };
  })(this));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pdfkit.line_wrapper.EventEmitter"></a>[function <span class="apidocSignatureSpan">pdfkit.line_wrapper.</span>EventEmitter ()](#apidoc.element.pdfkit.line_wrapper.EventEmitter)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pdfkit.line_wrapper.init"></a>[function <span class="apidocSignatureSpan">pdfkit.line_wrapper.</span>init ()](#apidoc.element.pdfkit.line_wrapper.init)
- description and source-code
```javascript
init = function () {
  this.domain = null;
  if (EventEmitter.usingDomains) {
    // if there is an active domain, then attach to it.
    domain = domain || require('domain');
    if (domain.active && !(this instanceof domain.Domain)) {
      this.domain = domain.active;
    }
  }

  if (!this._events || this._events === Object.getPrototypeOf(this)._events) {
    this._events = new EventHandlers();
    this._eventsCount = 0;
  }

  this._maxListeners = this._maxListeners || undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pdfkit.line_wrapper.listenerCount"></a>[function <span class="apidocSignatureSpan">pdfkit.line_wrapper.</span>listenerCount (emitter, type)](#apidoc.element.pdfkit.line_wrapper.listenerCount)
- description and source-code
```javascript
listenerCount = function (emitter, type) {
  if (typeof emitter.listenerCount === 'function') {
    return emitter.listenerCount(type);
  } else {
    return listenerCount.call(emitter, type);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.pdfkit.line_wrapper.prototype"></a>[module pdfkit.line_wrapper.prototype](#apidoc.module.pdfkit.line_wrapper.prototype)

#### <a name="apidoc.element.pdfkit.line_wrapper.prototype.constructor"></a>[function <span class="apidocSignatureSpan">pdfkit.line_wrapper.prototype.</span>constructor (document, options)](#apidoc.element.pdfkit.line_wrapper.prototype.constructor)
- description and source-code
```javascript
function LineWrapper(document, options) {
  var ref;
  this.document = document;
  this.indent = options.indent || 0;
  this.characterSpacing = options.characterSpacing || 0;
  this.wordSpacing = options.wordSpacing === 0;
  this.columns = options.columns || 1;
  this.columnGap = (ref = options.columnGap) != null ? ref : 18;
  this.lineWidth = (options.width - (this.columnGap * (this.columns - 1))) / this.columns;
  this.spaceLeft = this.lineWidth;
  this.startX = this.document.x;
  this.startY = this.document.y;
  this.column = 1;
  this.ellipsis = options.ellipsis;
  this.continuedX = 0;
  this.features = options.features;
  if (options.height != null) {
    this.height = options.height;
    this.maxY = this.startY + options.height;
  } else {
    this.maxY = this.document.page.maxY();
  }
  this.on('firstLine', (function(_this) {
    return function(options) {
      var indent;
      indent = _this.continuedX || _this.indent;
      _this.document.x += indent;
      _this.lineWidth -= indent;
      return _this.once('line', function() {
        _this.document.x -= indent;
        _this.lineWidth += indent;
        if (options.continued && !_this.continuedX) {
          _this.continuedX = _this.indent;
        }
        if (!options.continued) {
          return _this.continuedX = 0;
        }
      });
    };
  })(this));
  this.on('lastLine', (function(_this) {
    return function(options) {
      var align;
      align = options.align;
      if (align === 'justify') {
        options.align = 'left';
      }
      _this.lastLine = true;
      return _this.once('line', function() {
        _this.document.y += options.paragraphGap || 0;
        options.align = align;
        return _this.lastLine = false;
      });
    };
  })(this));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pdfkit.line_wrapper.prototype.eachWord"></a>[function <span class="apidocSignatureSpan">pdfkit.line_wrapper.prototype.</span>eachWord (text, fn)](#apidoc.element.pdfkit.line_wrapper.prototype.eachWord)
- description and source-code
```javascript
eachWord = function (text, fn) {
  var bk, breaker, fbk, l, last, lbk, shouldContinue, w, word, wordWidths;
  breaker = new LineBreaker(text);
  last = null;
  wordWidths = Object.create(null);
  while (bk = breaker.nextBreak()) {
    word = text.slice((last != null ? last.position : void 0) || 0, bk.position);
    w = wordWidths[word] != null ? wordWidths[word] : wordWidths[word] = this.wordWidth(word);
    if (w > this.lineWidth + this.continuedX) {
      lbk = last;
      fbk = {};
      while (word.length) {
        l = word.length;
        while (w > this.spaceLeft) {
          w = this.wordWidth(word.slice(0, --l));
        }
        fbk.required = l < word.length;
        shouldContinue = fn(word.slice(0, l), w, fbk, lbk);
        lbk = {
          required: false
        };
        word = word.slice(l);
        w = this.wordWidth(word);
        if (shouldContinue === false) {
          break;
        }
      }
    } else {
      shouldContinue = fn(word, w, bk, last);
    }
    if (shouldContinue === false) {
      break;
    }
    last = bk;
  }
}
```
- example usage
```shell
...
    options.lineWidth = _this.lineWidth;
    y = _this.document.y;
    _this.emit('line', buffer, options, _this);
    return lc++;
  };
})(this);
this.emit('sectionStart', options, this);
this.eachWord(text, (function(_this) {
  return function(word, w, bk, last) {
    var lh, shouldContinue;
    if ((last == null) || last.required) {
      _this.emit('firstLine', options, _this);
      _this.spaceLeft = _this.lineWidth;
    }
    if (w <= _this.spaceLeft) {
...
```

#### <a name="apidoc.element.pdfkit.line_wrapper.prototype.nextSection"></a>[function <span class="apidocSignatureSpan">pdfkit.line_wrapper.prototype.</span>nextSection (options)](#apidoc.element.pdfkit.line_wrapper.prototype.nextSection)
- description and source-code
```javascript
nextSection = function (options) {
  var ref;
  this.emit('sectionEnd', options, this);
  if (++this.column > this.columns) {
    if (this.height != null) {
      return false;
    }
    this.document.addPage();
    this.column = 1;
    this.startY = this.document.page.margins.top;
    this.maxY = this.document.page.maxY();
    this.document.x = this.startX;
    if (this.document._fillColor) {
      (ref = this.document).fillColor.apply(ref, this.document._fillColor);
    }
    this.emit('pageBreak', options, this);
  } else {
    this.document.x += this.lineWidth + this.columnGap;
    this.document.y = this.startY;
    this.emit('columnBreak', options, this);
  }
  this.emit('sectionStart', options, this);
  return true;
}
```
- example usage
```shell
...
  this.wordSpacing = options.wordSpacing;
}
if (options.ellipsis != null) {
  this.ellipsis = options.ellipsis;
}
nextY = this.document.y + this.document.currentLineHeight(true);
if (this.document.y > this.maxY || nextY > this.maxY) {
  this.nextSection();
}
buffer = '';
textWidth = 0;
wc = 0;
lc = 0;
y = this.document.y;
emitLine = (function(_this) {
...
```

#### <a name="apidoc.element.pdfkit.line_wrapper.prototype.wordWidth"></a>[function <span class="apidocSignatureSpan">pdfkit.line_wrapper.prototype.</span>wordWidth (word)](#apidoc.element.pdfkit.line_wrapper.prototype.wordWidth)
- description and source-code
```javascript
wordWidth = function (word) {
  return this.document.widthOfString(word, this) + this.characterSpacing + this.wordSpacing;
}
```
- example usage
```shell
...
    LineWrapper.prototype.eachWord = function(text, fn) {
var bk, breaker, fbk, l, last, lbk, shouldContinue, w, word, wordWidths;
breaker = new LineBreaker(text);
last = null;
wordWidths = Object.create(null);
while (bk = breaker.nextBreak()) {
  word = text.slice((last != null ? last.position : void 0) || 0, bk.position);
  w = wordWidths[word] != null ? wordWidths[word] : wordWidths[word] = this.wordWidth(word);
  if (w > this.lineWidth + this.continuedX) {
    lbk = last;
    fbk = {};
    while (word.length) {
      l = word.length;
      while (w > this.spaceLeft) {
        w = this.wordWidth(word.slice(0, --l));
...
```

#### <a name="apidoc.element.pdfkit.line_wrapper.prototype.wrap"></a>[function <span class="apidocSignatureSpan">pdfkit.line_wrapper.prototype.</span>wrap (text, options)](#apidoc.element.pdfkit.line_wrapper.prototype.wrap)
- description and source-code
```javascript
wrap = function (text, options) {
  var buffer, emitLine, lc, nextY, textWidth, wc, y;
  if (options.indent != null) {
    this.indent = options.indent;
  }
  if (options.characterSpacing != null) {
    this.characterSpacing = options.characterSpacing;
  }
  if (options.wordSpacing != null) {
    this.wordSpacing = options.wordSpacing;
  }
  if (options.ellipsis != null) {
    this.ellipsis = options.ellipsis;
  }
  nextY = this.document.y + this.document.currentLineHeight(true);
  if (this.document.y > this.maxY || nextY > this.maxY) {
    this.nextSection();
  }
  buffer = '';
  textWidth = 0;
  wc = 0;
  lc = 0;
  y = this.document.y;
  emitLine = (function(_this) {
    return function() {
      options.textWidth = textWidth + _this.wordSpacing * (wc - 1);
      options.wordCount = wc;
      options.lineWidth = _this.lineWidth;
      y = _this.document.y;
      _this.emit('line', buffer, options, _this);
      return lc++;
    };
  })(this);
  this.emit('sectionStart', options, this);
  this.eachWord(text, (function(_this) {
    return function(word, w, bk, last) {
      var lh, shouldContinue;
      if ((last == null) || last.required) {
        _this.emit('firstLine', options, _this);
        _this.spaceLeft = _this.lineWidth;
      }
      if (w <= _this.spaceLeft) {
        buffer += word;
        textWidth += w;
        wc++;
      }
      if (bk.required || w > _this.spaceLeft) {
        if (bk.required) {
          _this.emit('lastLine', options, _this);
        }
        lh = _this.document.currentLineHeight(true);
        if ((_this.height != null) && _this.ellipsis && _this.document.y + lh * 2 > _this.maxY && _this.column >= _this.columns) {
          if (_this.ellipsis === true) {
            _this.ellipsis = '…';
          }
          buffer = buffer.replace(/\s+$/, '');
          textWidth = _this.wordWidth(buffer + _this.ellipsis);
          while (textWidth > _this.lineWidth) {
            buffer = buffer.slice(0, -1).replace(/\s+$/, '');
            textWidth = _this.wordWidth(buffer + _this.ellipsis);
          }
          buffer = buffer + _this.ellipsis;
        }
        emitLine();
        if (_this.document.y + lh > _this.maxY) {
          shouldContinue = _this.nextSection();
          if (!shouldContinue) {
            wc = 0;
            buffer = '';
            return false;
          }
        }
        if (bk.required) {
          if (w > _this.spaceLeft) {
            buffer = word;
            textWidth = w;
            wc = 1;
            emitLine();
          }
          _this.spaceLeft = _this.lineWidth;
          buffer = '';
          textWidth = 0;
          return wc = 0;
        } else {
          _this.spaceLeft = _this.lineWidth - w;
          buffer = word;
          textWidth = w;
          return wc = 1;
        }
      } else {
        return _this.spaceLeft -= w;
      }
    };
  })(this));
  if (wc > 0) {
    this.emit('lastLine', options, this);
    emitLine();
  }
  this.emit('sectionEnd', options, this);
  if (options.continued === true) {
    if (lc > 1) {
      this.continuedX = 0;
    }
    this.continuedX += options.textWidth;
    return this.document.y = y;
  } else {
    return this.document.x = this.startX;
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.pdfkit.object"></a>[module pdfkit.object](#apidoc.module.pdfkit.object)

#### <a name="apidoc.element.pdfkit.object.object"></a>[function <span class="apidocSignatureSpan">pdfkit.</span>object ()](#apidoc.element.pdfkit.object.object)
- description and source-code
```javascript
function PDFObject() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pdfkit.object.convert"></a>[function <span class="apidocSignatureSpan">pdfkit.object.</span>convert (object)](#apidoc.element.pdfkit.object.convert)
- description and source-code
```javascript
convert = function (object) {
  var e, i, isUnicode, items, j, key, out, ref, string, val;
  if (typeof object === 'string') {
    return '/' + object;
  } else if (object instanceof String) {
    string = object.replace(escapableRe, function(c) {
      return escapable[c];
    });
    isUnicode = false;
    for (i = j = 0, ref = string.length; j < ref; i = j += 1) {
      if (string.charCodeAt(i) > 0x7f) {
        isUnicode = true;
        break;
      }
    }
    if (isUnicode) {
      string = swapBytes(new Buffer('\ufeff' + string, 'utf16le')).toString('binary');
    }
    return '(' + string + ')';
  } else if (Buffer.isBuffer(object)) {
    return '<' + object.toString('hex') + '>';
  } else if (object instanceof PDFReference) {
    return object.toString();
  } else if (object instanceof Date) {
    return '(D:' + pad(object.getUTCFullYear(), 4) + pad(object.getUTCMonth() + 1, 2) + pad(object.getUTCDate(), 2) + pad(object
.getUTCHours(), 2) + pad(object.getUTCMinutes(), 2) + pad(object.getUTCSeconds(), 2) + 'Z)';
  } else if (Array.isArray(object)) {
    items = ((function() {
      var k, len, results;
      results = [];
      for (k = 0, len = object.length; k < len; k++) {
        e = object[k];
        results.push(PDFObject.convert(e));
      }
      return results;
    })()).join(' ');
    return '[' + items + ']';
  } else if ({}.toString.call(object) === '[object Object]') {
    out = ['<<'];
    for (key in object) {
      val = object[key];
      out.push('/' + key + ' ' + PDFObject.convert(val));
    }
    out.push('>>');
    return out.join('\n');
  } else {
    return '' + object;
  }
}
```
- example usage
```shell
...
  return '(D:' + pad(object.getUTCFullYear(), 4) + pad(object.getUTCMonth() + 1, 2) + pad(object.getUTCDate(), 2) + pad(object.getUTCHours
(), 2) + pad(object.getUTCMinutes(), 2) + pad(object.getUTCSeconds(), 2) + 'Z)';
} else if (Array.isArray(object)) {
  items = ((function() {
    var k, len, results;
    results = [];
    for (k = 0, len = object.length; k < len; k++) {
      e = object[k];
      results.push(PDFObject.convert(e));
    }
    return results;
  })()).join(' ');
  return '[' + items + ']';
} else if ({}.toString.call(object) === '[object Object]') {
  out = ['<<'];
  for (key in object) {
...
```



# <a name="apidoc.module.pdfkit.page"></a>[module pdfkit.page](#apidoc.module.pdfkit.page)

#### <a name="apidoc.element.pdfkit.page.page"></a>[function <span class="apidocSignatureSpan">pdfkit.</span>page (document, options)](#apidoc.element.pdfkit.page.page)
- description and source-code
```javascript
function PDFPage(document, options) {
  var dimensions;
  this.document = document;
  if (options == null) {
    options = {};
  }
  this.size = options.size || 'letter';
  this.layout = options.layout || 'portrait';
  if (typeof options.margin === 'number') {
    this.margins = {
      top: options.margin,
      left: options.margin,
      bottom: options.margin,
      right: options.margin
    };
  } else {
    this.margins = options.margins || DEFAULT_MARGINS;
  }
  dimensions = Array.isArray(this.size) ? this.size : SIZES[this.size.toUpperCase()];
  this.width = dimensions[this.layout === 'portrait' ? 0 : 1];
  this.height = dimensions[this.layout === 'portrait' ? 1 : 0];
  this.content = this.document.ref();
  this.resources = this.document.ref({
    ProcSet: ['PDF', 'Text', 'ImageB', 'ImageC', 'ImageI']
  });
  Object.defineProperties(this, {
    fonts: {
      get: (function(_this) {
        return function() {
          var base;
          return (base = _this.resources.data).Font != null ? base.Font : base.Font = {};
        };
      })(this)
    },
    xobjects: {
      get: (function(_this) {
        return function() {
          var base;
          return (base = _this.resources.data).XObject != null ? base.XObject : base.XObject = {};
        };
      })(this)
    },
    ext_gstates: {
      get: (function(_this) {
        return function() {
          var base;
          return (base = _this.resources.data).ExtGState != null ? base.ExtGState : base.ExtGState = {};
        };
      })(this)
    },
    patterns: {
      get: (function(_this) {
        return function() {
          var base;
          return (base = _this.resources.data).Pattern != null ? base.Pattern : base.Pattern = {};
        };
      })(this)
    },
    annotations: {
      get: (function(_this) {
        return function() {
          var base;
          return (base = _this.dictionary.data).Annots != null ? base.Annots : base.Annots = [];
        };
      })(this)
    }
  });
  this.dictionary = this.document.ref({
    Type: 'Page',
    Parent: this.document._root.data.Pages,
    MediaBox: [0, 0, this.width, this.height],
    Contents: this.content,
    Resources: this.resources
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.pdfkit.page.prototype"></a>[module pdfkit.page.prototype](#apidoc.module.pdfkit.page.prototype)

#### <a name="apidoc.element.pdfkit.page.prototype.end"></a>[function <span class="apidocSignatureSpan">pdfkit.page.prototype.</span>end ()](#apidoc.element.pdfkit.page.prototype.end)
- description and source-code
```javascript
end = function () {
  this.dictionary.end();
  this.resources.end();
  return this.content.end();
}
```
- example usage
```shell
...
doc.addPage()
   .fillColor("blue")
   .text('Here is a link!', 100, 100)
   .underline(100, 100, 160, 27, color: "#0000FF")
   .link(100, 100, 160, 27, 'http://google.com/')

# Finalize PDF file
doc.end()
'''

[The PDF output from this example](http://pdfkit.org/demo/out.pdf) (with a few additions) shows the power of PDFKit — producing
complex documents with a very small amount of code.  For more, see the 'demo' folder and the
[PDFKit programming guide](http://pdfkit.org/docs/getting_started.html).

## Browser Usage
...
```

#### <a name="apidoc.element.pdfkit.page.prototype.maxY"></a>[function <span class="apidocSignatureSpan">pdfkit.page.prototype.</span>maxY ()](#apidoc.element.pdfkit.page.prototype.maxY)
- description and source-code
```javascript
maxY = function () {
  return this.height - this.margins.bottom;
}
```
- example usage
```shell
...
this.ellipsis = options.ellipsis;
this.continuedX = 0;
this.features = options.features;
if (options.height != null) {
  this.height = options.height;
  this.maxY = this.startY + options.height;
} else {
  this.maxY = this.document.page.maxY();
}
this.on('firstLine', (function(_this) {
  return function(options) {
    var indent;
    indent = _this.continuedX || _this.indent;
    _this.document.x += indent;
    _this.lineWidth -= indent;
...
```

#### <a name="apidoc.element.pdfkit.page.prototype.write"></a>[function <span class="apidocSignatureSpan">pdfkit.page.prototype.</span>write (chunk)](#apidoc.element.pdfkit.page.prototype.write)
- description and source-code
```javascript
write = function (chunk) {
  return this.content.write(chunk);
}
```
- example usage
```shell
...
}

PDFPage.prototype.maxY = function() {
  return this.height - this.margins.bottom;
};

PDFPage.prototype.write = function(chunk) {
  return this.content.write(chunk);
};

PDFPage.prototype.end = function() {
  this.dictionary.end();
  this.resources.end();
  return this.content.end();
};
...
```



# <a name="apidoc.module.pdfkit.path"></a>[module pdfkit.path](#apidoc.module.pdfkit.path)

#### <a name="apidoc.element.pdfkit.path.path"></a>[function <span class="apidocSignatureSpan">pdfkit.</span>path ()](#apidoc.element.pdfkit.path.path)
- description and source-code
```javascript
function SVGPath() {}
```
- example usage
```shell
...
.lineTo(100, 250)
.lineTo(200, 250)
.fill("#FF3300")

# Apply some transforms and render an SVG path with the 'even-odd' fill rule
doc.scale(0.6)
.translate(470, -380)
.path('M 250,75 L 323,301 131,161 369,161 177,301 z')
.fill('red', 'even-odd')
.restore()

# Add some text with annotations
doc.addPage()
.fillColor("blue")
.text('Here is a link!', 100, 100)
...
```

#### <a name="apidoc.element.pdfkit.path.apply"></a>[function <span class="apidocSignatureSpan">pdfkit.path.</span>apply (doc, path)](#apidoc.element.pdfkit.path.apply)
- description and source-code
```javascript
apply = function (doc, path) {
  var commands;
  commands = parse(path);
  return apply(commands, doc);
}
```
- example usage
```shell
...

function PDFLinearGradient(doc, x1, y1, x2, y2) {
  this.doc = doc;
  this.x1 = x1;
  this.y1 = y1;
  this.x2 = x2;
  this.y2 = y2;
  PDFLinearGradient.__super__.constructor.apply(this, arguments);
}

PDFLinearGradient.prototype.shader = function(fn) {
  return this.doc.ref({
    ShadingType: 2,
    ColorSpace: this._colorSpace,
    Coords: [this.x1, this.y1, this.x2, this.y2],
...
```



# <a name="apidoc.module.pdfkit.reference"></a>[module pdfkit.reference](#apidoc.module.pdfkit.reference)

#### <a name="apidoc.element.pdfkit.reference.reference"></a>[function <span class="apidocSignatureSpan">pdfkit.</span>reference (document, id, data)](#apidoc.element.pdfkit.reference.reference)
- description and source-code
```javascript
function PDFReference(document, id, data) {
  this.document = document;
  this.id = id;
  this.data = data != null ? data : {};
  this.finalize = bind(this.finalize, this);
  PDFReference.__super__.constructor.call(this, {
    decodeStrings: false
  });
  this.gen = 0;
  this.deflate = null;
  this.compress = this.document.compress && !this.data.Filter;
  this.uncompressedLength = 0;
  this.chunks = [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pdfkit.reference.WritableState"></a>[function <span class="apidocSignatureSpan">pdfkit.reference.</span>WritableState (options, stream)](#apidoc.element.pdfkit.reference.WritableState)
- description and source-code
```javascript
function WritableState(options, stream) {
  options = options || {};

  // object stream flag to indicate whether or not this stream
  // contains buffers or objects.
  this.objectMode = !!options.objectMode;

  if (stream instanceof Stream.Duplex)
    this.objectMode = this.objectMode || !!options.writableObjectMode;

  // the point at which write() starts returning false
  // Note: 0 is a valid value, means that we always return false if
  // the entire buffer is not flushed immediately on write()
  var hwm = options.highWaterMark;
  var defaultHwm = this.objectMode ? 16 : 16 * 1024;
  this.highWaterMark = (hwm || hwm === 0) ? hwm : defaultHwm;

  // cast to ints.
  this.highWaterMark = ~~this.highWaterMark;

  // drain event flag.
  this.needDrain = false;
  // at the start of calling end()
  this.ending = false;
  // when end() has been called, and returned
  this.ended = false;
  // when 'finish' is emitted
  this.finished = false;

  // should we decode strings into buffers before passing to _write?
  // this is here so that some node-core streams can optimize string
  // handling at a lower level.
  var noDecode = options.decodeStrings === false;
  this.decodeStrings = !noDecode;

  // Crypto is kind of old and crusty.  Historically, its default string
  // encoding is 'binary' so we have to make this configurable.
  // Everything else in the universe uses 'utf8', though.
  this.defaultEncoding = options.defaultEncoding || 'utf8';

  // not an actual buffer we keep track of, but a measurement
  // of how much we're waiting to get pushed to some underlying
  // socket or file.
  this.length = 0;

  // a flag to see when we're in the middle of a write.
  this.writing = false;

  // when true all writes will be buffered until .uncork() call
  this.corked = 0;

  // a flag to be able to tell if the onwrite cb is called immediately,
  // or on a later tick.  We set this to true at first, because any
  // actions that shouldn't happen until "later" should generally also
  // not happen before the first write call.
  this.sync = true;

  // a flag to know if we're processing previously buffered items, which
  // may call the _write() callback in the same tick, so that we don't
  // end up in an overlapped onwrite situation.
  this.bufferProcessing = false;

  // the callback that's passed to _write(chunk,cb)
  this.onwrite = function(er) {
    onwrite(stream, er);
  };

  // the callback that the user supplies to write(chunk,encoding,cb)
  this.writecb = null;

  // the amount that is being written when _write is called.
  this.writelen = 0;

  this.bufferedRequest = null;
  this.lastBufferedRequest = null;

  // number of pending user-supplied write callbacks
  // this must be 0 before 'finish' can be emitted
  this.pendingcb = 0;

  // emit prefinish if the only thing we're waiting for is _write cbs
  // This is relevant for synchronous Transform streams
  this.prefinished = false;

  // True if the error was already emitted and should not be thrown again
  this.errorEmitted = false;

  // count buffered requests
  this.bufferedRequestCount = 0;

  // allocate the first CorkedRequest, there is always
  // one allocated and free to use, and we maintain at most two
  this.corkedRequestsFree = new CorkedRequest(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pdfkit.reference.super_"></a>[function <span class="apidocSignatureSpan">pdfkit.reference.</span>super_ ()](#apidoc.element.pdfkit.reference.super_)
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



# <a name="apidoc.module.pdfkit.reference.prototype"></a>[module pdfkit.reference.prototype](#apidoc.module.pdfkit.reference.prototype)

#### <a name="apidoc.element.pdfkit.reference.prototype._write"></a>[function <span class="apidocSignatureSpan">pdfkit.reference.prototype.</span>_write (chunk, encoding, callback)](#apidoc.element.pdfkit.reference.prototype._write)
- description and source-code
```javascript
_write = function (chunk, encoding, callback) {
  var base;
  if (!Buffer.isBuffer(chunk)) {
    chunk = new Buffer(chunk + '\n', 'binary');
  }
  this.uncompressedLength += chunk.length;
  if ((base = this.data).Length == null) {
    base.Length = 0;
  }
  if (this.compress) {
    if (!this.deflate) {
      this.initDeflate();
    }
    this.deflate.write(chunk);
  } else {
    this.chunks.push(chunk);
    this.data.Length += chunk.length;
  }
  return callback();
}
```
- example usage
```shell
...
    return this.finalize();
  }
};

PDFReference.prototype.finalize = function() {
  var chunk, i, len, ref;
  this.offset = this.document._offset;
  this.document._write(this.id + " " + this.gen + " obj");
  this.document._write(PDFObject.convert(this.data));
  if (this.chunks.length) {
    this.document._write('stream');
    ref = this.chunks;
    for (i = 0, len = ref.length; i < len; i++) {
      chunk = ref[i];
      this.document._write(chunk);
...
```

#### <a name="apidoc.element.pdfkit.reference.prototype.constructor"></a>[function <span class="apidocSignatureSpan">pdfkit.reference.prototype.</span>constructor (document, id, data)](#apidoc.element.pdfkit.reference.prototype.constructor)
- description and source-code
```javascript
function PDFReference(document, id, data) {
  this.document = document;
  this.id = id;
  this.data = data != null ? data : {};
  this.finalize = bind(this.finalize, this);
  PDFReference.__super__.constructor.call(this, {
    decodeStrings: false
  });
  this.gen = 0;
  this.deflate = null;
  this.compress = this.document.compress && !this.data.Filter;
  this.uncompressedLength = 0;
  this.chunks = [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pdfkit.reference.prototype.end"></a>[function <span class="apidocSignatureSpan">pdfkit.reference.prototype.</span>end (chunk)](#apidoc.element.pdfkit.reference.prototype.end)
- description and source-code
```javascript
end = function (chunk) {
  PDFReference.__super__.end.apply(this, arguments);
  if (this.deflate) {
    return this.deflate.end();
  } else {
    return this.finalize();
  }
}
```
- example usage
```shell
...
doc.addPage()
   .fillColor("blue")
   .text('Here is a link!', 100, 100)
   .underline(100, 100, 160, 27, color: "#0000FF")
   .link(100, 100, 160, 27, 'http://google.com/')

# Finalize PDF file
doc.end()
'''

[The PDF output from this example](http://pdfkit.org/demo/out.pdf) (with a few additions) shows the power of PDFKit — producing
complex documents with a very small amount of code.  For more, see the 'demo' folder and the
[PDFKit programming guide](http://pdfkit.org/docs/getting_started.html).

## Browser Usage
...
```

#### <a name="apidoc.element.pdfkit.reference.prototype.finalize"></a>[function <span class="apidocSignatureSpan">pdfkit.reference.prototype.</span>finalize ()](#apidoc.element.pdfkit.reference.prototype.finalize)
- description and source-code
```javascript
finalize = function () {
  var chunk, i, len, ref;
  this.offset = this.document._offset;
  this.document._write(this.id + " " + this.gen + " obj");
  this.document._write(PDFObject.convert(this.data));
  if (this.chunks.length) {
    this.document._write('stream');
    ref = this.chunks;
    for (i = 0, len = ref.length; i < len; i++) {
      chunk = ref[i];
      this.document._write(chunk);
    }
    this.chunks.length = 0;
    this.document._write('\nendstream');
  }
  this.document._write('endobj');
  return this.document._refEnd(this);
}
```
- example usage
```shell
...
};

PDFReference.prototype.end = function(chunk) {
  PDFReference.__super__.end.apply(this, arguments);
  if (this.deflate) {
    return this.deflate.end();
  } else {
    return this.finalize();
  }
};

PDFReference.prototype.finalize = function() {
  var chunk, i, len, ref;
  this.offset = this.document._offset;
  this.document._write(this.id + " " + this.gen + " obj");
...
```

#### <a name="apidoc.element.pdfkit.reference.prototype.initDeflate"></a>[function <span class="apidocSignatureSpan">pdfkit.reference.prototype.</span>initDeflate ()](#apidoc.element.pdfkit.reference.prototype.initDeflate)
- description and source-code
```javascript
initDeflate = function () {
  this.data.Filter = 'FlateDecode';
  this.deflate = zlib.createDeflate();
  this.deflate.on('data', (function(_this) {
    return function(chunk) {
      _this.chunks.push(chunk);
      return _this.data.Length += chunk.length;
    };
  })(this));
  return this.deflate.on('end', this.finalize);
}
```
- example usage
```shell
...
}
this.uncompressedLength += chunk.length;
if ((base = this.data).Length == null) {
  base.Length = 0;
}
if (this.compress) {
  if (!this.deflate) {
    this.initDeflate();
  }
  this.deflate.write(chunk);
} else {
  this.chunks.push(chunk);
  this.data.Length += chunk.length;
}
return callback();
...
```

#### <a name="apidoc.element.pdfkit.reference.prototype.toString"></a>[function <span class="apidocSignatureSpan">pdfkit.reference.prototype.</span>toString ()](#apidoc.element.pdfkit.reference.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return this.id + " " + this.gen + " R";
}
```
- example usage
```shell
...
      if (!data) {
        return;
      }
    }
  }
  if (data[0] === 0xff && data[1] === 0xd8) {
    return new JPEG(data, label);
  } else if (data[0] === 0x89 && data.toString('ascii', 1, 4) === 'PNG') {
    return new PNG(data, label);
  } else {
    throw new Error('Unknown image format.');
  }
};

return PDFImage;
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
