# api documentation for  [mississippi (v1.3.0)](https://github.com/maxogden/mississippi#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-mississippi.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-mississippi) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-mississippi.svg)](https://travis-ci.org/npmdoc/node-npmdoc-mississippi)
#### a collection of useful streams

[![NPM](https://nodei.co/npm/mississippi.png?downloads=true)](https://www.npmjs.com/package/mississippi)

[![apidoc](https://npmdoc.github.io/node-npmdoc-mississippi/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-mississippi_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-mississippi/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-mississippi/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-mississippi/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "max ogden"
    },
    "bugs": {
        "url": "https://github.com/maxogden/mississippi/issues"
    },
    "dependencies": {
        "concat-stream": "^1.5.0",
        "duplexify": "^3.4.2",
        "end-of-stream": "^1.1.0",
        "flush-write-stream": "^1.0.0",
        "from2": "^2.1.0",
        "parallel-transform": "^1.1.0",
        "pump": "^1.0.0",
        "pumpify": "^1.3.3",
        "stream-each": "^1.1.0",
        "through2": "^2.0.0"
    },
    "description": "a collection of useful streams",
    "devDependencies": {},
    "directories": {},
    "dist": {
        "shasum": "d201583eb12327e3c5c1642a404a9cacf94e34f5",
        "tarball": "https://registry.npmjs.org/mississippi/-/mississippi-1.3.0.tgz"
    },
    "gitHead": "dd64841b932d06baf7859ee80db78d139c90b4c7",
    "homepage": "https://github.com/maxogden/mississippi#readme",
    "license": "BSD-2-Clause",
    "main": "index.js",
    "maintainers": [
        {
            "name": "maxogden",
            "email": "max@maxogden.com"
        }
    ],
    "name": "mississippi",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/maxogden/mississippi.git"
    },
    "scripts": {
        "test": "echo \"Error: no test specified\" && exit 1"
    },
    "version": "1.3.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module mississippi](#apidoc.module.mississippi)
1.  [function <span class="apidocSignatureSpan">mississippi.</span>concat (opts, cb)](#apidoc.element.mississippi.concat)
1.  [function <span class="apidocSignatureSpan">mississippi.</span>concat.super_ (options)](#apidoc.element.mississippi.concat.super_)
1.  [function <span class="apidocSignatureSpan">mississippi.</span>duplex (writable, readable, opts)](#apidoc.element.mississippi.duplex)
1.  [function <span class="apidocSignatureSpan">mississippi.</span>duplex.super_ (options)](#apidoc.element.mississippi.duplex.super_)
1.  [function <span class="apidocSignatureSpan">mississippi.</span>each (stream, fn, cb)](#apidoc.element.mississippi.each)
1.  [function <span class="apidocSignatureSpan">mississippi.</span>finished (stream, opts, callback)](#apidoc.element.mississippi.finished)
1.  [function <span class="apidocSignatureSpan">mississippi.</span>from (opts, read)](#apidoc.element.mississippi.from)
1.  [function <span class="apidocSignatureSpan">mississippi.</span>pipe ()](#apidoc.element.mississippi.pipe)
1.  [function <span class="apidocSignatureSpan">mississippi.</span>pipeline ()](#apidoc.element.mississippi.pipeline)
1.  [function <span class="apidocSignatureSpan">mississippi.</span>pipeline.obj ()](#apidoc.element.mississippi.pipeline.obj)
1.  [function <span class="apidocSignatureSpan">mississippi.</span>through (options, transform, flush)](#apidoc.element.mississippi.through)
1.  [function <span class="apidocSignatureSpan">mississippi.</span>to (opts, write, flush)](#apidoc.element.mississippi.to)
1.  object <span class="apidocSignatureSpan">mississippi.</span>concat.prototype
1.  object <span class="apidocSignatureSpan">mississippi.</span>concat.super_.WritableState.prototype
1.  object <span class="apidocSignatureSpan">mississippi.</span>concat.super_.prototype
1.  object <span class="apidocSignatureSpan">mississippi.</span>duplex.prototype
1.  object <span class="apidocSignatureSpan">mississippi.</span>duplex.super_.prototype
1.  object <span class="apidocSignatureSpan">mississippi.</span>duplex.super_.super_.prototype
1.  object <span class="apidocSignatureSpan">mississippi.</span>pipeline.obj.prototype
1.  object <span class="apidocSignatureSpan">mississippi.</span>pipeline.prototype
1.  object <span class="apidocSignatureSpan">mississippi.</span>to.prototype

#### [module mississippi.concat](#apidoc.module.mississippi.concat)
1.  [function <span class="apidocSignatureSpan">mississippi.</span>concat (opts, cb)](#apidoc.element.mississippi.concat.concat)
1.  [function <span class="apidocSignatureSpan">mississippi.concat.</span>super_ (options)](#apidoc.element.mississippi.concat.super_)

#### [module mississippi.concat.prototype](#apidoc.module.mississippi.concat.prototype)
1.  [function <span class="apidocSignatureSpan">mississippi.concat.prototype.</span>_write (chunk, enc, next)](#apidoc.element.mississippi.concat.prototype._write)
1.  [function <span class="apidocSignatureSpan">mississippi.concat.prototype.</span>getBody ()](#apidoc.element.mississippi.concat.prototype.getBody)
1.  [function <span class="apidocSignatureSpan">mississippi.concat.prototype.</span>inferEncoding (buff)](#apidoc.element.mississippi.concat.prototype.inferEncoding)

#### [module mississippi.concat.super_](#apidoc.module.mississippi.concat.super_)
1.  [function <span class="apidocSignatureSpan">mississippi.concat.</span>super_ ()](#apidoc.element.mississippi.concat.super_.super_)
1.  [function <span class="apidocSignatureSpan">mississippi.concat.super_.</span>WritableState (options, stream)](#apidoc.element.mississippi.concat.super_.WritableState)

#### [module mississippi.concat.super_.WritableState.prototype](#apidoc.module.mississippi.concat.super_.WritableState.prototype)
1.  [function <span class="apidocSignatureSpan">mississippi.concat.super_.WritableState.prototype.</span>getBuffer ()](#apidoc.element.mississippi.concat.super_.WritableState.prototype.getBuffer)

#### [module mississippi.concat.super_.prototype](#apidoc.module.mississippi.concat.super_.prototype)
1.  [function <span class="apidocSignatureSpan">mississippi.concat.super_.prototype.</span>_write (chunk, encoding, cb)](#apidoc.element.mississippi.concat.super_.prototype._write)
1.  [function <span class="apidocSignatureSpan">mississippi.concat.super_.prototype.</span>cork ()](#apidoc.element.mississippi.concat.super_.prototype.cork)
1.  [function <span class="apidocSignatureSpan">mississippi.concat.super_.prototype.</span>end (chunk, encoding, cb)](#apidoc.element.mississippi.concat.super_.prototype.end)
1.  [function <span class="apidocSignatureSpan">mississippi.concat.super_.prototype.</span>pipe ()](#apidoc.element.mississippi.concat.super_.prototype.pipe)
1.  [function <span class="apidocSignatureSpan">mississippi.concat.super_.prototype.</span>setDefaultEncoding (encoding)](#apidoc.element.mississippi.concat.super_.prototype.setDefaultEncoding)
1.  [function <span class="apidocSignatureSpan">mississippi.concat.super_.prototype.</span>uncork ()](#apidoc.element.mississippi.concat.super_.prototype.uncork)
1.  [function <span class="apidocSignatureSpan">mississippi.concat.super_.prototype.</span>write (chunk, encoding, cb)](#apidoc.element.mississippi.concat.super_.prototype.write)
1.  object <span class="apidocSignatureSpan">mississippi.concat.super_.prototype.</span>_writev

#### [module mississippi.duplex](#apidoc.module.mississippi.duplex)
1.  [function <span class="apidocSignatureSpan">mississippi.</span>duplex (writable, readable, opts)](#apidoc.element.mississippi.duplex.duplex)
1.  [function <span class="apidocSignatureSpan">mississippi.duplex.</span>obj (writable, readable, opts)](#apidoc.element.mississippi.duplex.obj)
1.  [function <span class="apidocSignatureSpan">mississippi.duplex.</span>super_ (options)](#apidoc.element.mississippi.duplex.super_)

#### [module mississippi.duplex.prototype](#apidoc.module.mississippi.duplex.prototype)
1.  [function <span class="apidocSignatureSpan">mississippi.duplex.prototype.</span>_destroy (err)](#apidoc.element.mississippi.duplex.prototype._destroy)
1.  [function <span class="apidocSignatureSpan">mississippi.duplex.prototype.</span>_finish (cb)](#apidoc.element.mississippi.duplex.prototype._finish)
1.  [function <span class="apidocSignatureSpan">mississippi.duplex.prototype.</span>_forward ()](#apidoc.element.mississippi.duplex.prototype._forward)
1.  [function <span class="apidocSignatureSpan">mississippi.duplex.prototype.</span>_read ()](#apidoc.element.mississippi.duplex.prototype._read)
1.  [function <span class="apidocSignatureSpan">mississippi.duplex.prototype.</span>_write (data, enc, cb)](#apidoc.element.mississippi.duplex.prototype._write)
1.  [function <span class="apidocSignatureSpan">mississippi.duplex.prototype.</span>cork ()](#apidoc.element.mississippi.duplex.prototype.cork)
1.  [function <span class="apidocSignatureSpan">mississippi.duplex.prototype.</span>destroy (err)](#apidoc.element.mississippi.duplex.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">mississippi.duplex.prototype.</span>end (data, enc, cb)](#apidoc.element.mississippi.duplex.prototype.end)
1.  [function <span class="apidocSignatureSpan">mississippi.duplex.prototype.</span>setReadable (readable)](#apidoc.element.mississippi.duplex.prototype.setReadable)
1.  [function <span class="apidocSignatureSpan">mississippi.duplex.prototype.</span>setWritable (writable)](#apidoc.element.mississippi.duplex.prototype.setWritable)
1.  [function <span class="apidocSignatureSpan">mississippi.duplex.prototype.</span>uncork ()](#apidoc.element.mississippi.duplex.prototype.uncork)

#### [module mississippi.duplex.super_](#apidoc.module.mississippi.duplex.super_)
1.  [function <span class="apidocSignatureSpan">mississippi.duplex.</span>super_ (options)](#apidoc.element.mississippi.duplex.super_.super_)

#### [module mississippi.duplex.super_.prototype](#apidoc.module.mississippi.duplex.super_.prototype)
1.  [function <span class="apidocSignatureSpan">mississippi.duplex.super_.prototype.</span>_write (chunk, encoding, cb)](#apidoc.element.mississippi.duplex.super_.prototype._write)
1.  [function <span class="apidocSignatureSpan">mississippi.duplex.super_.prototype.</span>cork ()](#apidoc.element.mississippi.duplex.super_.prototype.cork)
1.  [function <span class="apidocSignatureSpan">mississippi.duplex.super_.prototype.</span>end (chunk, encoding, cb)](#apidoc.element.mississippi.duplex.super_.prototype.end)
1.  [function <span class="apidocSignatureSpan">mississippi.duplex.super_.prototype.</span>setDefaultEncoding (encoding)](#apidoc.element.mississippi.duplex.super_.prototype.setDefaultEncoding)
1.  [function <span class="apidocSignatureSpan">mississippi.duplex.super_.prototype.</span>uncork ()](#apidoc.element.mississippi.duplex.super_.prototype.uncork)
1.  [function <span class="apidocSignatureSpan">mississippi.duplex.super_.prototype.</span>write (chunk, encoding, cb)](#apidoc.element.mississippi.duplex.super_.prototype.write)
1.  object <span class="apidocSignatureSpan">mississippi.duplex.super_.prototype.</span>_writev

#### [module mississippi.duplex.super_.super_.prototype](#apidoc.module.mississippi.duplex.super_.super_.prototype)
1.  [function <span class="apidocSignatureSpan">mississippi.duplex.super_.super_.prototype.</span>_read (n)](#apidoc.element.mississippi.duplex.super_.super_.prototype._read)
1.  [function <span class="apidocSignatureSpan">mississippi.duplex.super_.super_.prototype.</span>addListener (ev, fn)](#apidoc.element.mississippi.duplex.super_.super_.prototype.addListener)
1.  [function <span class="apidocSignatureSpan">mississippi.duplex.super_.super_.prototype.</span>isPaused ()](#apidoc.element.mississippi.duplex.super_.super_.prototype.isPaused)
1.  [function <span class="apidocSignatureSpan">mississippi.duplex.super_.super_.prototype.</span>on (ev, fn)](#apidoc.element.mississippi.duplex.super_.super_.prototype.on)
1.  [function <span class="apidocSignatureSpan">mississippi.duplex.super_.super_.prototype.</span>pause ()](#apidoc.element.mississippi.duplex.super_.super_.prototype.pause)
1.  [function <span class="apidocSignatureSpan">mississippi.duplex.super_.super_.prototype.</span>pipe (dest, pipeOpts)](#apidoc.element.mississippi.duplex.super_.super_.prototype.pipe)
1.  [function <span class="apidocSignatureSpan">mississippi.duplex.super_.super_.prototype.</span>push (chunk, encoding)](#apidoc.element.mississippi.duplex.super_.super_.prototype.push)
1.  [function <span class="apidocSignatureSpan">mississippi.duplex.super_.super_.prototype.</span>read (n)](#apidoc.element.mississippi.duplex.super_.super_.prototype.read)
1.  [function <span class="apidocSignatureSpan">mississippi.duplex.super_.super_.prototype.</span>resume ()](#apidoc.element.mississippi.duplex.super_.super_.prototype.resume)
1.  [function <span class="apidocSignatureSpan">mississippi.duplex.super_.super_.prototype.</span>setEncoding (enc)](#apidoc.element.mississippi.duplex.super_.super_.prototype.setEncoding)
1.  [function <span class="apidocSignatureSpan">mississippi.duplex.super_.super_.prototype.</span>unpipe (dest)](#apidoc.element.mississippi.duplex.super_.super_.prototype.unpipe)
1.  [function <span class="apidocSignatureSpan">mississippi.duplex.super_.super_.prototype.</span>unshift (chunk)](#apidoc.element.mississippi.duplex.super_.super_.prototype.unshift)
1.  [function <span class="apidocSignatureSpan">mississippi.duplex.super_.super_.prototype.</span>wrap (stream)](#apidoc.element.mississippi.duplex.super_.super_.prototype.wrap)

#### [module mississippi.from](#apidoc.module.mississippi.from)
1.  [function <span class="apidocSignatureSpan">mississippi.</span>from (opts, read)](#apidoc.element.mississippi.from.from)
1.  [function <span class="apidocSignatureSpan">mississippi.from.</span>ctor (opts, read)](#apidoc.element.mississippi.from.ctor)
1.  [function <span class="apidocSignatureSpan">mississippi.from.</span>obj (opts, read)](#apidoc.element.mississippi.from.obj)

#### [module mississippi.pipeline](#apidoc.module.mississippi.pipeline)
1.  [function <span class="apidocSignatureSpan">mississippi.</span>pipeline ()](#apidoc.element.mississippi.pipeline.pipeline)
1.  [function <span class="apidocSignatureSpan">mississippi.pipeline.</span>obj ()](#apidoc.element.mississippi.pipeline.obj)
1.  [function <span class="apidocSignatureSpan">mississippi.pipeline.</span>super_ (writable, readable, opts)](#apidoc.element.mississippi.pipeline.super_)

#### [module mississippi.pipeline.obj](#apidoc.module.mississippi.pipeline.obj)
1.  [function <span class="apidocSignatureSpan">mississippi.pipeline.</span>obj ()](#apidoc.element.mississippi.pipeline.obj.obj)
1.  [function <span class="apidocSignatureSpan">mississippi.pipeline.obj.</span>super_ (writable, readable, opts)](#apidoc.element.mississippi.pipeline.obj.super_)

#### [module mississippi.pipeline.obj.prototype](#apidoc.module.mississippi.pipeline.obj.prototype)
1.  [function <span class="apidocSignatureSpan">mississippi.pipeline.obj.prototype.</span>setPipeline ()](#apidoc.element.mississippi.pipeline.obj.prototype.setPipeline)

#### [module mississippi.pipeline.prototype](#apidoc.module.mississippi.pipeline.prototype)
1.  [function <span class="apidocSignatureSpan">mississippi.pipeline.prototype.</span>setPipeline ()](#apidoc.element.mississippi.pipeline.prototype.setPipeline)

#### [module mississippi.through](#apidoc.module.mississippi.through)
1.  [function <span class="apidocSignatureSpan">mississippi.</span>through (options, transform, flush)](#apidoc.element.mississippi.through.through)
1.  [function <span class="apidocSignatureSpan">mississippi.through.</span>ctor (options, transform, flush)](#apidoc.element.mississippi.through.ctor)
1.  [function <span class="apidocSignatureSpan">mississippi.through.</span>obj (options, transform, flush)](#apidoc.element.mississippi.through.obj)

#### [module mississippi.to](#apidoc.module.mississippi.to)
1.  [function <span class="apidocSignatureSpan">mississippi.</span>to (opts, write, flush)](#apidoc.element.mississippi.to.to)
1.  [function <span class="apidocSignatureSpan">mississippi.to.</span>obj (opts, worker, flush)](#apidoc.element.mississippi.to.obj)
1.  [function <span class="apidocSignatureSpan">mississippi.to.</span>super_ (options)](#apidoc.element.mississippi.to.super_)

#### [module mississippi.to.prototype](#apidoc.module.mississippi.to.prototype)
1.  [function <span class="apidocSignatureSpan">mississippi.to.prototype.</span>_write (data, enc, cb)](#apidoc.element.mississippi.to.prototype._write)
1.  [function <span class="apidocSignatureSpan">mississippi.to.prototype.</span>destroy (err)](#apidoc.element.mississippi.to.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">mississippi.to.prototype.</span>end (data, enc, cb)](#apidoc.element.mississippi.to.prototype.end)



# <a name="apidoc.module.mississippi"></a>[module mississippi](#apidoc.module.mississippi)

#### <a name="apidoc.element.mississippi.concat"></a>[function <span class="apidocSignatureSpan">mississippi.</span>concat (opts, cb)](#apidoc.element.mississippi.concat)
- description and source-code
```javascript
function ConcatStream(opts, cb) {
  if (!(this instanceof ConcatStream)) return new ConcatStream(opts, cb)

  if (typeof opts === 'function') {
    cb = opts
    opts = {}
  }
  if (!opts) opts = {}

  var encoding = opts.encoding
  var shouldInferEncoding = false

  if (!encoding) {
    shouldInferEncoding = true
  } else {
    encoding =  String(encoding).toLowerCase()
    if (encoding === 'u8' || encoding === 'uint8') {
      encoding = 'uint8array'
    }
  }

  Writable.call(this, { objectMode: true })

  this.encoding = encoding
  this.shouldInferEncoding = shouldInferEncoding

  if (cb) this.on('finish', function () { cb(this.getBody()) })
  this.body = []
}
```
- example usage
```shell
...
writing world
(nothing happens for 1 sec)
finished
'''

### concat

#####'var concat = miss.concat(cb)'

Returns a writable stream that concatenates all data written to the stream and calls a callback with the single result.

Calling 'miss.concat(cb)' returns a writable stream. 'cb' is called when the writable stream is finished, e.g. when all data is
done being written to it. 'cb' is called with a single argument, '(data)', which will contain the result of concatenating all the
 data written to the stream.

Note that 'miss.concat' will not handle stream errors for you. To handle errors, use 'miss.pipe' or handle the 'error' event manually
.
...
```

#### <a name="apidoc.element.mississippi.concat.super_"></a>[function <span class="apidocSignatureSpan">mississippi.</span>concat.super_ (options)](#apidoc.element.mississippi.concat.super_)
- description and source-code
```javascript
function Writable(options) {
  Duplex = Duplex || require('./_stream_duplex');

  // Writable ctor is applied to Duplexes, too.
  // 'realHasInstance' is necessary because using plain 'instanceof'
  // would return false, as no '_writableState' property is attached.

  // Trying to use the custom 'instanceof' for Writable here will also break the
  // Node.js LazyTransform implementation, which has a non-trivial getter for
  // '_writableState' that would lead to infinite recursion.
  if (!realHasInstance.call(Writable, this) && !(this instanceof Duplex)) {
    return new Writable(options);
  }

  this._writableState = new WritableState(options, this);

  // legacy.
  this.writable = true;

  if (options) {
    if (typeof options.write === 'function') this._write = options.write;

    if (typeof options.writev === 'function') this._writev = options.writev;
  }

  Stream.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.duplex"></a>[function <span class="apidocSignatureSpan">mississippi.</span>duplex (writable, readable, opts)](#apidoc.element.mississippi.duplex)
- description and source-code
```javascript
duplex = function (writable, readable, opts) {
  if (!(this instanceof Duplexify)) return new Duplexify(writable, readable, opts)
  stream.Duplex.call(this, opts)

  this._writable = null
  this._readable = null
  this._readable2 = null

  this._forwardDestroy = !opts || opts.destroy !== false
  this._forwardEnd = !opts || opts.end !== false
  this._corked = 1 // start corked
  this._ondrain = null
  this._drained = false
  this._forwarding = false
  this._unwrite = null
  this._unread = null
  this._ended = false

  this.destroyed = false

  if (writable) this.setWritable(writable)
  if (readable) this.setReadable(readable)
}
```
- example usage
```shell
...
  if (err) return console.error('Image processing error!', err)
  console.log('Image processed successfully')
})
'''

### duplex

##### 'var duplex = miss.duplex([writable, readable, opts])'

Take two separate streams, a writable and a readable, and turn them into a single [duplex (readable and writable) stream](https://
nodejs.org/api/stream.html#stream_class_stream_duplex).

The returned stream will emit data from the readable. When you write to it it writes to the writable.

You can either choose to supply the writable and the readable at the time you create the stream, or you can do it later using the
 '.setWritable' and '.setReadable' methods and data written to the stream in the meantime will be buffered for you.
...
```

#### <a name="apidoc.element.mississippi.duplex.super_"></a>[function <span class="apidocSignatureSpan">mississippi.</span>duplex.super_ (options)](#apidoc.element.mississippi.duplex.super_)
- description and source-code
```javascript
function Duplex(options) {
  if (!(this instanceof Duplex)) return new Duplex(options);

  Readable.call(this, options);
  Writable.call(this, options);

  if (options && options.readable === false) this.readable = false;

  if (options && options.writable === false) this.writable = false;

  this.allowHalfOpen = true;
  if (options && options.allowHalfOpen === false) this.allowHalfOpen = false;

  this.once('end', onend);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.each"></a>[function <span class="apidocSignatureSpan">mississippi.</span>each (stream, fn, cb)](#apidoc.element.mississippi.each)
- description and source-code
```javascript
function each(stream, fn, cb) {
  var want = true
  var error = null
  var ended = false
  var running = false

  stream.on('readable', onreadable)
  onreadable()

  if (cb) eos(stream, {readable: true, writable: false}, done)
  return stream

  function done (err) {
    if (!error) error = err
    ended = true
    if (!running) cb(error)
  }

  function onreadable () {
    if (want) read()
  }

  function afterRead (err) {
    running = false

    if (err) {
      error = err
      if (ended) return cb(error)
      stream.destroy(err)
      return
    }
    if (ended) return cb(error)
    read()
  }

  function read () {
    if (ended || running) return
    want = false

    var data = shift(stream)
    if (!data) {
      want = true
      return
    }

    running = true
    fn(data, afterRead)
  }
}
```
- example usage
```shell
...
  if (err) return console.error('Copy error!', err)
  console.log('Copied successfully')
})
'''

### each

##### 'miss.each(stream, each, [done])'

Iterate the data in 'stream' one chunk at a time. Your 'each' function will be called with '(data, next)' where data is a data chunk
 and next is a callback. Call 'next' when you are ready to consume the next chunk.

Optionally you can call 'next' with an error to destroy the stream. You can also pass the optional third argument, 'done', which
 is a function that will be called with '(err)' when the stream ends. The 'err' argument will be populated with an error if the
stream emitted an error.

#### original module
...
```

#### <a name="apidoc.element.mississippi.finished"></a>[function <span class="apidocSignatureSpan">mississippi.</span>finished (stream, opts, callback)](#apidoc.element.mississippi.finished)
- description and source-code
```javascript
finished = function (stream, opts, callback) {
	if (typeof opts === 'function') return eos(stream, null, opts);
	if (!opts) opts = {};

	callback = once(callback || noop);

	var ws = stream._writableState;
	var rs = stream._readableState;
	var readable = opts.readable || (opts.readable !== false && stream.readable);
	var writable = opts.writable || (opts.writable !== false && stream.writable);

	var onlegacyfinish = function() {
		if (!stream.writable) onfinish();
	};

	var onfinish = function() {
		writable = false;
		if (!readable) callback.call(stream);
	};

	var onend = function() {
		readable = false;
		if (!writable) callback.call(stream);
	};

	var onexit = function(exitCode) {
		callback.call(stream, exitCode ? new Error('exited with error code: ' + exitCode) : null);
	};

	var onclose = function() {
		if (readable && !(rs && rs.ended)) return callback.call(stream, new Error('premature close'));
		if (writable && !(ws && ws.ended)) return callback.call(stream, new Error('premature close'));
	};

	var onrequest = function() {
		stream.req.on('finish', onfinish);
	};

	if (isRequest(stream)) {
		stream.on('complete', onfinish);
		stream.on('abort', onclose);
		if (stream.req) onrequest();
		else stream.on('request', onrequest);
	} else if (writable && !ws) { // legacy streams
		stream.on('end', onlegacyfinish);
		stream.on('close', onlegacyfinish);
	}

	if (isChildProcess(stream)) stream.on('exit', onexit);

	stream.on('end', onend);
	stream.on('finish', onfinish);
	if (opts.error !== false) stream.on('error', callback);
	stream.on('close', onclose);

	return function() {
		stream.removeListener('complete', onfinish);
		stream.removeListener('abort', onclose);
		stream.removeListener('request', onrequest);
		if (stream.req) stream.req.removeListener('finish', onfinish);
		stream.removeListener('end', onlegacyfinish);
		stream.removeListener('close', onlegacyfinish);
		stream.removeListener('finish', onfinish);
		stream.removeListener('exit', onexit);
		stream.removeListener('end', onend);
		stream.removeListener('error', callback);
		stream.removeListener('close', onclose);
	};
}
```
- example usage
```shell
...
  console.error(err) // print the error to STDERR
  process.exit(1) // exit program with non-zero exit code
}
'''

### finished

#####'miss.finished(stream, cb)'

Waits for 'stream' to finish or error and then calls 'cb' with '(err)'. 'cb' will only be called once. 'err' will be null if the
 stream finished without error, or else it will be populated with the error from the streams 'error' event.

This function is useful for simplifying stream handling code as it lets you handle success or error conditions in a single code
path. It's used internally 'miss.pipe'.

#### original module
...
```

#### <a name="apidoc.element.mississippi.from"></a>[function <span class="apidocSignatureSpan">mississippi.</span>from (opts, read)](#apidoc.element.mississippi.from)
- description and source-code
```javascript
function from2(opts, read) {
  if (typeof opts !== 'object' || Array.isArray(opts)) {
    read = opts
    opts = {}
  }

  var rs = new Proto(opts)
  rs._from = Array.isArray(read) ? toFunction(read) : (read || noop)
  return rs
}
```
- example usage
```shell
...
  if (err) return console.error('Trouble uppercasing!')
  console.log('Splendid uppercasing!')
})
'''

### from

#####'miss.from([opts], read)'

Make a custom [readable stream](https://nodejs.org/docs/latest/api/stream.html#stream_class_stream_readable).

'opts' contains the options to pass on to the ReadableStream constructor e.g. for creating a readable object stream (or use the
shortcut 'miss.from.obj([...])').

Returns a readable stream that calls 'read(size, next)' when data is requested from the stream.
...
```

#### <a name="apidoc.element.mississippi.pipe"></a>[function <span class="apidocSignatureSpan">mississippi.</span>pipe ()](#apidoc.element.mississippi.pipe)
- description and source-code
```javascript
pipe = function () {
  var streams = Array.prototype.slice.call(arguments)
  var callback = isFn(streams[streams.length - 1] || noop) && streams.pop() || noop

  if (Array.isArray(streams[0])) streams = streams[0]
  if (streams.length < 2) throw new Error('pump requires two streams per minimum')

  var error
  var destroys = streams.map(function (stream, i) {
    var reading = i < streams.length - 1
    var writing = i > 0
    return destroyer(stream, reading, writing, function (err) {
      if (!error) error = err
      if (err) destroys.forEach(call)
      if (reading) return
      destroys.forEach(call)
      callback(error)
    })
  })

  return streams.reduce(pipe)
}
```
- example usage
```shell
...
- [to](#to)
- [concat](#concat)
- [finished](#finished)
- [parallel](#parallel)

### pipe

##### 'miss.pipe(stream1, stream2, stream3, ..., cb)'

Pipes streams together and destroys all of them if one of them closes. Calls 'cb' with '(error)' if there was an error in any of
 the streams.

When using standard 'source.pipe(destination)' the source will _not_ be destroyed if the destination emits close or error. You are
 also not able to provide a callback to tell when the pipe has finished.

'miss.pipe' does these two things for you, ensuring you handle stream errors 100% of the time (unhandled errors are probably the
 most common bug in most node streams code)
...
```

#### <a name="apidoc.element.mississippi.pipeline"></a>[function <span class="apidocSignatureSpan">mississippi.</span>pipeline ()](#apidoc.element.mississippi.pipeline)
- description and source-code
```javascript
pipeline = function () {
  var streams = toArray(arguments)
  if (!(this instanceof Pumpify)) return new Pumpify(streams)
  Duplexify.call(this, null, null, opts)
  if (streams.length) this.setPipeline(streams)
}
```
- example usage
```shell
...

'''js
var fs = require('fs')
var split = require('split2')

var newLineSeparatedNumbers = fs.createReadStream('numbers.txt')

var pipeline = miss.pipeline(newLineSeparatedNumbers, split())
var each = miss.each(pipeline, eachLine, done)
var sum = 0

function eachLine (line, next) {
  sum += parseInt(line.toString())
  next()
}
...
```

#### <a name="apidoc.element.mississippi.pipeline.obj"></a>[function <span class="apidocSignatureSpan">mississippi.</span>pipeline.obj ()](#apidoc.element.mississippi.pipeline.obj)
- description and source-code
```javascript
pipeline.obj = function () {
  var streams = toArray(arguments)
  if (!(this instanceof Pumpify)) return new Pumpify(streams)
  Duplexify.call(this, null, null, opts)
  if (streams.length) this.setPipeline(streams)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.through"></a>[function <span class="apidocSignatureSpan">mississippi.</span>through (options, transform, flush)](#apidoc.element.mississippi.through)
- description and source-code
```javascript
through = function (options, transform, flush) {
  if (typeof options == 'function') {
    flush     = transform
    transform = options
    options   = {}
  }

  if (typeof transform != 'function')
    transform = noop

  if (typeof flush != 'function')
    flush = null

  return construct(options, transform, flush)
}
```
- example usage
```shell
...

// duplexCurl will write to stdin and read from stdout
var duplexCurl = miss.duplex(curl.stdin, curl.stdout)
'''

### through

#####'var transformer = miss.through([options, transformFunction, flushFunction])'

Make a custom [transform stream](https://nodejs.org/docs/latest/api/stream.html#stream_class_stream_transform).

The 'options' object is passed to the internal transform stream and can be used to create an 'objectMode' stream (or use the shortcut
 'miss.through.obj([...])')

The 'transformFunction' is called when data is available for the writable side and has the signature '(chunk, encoding, cb)'. Within
 the function, add data to the readable side any number of times with 'this.push(data)'. Call 'cb()' to indicate processing of the
 'chunk' is complete. Or to easily emit a single error or chunk, call 'cb(err, chunk)'
...
```

#### <a name="apidoc.element.mississippi.to"></a>[function <span class="apidocSignatureSpan">mississippi.</span>to (opts, write, flush)](#apidoc.element.mississippi.to)
- description and source-code
```javascript
function WriteStream(opts, write, flush) {
  if (!(this instanceof WriteStream)) return new WriteStream(opts, write, flush)

  if (typeof opts === 'function') {
    flush = write
    write = opts
    opts = {}
  }

  stream.Writable.call(this, opts)

  this.destroyed = false
  this._worker = write || null
  this._flush = flush || null
}
```
- example usage
```shell
...
// pipe "hello world" out
// to stdout.
fromString('hello world').pipe(process.stdout)
'''

### to

#####'miss.to([options], write, [flush])'

Make a custom [writable stream](https://nodejs.org/docs/latest/api/stream.html#stream_class_stream_writable).

'opts' contains the options to pass on to the WritableStream constructor e.g. for creating a readable object stream (or use the
shortcut 'miss.to.obj([...])').

Returns a writable stream that calls 'write(data, enc, cb)' when data is written to the stream.
...
```



# <a name="apidoc.module.mississippi.concat"></a>[module mississippi.concat](#apidoc.module.mississippi.concat)

#### <a name="apidoc.element.mississippi.concat.concat"></a>[function <span class="apidocSignatureSpan">mississippi.</span>concat (opts, cb)](#apidoc.element.mississippi.concat.concat)
- description and source-code
```javascript
function ConcatStream(opts, cb) {
  if (!(this instanceof ConcatStream)) return new ConcatStream(opts, cb)

  if (typeof opts === 'function') {
    cb = opts
    opts = {}
  }
  if (!opts) opts = {}

  var encoding = opts.encoding
  var shouldInferEncoding = false

  if (!encoding) {
    shouldInferEncoding = true
  } else {
    encoding =  String(encoding).toLowerCase()
    if (encoding === 'u8' || encoding === 'uint8') {
      encoding = 'uint8array'
    }
  }

  Writable.call(this, { objectMode: true })

  this.encoding = encoding
  this.shouldInferEncoding = shouldInferEncoding

  if (cb) this.on('finish', function () { cb(this.getBody()) })
  this.body = []
}
```
- example usage
```shell
...
writing world
(nothing happens for 1 sec)
finished
'''

### concat

#####'var concat = miss.concat(cb)'

Returns a writable stream that concatenates all data written to the stream and calls a callback with the single result.

Calling 'miss.concat(cb)' returns a writable stream. 'cb' is called when the writable stream is finished, e.g. when all data is
done being written to it. 'cb' is called with a single argument, '(data)', which will contain the result of concatenating all the
 data written to the stream.

Note that 'miss.concat' will not handle stream errors for you. To handle errors, use 'miss.pipe' or handle the 'error' event manually
.
...
```

#### <a name="apidoc.element.mississippi.concat.super_"></a>[function <span class="apidocSignatureSpan">mississippi.concat.</span>super_ (options)](#apidoc.element.mississippi.concat.super_)
- description and source-code
```javascript
function Writable(options) {
  Duplex = Duplex || require('./_stream_duplex');

  // Writable ctor is applied to Duplexes, too.
  // 'realHasInstance' is necessary because using plain 'instanceof'
  // would return false, as no '_writableState' property is attached.

  // Trying to use the custom 'instanceof' for Writable here will also break the
  // Node.js LazyTransform implementation, which has a non-trivial getter for
  // '_writableState' that would lead to infinite recursion.
  if (!realHasInstance.call(Writable, this) && !(this instanceof Duplex)) {
    return new Writable(options);
  }

  this._writableState = new WritableState(options, this);

  // legacy.
  this.writable = true;

  if (options) {
    if (typeof options.write === 'function') this._write = options.write;

    if (typeof options.writev === 'function') this._writev = options.writev;
  }

  Stream.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mississippi.concat.prototype"></a>[module mississippi.concat.prototype](#apidoc.module.mississippi.concat.prototype)

#### <a name="apidoc.element.mississippi.concat.prototype._write"></a>[function <span class="apidocSignatureSpan">mississippi.concat.prototype.</span>_write (chunk, enc, next)](#apidoc.element.mississippi.concat.prototype._write)
- description and source-code
```javascript
_write = function (chunk, enc, next) {
  this.body.push(chunk)
  next()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.concat.prototype.getBody"></a>[function <span class="apidocSignatureSpan">mississippi.concat.prototype.</span>getBody ()](#apidoc.element.mississippi.concat.prototype.getBody)
- description and source-code
```javascript
getBody = function () {
  if (!this.encoding && this.body.length === 0) return []
  if (this.shouldInferEncoding) this.encoding = this.inferEncoding()
  if (this.encoding === 'array') return arrayConcat(this.body)
  if (this.encoding === 'string') return stringConcat(this.body)
  if (this.encoding === 'buffer') return bufferConcat(this.body)
  if (this.encoding === 'uint8array') return u8Concat(this.body)
  return this.body
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.concat.prototype.inferEncoding"></a>[function <span class="apidocSignatureSpan">mississippi.concat.prototype.</span>inferEncoding (buff)](#apidoc.element.mississippi.concat.prototype.inferEncoding)
- description and source-code
```javascript
inferEncoding = function (buff) {
  var firstBuffer = buff === undefined ? this.body[0] : buff;
  if (Buffer.isBuffer(firstBuffer)) return 'buffer'
  if (typeof Uint8Array !== 'undefined' && firstBuffer instanceof Uint8Array) return 'uint8array'
  if (Array.isArray(firstBuffer)) return 'array'
  if (typeof firstBuffer === 'string') return 'string'
  if (Object.prototype.toString.call(firstBuffer) === "[object Object]") return 'object'
  return 'buffer'
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mississippi.concat.super_"></a>[module mississippi.concat.super_](#apidoc.module.mississippi.concat.super_)

#### <a name="apidoc.element.mississippi.concat.super_.super_"></a>[function <span class="apidocSignatureSpan">mississippi.concat.</span>super_ ()](#apidoc.element.mississippi.concat.super_.super_)
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

#### <a name="apidoc.element.mississippi.concat.super_.WritableState"></a>[function <span class="apidocSignatureSpan">mississippi.concat.super_.</span>WritableState (options, stream)](#apidoc.element.mississippi.concat.super_.WritableState)
- description and source-code
```javascript
function WritableState(options, stream) {
  Duplex = Duplex || require('./_stream_duplex');

  options = options || {};

  // object stream flag to indicate whether or not this stream
  // contains buffers or objects.
  this.objectMode = !!options.objectMode;

  if (stream instanceof Duplex) this.objectMode = this.objectMode || !!options.writableObjectMode;

  // the point at which write() starts returning false
  // Note: 0 is a valid value, means that we always return false if
  // the entire buffer is not flushed immediately on write()
  var hwm = options.highWaterMark;
  var defaultHwm = this.objectMode ? 16 : 16 * 1024;
  this.highWaterMark = hwm || hwm === 0 ? hwm : defaultHwm;

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
  this.onwrite = function (er) {
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



# <a name="apidoc.module.mississippi.concat.super_.WritableState.prototype"></a>[module mississippi.concat.super_.WritableState.prototype](#apidoc.module.mississippi.concat.super_.WritableState.prototype)

#### <a name="apidoc.element.mississippi.concat.super_.WritableState.prototype.getBuffer"></a>[function <span class="apidocSignatureSpan">mississippi.concat.super_.WritableState.prototype.</span>getBuffer ()](#apidoc.element.mississippi.concat.super_.WritableState.prototype.getBuffer)
- description and source-code
```javascript
function getBuffer() {
  var current = this.bufferedRequest;
  var out = [];
  while (current) {
    out.push(current);
    current = current.next;
  }
  return out;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mississippi.concat.super_.prototype"></a>[module mississippi.concat.super_.prototype](#apidoc.module.mississippi.concat.super_.prototype)

#### <a name="apidoc.element.mississippi.concat.super_.prototype._write"></a>[function <span class="apidocSignatureSpan">mississippi.concat.super_.prototype.</span>_write (chunk, encoding, cb)](#apidoc.element.mississippi.concat.super_.prototype._write)
- description and source-code
```javascript
_write = function (chunk, encoding, cb) {
  cb(new Error('_write() is not implemented'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.concat.super_.prototype.cork"></a>[function <span class="apidocSignatureSpan">mississippi.concat.super_.prototype.</span>cork ()](#apidoc.element.mississippi.concat.super_.prototype.cork)
- description and source-code
```javascript
cork = function () {
  var state = this._writableState;

  state.corked++;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.concat.super_.prototype.end"></a>[function <span class="apidocSignatureSpan">mississippi.concat.super_.prototype.</span>end (chunk, encoding, cb)](#apidoc.element.mississippi.concat.super_.prototype.end)
- description and source-code
```javascript
end = function (chunk, encoding, cb) {
  var state = this._writableState;

  if (typeof chunk === 'function') {
    cb = chunk;
    chunk = null;
    encoding = null;
  } else if (typeof encoding === 'function') {
    cb = encoding;
    encoding = null;
  }

  if (chunk !== null && chunk !== undefined) this.write(chunk, encoding);

  // .end() fully uncorks
  if (state.corked) {
    state.corked = 1;
    this.uncork();
  }

  // ignore unnecessary end() calls.
  if (!state.ending && !state.finished) endWritable(this, state, cb);
}
```
- example usage
```shell
...

ws.on('finish', function () {
  console.log('finished')
})

ws.write('hello')
ws.write('world')
ws.end()

function write (data, enc, cb) {
  // i am your normal ._write method
  console.log('writing', data.toString())
  cb()
}
...
```

#### <a name="apidoc.element.mississippi.concat.super_.prototype.pipe"></a>[function <span class="apidocSignatureSpan">mississippi.concat.super_.prototype.</span>pipe ()](#apidoc.element.mississippi.concat.super_.prototype.pipe)
- description and source-code
```javascript
pipe = function () {
  this.emit('error', new Error('Cannot pipe, not readable'));
}
```
- example usage
```shell
...
- [to](#to)
- [concat](#concat)
- [finished](#finished)
- [parallel](#parallel)

### pipe

##### 'miss.pipe(stream1, stream2, stream3, ..., cb)'

Pipes streams together and destroys all of them if one of them closes. Calls 'cb' with '(error)' if there was an error in any of
 the streams.

When using standard 'source.pipe(destination)' the source will _not_ be destroyed if the destination emits close or error. You are
 also not able to provide a callback to tell when the pipe has finished.

'miss.pipe' does these two things for you, ensuring you handle stream errors 100% of the time (unhandled errors are probably the
 most common bug in most node streams code)
...
```

#### <a name="apidoc.element.mississippi.concat.super_.prototype.setDefaultEncoding"></a>[function <span class="apidocSignatureSpan">mississippi.concat.super_.prototype.</span>setDefaultEncoding (encoding)](#apidoc.element.mississippi.concat.super_.prototype.setDefaultEncoding)
- description and source-code
```javascript
function setDefaultEncoding(encoding) {
  // node::ParseEncoding() requires lower case.
  if (typeof encoding === 'string') encoding = encoding.toLowerCase();
  if (!(['hex', 'utf8', 'utf-8', 'ascii', 'binary', 'base64', 'ucs2', 'ucs-2', 'utf16le', 'utf-16le', 'raw'].indexOf((encoding + '').
toLowerCase()) > -1)) throw new TypeError('Unknown encoding: ' + encoding);
  this._writableState.defaultEncoding = encoding;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.concat.super_.prototype.uncork"></a>[function <span class="apidocSignatureSpan">mississippi.concat.super_.prototype.</span>uncork ()](#apidoc.element.mississippi.concat.super_.prototype.uncork)
- description and source-code
```javascript
uncork = function () {
  var state = this._writableState;

  if (state.corked) {
    state.corked--;

    if (!state.writing && !state.corked && !state.finished && !state.bufferProcessing && state.bufferedRequest) clearBuffer(this
, state);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.concat.super_.prototype.write"></a>[function <span class="apidocSignatureSpan">mississippi.concat.super_.prototype.</span>write (chunk, encoding, cb)](#apidoc.element.mississippi.concat.super_.prototype.write)
- description and source-code
```javascript
write = function (chunk, encoding, cb) {
  var state = this._writableState;
  var ret = false;
  var isBuf = Buffer.isBuffer(chunk);

  if (typeof encoding === 'function') {
    cb = encoding;
    encoding = null;
  }

  if (isBuf) encoding = 'buffer';else if (!encoding) encoding = state.defaultEncoding;

  if (typeof cb !== 'function') cb = nop;

  if (state.ended) writeAfterEnd(this, cb);else if (isBuf || validChunk(this, state, chunk, cb)) {
    state.pendingcb++;
    ret = writeOrBuffer(this, state, isBuf, chunk, encoding, cb);
  }

  return ret;
}
```
- example usage
```shell
...
'''js
var ws = miss.to(write, flush)

ws.on('finish', function () {
console.log('finished')
})

ws.write('hello')
ws.write('world')
ws.end()

function write (data, enc, cb) {
// i am your normal ._write method
console.log('writing', data.toString())
cb()
...
```



# <a name="apidoc.module.mississippi.duplex"></a>[module mississippi.duplex](#apidoc.module.mississippi.duplex)

#### <a name="apidoc.element.mississippi.duplex.duplex"></a>[function <span class="apidocSignatureSpan">mississippi.</span>duplex (writable, readable, opts)](#apidoc.element.mississippi.duplex.duplex)
- description and source-code
```javascript
duplex = function (writable, readable, opts) {
  if (!(this instanceof Duplexify)) return new Duplexify(writable, readable, opts)
  stream.Duplex.call(this, opts)

  this._writable = null
  this._readable = null
  this._readable2 = null

  this._forwardDestroy = !opts || opts.destroy !== false
  this._forwardEnd = !opts || opts.end !== false
  this._corked = 1 // start corked
  this._ondrain = null
  this._drained = false
  this._forwarding = false
  this._unwrite = null
  this._unread = null
  this._ended = false

  this.destroyed = false

  if (writable) this.setWritable(writable)
  if (readable) this.setReadable(readable)
}
```
- example usage
```shell
...
  if (err) return console.error('Image processing error!', err)
  console.log('Image processed successfully')
})
'''

### duplex

##### 'var duplex = miss.duplex([writable, readable, opts])'

Take two separate streams, a writable and a readable, and turn them into a single [duplex (readable and writable) stream](https://
nodejs.org/api/stream.html#stream_class_stream_duplex).

The returned stream will emit data from the readable. When you write to it it writes to the writable.

You can either choose to supply the writable and the readable at the time you create the stream, or you can do it later using the
 '.setWritable' and '.setReadable' methods and data written to the stream in the meantime will be buffered for you.
...
```

#### <a name="apidoc.element.mississippi.duplex.obj"></a>[function <span class="apidocSignatureSpan">mississippi.duplex.</span>obj (writable, readable, opts)](#apidoc.element.mississippi.duplex.obj)
- description and source-code
```javascript
obj = function (writable, readable, opts) {
  if (!opts) opts = {}
  opts.objectMode = true
  opts.highWaterMark = 16
  return new Duplexify(writable, readable, opts)
}
```
- example usage
```shell
...

### through

#####'var transformer = miss.through([options, transformFunction, flushFunction])'

Make a custom [transform stream](https://nodejs.org/docs/latest/api/stream.html#stream_class_stream_transform).

The 'options' object is passed to the internal transform stream and can be used to create an 'objectMode' stream (or use the shortcut
 'miss.through.obj([...])')

The 'transformFunction' is called when data is available for the writable side and has the signature '(chunk, encoding, cb)'. Within
 the function, add data to the readable side any number of times with 'this.push(data)'. Call 'cb()' to indicate processing of the
 'chunk' is complete. Or to easily emit a single error or chunk, call 'cb(err, chunk)'

The 'flushFunction', with signature '(cb)', is called just before the stream is complete and should be used to wrap up stream processing
.

#### original module
...
```

#### <a name="apidoc.element.mississippi.duplex.super_"></a>[function <span class="apidocSignatureSpan">mississippi.duplex.</span>super_ (options)](#apidoc.element.mississippi.duplex.super_)
- description and source-code
```javascript
function Duplex(options) {
  if (!(this instanceof Duplex)) return new Duplex(options);

  Readable.call(this, options);
  Writable.call(this, options);

  if (options && options.readable === false) this.readable = false;

  if (options && options.writable === false) this.writable = false;

  this.allowHalfOpen = true;
  if (options && options.allowHalfOpen === false) this.allowHalfOpen = false;

  this.once('end', onend);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mississippi.duplex.prototype"></a>[module mississippi.duplex.prototype](#apidoc.module.mississippi.duplex.prototype)

#### <a name="apidoc.element.mississippi.duplex.prototype._destroy"></a>[function <span class="apidocSignatureSpan">mississippi.duplex.prototype.</span>_destroy (err)](#apidoc.element.mississippi.duplex.prototype._destroy)
- description and source-code
```javascript
_destroy = function (err) {
  if (err) {
    var ondrain = this._ondrain
    this._ondrain = null
    if (ondrain) ondrain(err)
    else this.emit('error', err)
  }

  if (this._forwardDestroy) {
    if (this._readable && this._readable.destroy) this._readable.destroy()
    if (this._writable && this._writable.destroy) this._writable.destroy()
  }

  this.emit('close')
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.duplex.prototype._finish"></a>[function <span class="apidocSignatureSpan">mississippi.duplex.prototype.</span>_finish (cb)](#apidoc.element.mississippi.duplex.prototype._finish)
- description and source-code
```javascript
_finish = function (cb) {
  var self = this
  this.emit('preend')
  onuncork(this, function() {
    end(self._forwardEnd && self._writable, function() {
      // haxx to not emit prefinish twice
      if (self._writableState.prefinished === false) self._writableState.prefinished = true
      self.emit('prefinish')
      onuncork(self, cb)
    })
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.duplex.prototype._forward"></a>[function <span class="apidocSignatureSpan">mississippi.duplex.prototype.</span>_forward ()](#apidoc.element.mississippi.duplex.prototype._forward)
- description and source-code
```javascript
_forward = function () {
  if (this._forwarding || !this._readable2 || !this._drained) return
  this._forwarding = true

  var data

  while (this._drained && (data = shift(this._readable2)) !== null) {
    if (this.destroyed) continue
    this._drained = this.push(data)
  }

  this._forwarding = false
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.duplex.prototype._read"></a>[function <span class="apidocSignatureSpan">mississippi.duplex.prototype.</span>_read ()](#apidoc.element.mississippi.duplex.prototype._read)
- description and source-code
```javascript
_read = function () {
  this._drained = true
  this._forward()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.duplex.prototype._write"></a>[function <span class="apidocSignatureSpan">mississippi.duplex.prototype.</span>_write (data, enc, cb)](#apidoc.element.mississippi.duplex.prototype._write)
- description and source-code
```javascript
_write = function (data, enc, cb) {
  if (this.destroyed) return cb()
  if (this._corked) return onuncork(this, this._write.bind(this, data, enc, cb))
  if (data === SIGNAL_FLUSH) return this._finish(cb)
  if (!this._writable) return cb()

  if (this._writable.write(data) === false) this._ondrain = cb
  else cb()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.duplex.prototype.cork"></a>[function <span class="apidocSignatureSpan">mississippi.duplex.prototype.</span>cork ()](#apidoc.element.mississippi.duplex.prototype.cork)
- description and source-code
```javascript
cork = function () {
  if (++this._corked === 1) this.emit('cork')
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.duplex.prototype.destroy"></a>[function <span class="apidocSignatureSpan">mississippi.duplex.prototype.</span>destroy (err)](#apidoc.element.mississippi.duplex.prototype.destroy)
- description and source-code
```javascript
destroy = function (err) {
  if (this.destroyed) return
  this.destroyed = true

  var self = this
  process.nextTick(function() {
    self._destroy(err)
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.duplex.prototype.end"></a>[function <span class="apidocSignatureSpan">mississippi.duplex.prototype.</span>end (data, enc, cb)](#apidoc.element.mississippi.duplex.prototype.end)
- description and source-code
```javascript
end = function (data, enc, cb) {
  if (typeof data === 'function') return this.end(null, null, data)
  if (typeof enc === 'function') return this.end(data, null, enc)
  this._ended = true
  if (data) this.write(data)
  if (!this._writableState.ending) this.write(SIGNAL_FLUSH)
  return stream.Writable.prototype.end.call(this, cb)
}
```
- example usage
```shell
...

ws.on('finish', function () {
  console.log('finished')
})

ws.write('hello')
ws.write('world')
ws.end()

function write (data, enc, cb) {
  // i am your normal ._write method
  console.log('writing', data.toString())
  cb()
}
...
```

#### <a name="apidoc.element.mississippi.duplex.prototype.setReadable"></a>[function <span class="apidocSignatureSpan">mississippi.duplex.prototype.</span>setReadable (readable)](#apidoc.element.mississippi.duplex.prototype.setReadable)
- description and source-code
```javascript
setReadable = function (readable) {
  if (this._unread) this._unread()

  if (this.destroyed) {
    if (readable && readable.destroy) readable.destroy()
    return
  }

  if (readable === null || readable === false) {
    this.push(null)
    this.resume()
    return
  }

  var self = this
  var unend = eos(readable, {writable:false, readable:true}, destroyer(this))

  var onreadable = function() {
    self._forward()
  }

  var onend = function() {
    self.push(null)
  }

  var clear = function() {
    self._readable2.removeListener('readable', onreadable)
    self._readable2.removeListener('end', onend)
    unend()
  }

  this._drained = true
  this._readable = readable
  this._readable2 = readable._readableState ? readable : toStreams2(readable)
  this._readable2.on('readable', onreadable)
  this._readable2.on('end', onend)
  this._unread = clear

  this._forward()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.duplex.prototype.setWritable"></a>[function <span class="apidocSignatureSpan">mississippi.duplex.prototype.</span>setWritable (writable)](#apidoc.element.mississippi.duplex.prototype.setWritable)
- description and source-code
```javascript
setWritable = function (writable) {
  if (this._unwrite) this._unwrite()

  if (this.destroyed) {
    if (writable && writable.destroy) writable.destroy()
    return
  }

  if (writable === null || writable === false) {
    this.end()
    return
  }

  var self = this
  var unend = eos(writable, {writable:true, readable:false}, destroyer(this, this._forwardEnd))

  var ondrain = function() {
    var ondrain = self._ondrain
    self._ondrain = null
    if (ondrain) ondrain()
  }

  var clear = function() {
    self._writable.removeListener('drain', ondrain)
    unend()
  }

  if (this._unwrite) process.nextTick(ondrain) // force a drain on stream reset to avoid livelocks

  this._writable = writable
  this._writable.on('drain', ondrain)
  this._unwrite = clear

  this.uncork() // always uncork setWritable
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.duplex.prototype.uncork"></a>[function <span class="apidocSignatureSpan">mississippi.duplex.prototype.</span>uncork ()](#apidoc.element.mississippi.duplex.prototype.uncork)
- description and source-code
```javascript
uncork = function () {
  if (this._corked && --this._corked === 0) this.emit('uncork')
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mississippi.duplex.super_"></a>[module mississippi.duplex.super_](#apidoc.module.mississippi.duplex.super_)

#### <a name="apidoc.element.mississippi.duplex.super_.super_"></a>[function <span class="apidocSignatureSpan">mississippi.duplex.</span>super_ (options)](#apidoc.element.mississippi.duplex.super_.super_)
- description and source-code
```javascript
function Readable(options) {
  Duplex = Duplex || require('./_stream_duplex');

  if (!(this instanceof Readable)) return new Readable(options);

  this._readableState = new ReadableState(options, this);

  // legacy
  this.readable = true;

  if (options && typeof options.read === 'function') this._read = options.read;

  Stream.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mississippi.duplex.super_.prototype"></a>[module mississippi.duplex.super_.prototype](#apidoc.module.mississippi.duplex.super_.prototype)

#### <a name="apidoc.element.mississippi.duplex.super_.prototype._write"></a>[function <span class="apidocSignatureSpan">mississippi.duplex.super_.prototype.</span>_write (chunk, encoding, cb)](#apidoc.element.mississippi.duplex.super_.prototype._write)
- description and source-code
```javascript
_write = function (chunk, encoding, cb) {
  cb(new Error('_write() is not implemented'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.duplex.super_.prototype.cork"></a>[function <span class="apidocSignatureSpan">mississippi.duplex.super_.prototype.</span>cork ()](#apidoc.element.mississippi.duplex.super_.prototype.cork)
- description and source-code
```javascript
cork = function () {
  var state = this._writableState;

  state.corked++;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.duplex.super_.prototype.end"></a>[function <span class="apidocSignatureSpan">mississippi.duplex.super_.prototype.</span>end (chunk, encoding, cb)](#apidoc.element.mississippi.duplex.super_.prototype.end)
- description and source-code
```javascript
end = function (chunk, encoding, cb) {
  var state = this._writableState;

  if (typeof chunk === 'function') {
    cb = chunk;
    chunk = null;
    encoding = null;
  } else if (typeof encoding === 'function') {
    cb = encoding;
    encoding = null;
  }

  if (chunk !== null && chunk !== undefined) this.write(chunk, encoding);

  // .end() fully uncorks
  if (state.corked) {
    state.corked = 1;
    this.uncork();
  }

  // ignore unnecessary end() calls.
  if (!state.ending && !state.finished) endWritable(this, state, cb);
}
```
- example usage
```shell
...

ws.on('finish', function () {
  console.log('finished')
})

ws.write('hello')
ws.write('world')
ws.end()

function write (data, enc, cb) {
  // i am your normal ._write method
  console.log('writing', data.toString())
  cb()
}
...
```

#### <a name="apidoc.element.mississippi.duplex.super_.prototype.setDefaultEncoding"></a>[function <span class="apidocSignatureSpan">mississippi.duplex.super_.prototype.</span>setDefaultEncoding (encoding)](#apidoc.element.mississippi.duplex.super_.prototype.setDefaultEncoding)
- description and source-code
```javascript
function setDefaultEncoding(encoding) {
  // node::ParseEncoding() requires lower case.
  if (typeof encoding === 'string') encoding = encoding.toLowerCase();
  if (!(['hex', 'utf8', 'utf-8', 'ascii', 'binary', 'base64', 'ucs2', 'ucs-2', 'utf16le', 'utf-16le', 'raw'].indexOf((encoding + '').
toLowerCase()) > -1)) throw new TypeError('Unknown encoding: ' + encoding);
  this._writableState.defaultEncoding = encoding;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.duplex.super_.prototype.uncork"></a>[function <span class="apidocSignatureSpan">mississippi.duplex.super_.prototype.</span>uncork ()](#apidoc.element.mississippi.duplex.super_.prototype.uncork)
- description and source-code
```javascript
uncork = function () {
  var state = this._writableState;

  if (state.corked) {
    state.corked--;

    if (!state.writing && !state.corked && !state.finished && !state.bufferProcessing && state.bufferedRequest) clearBuffer(this
, state);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.duplex.super_.prototype.write"></a>[function <span class="apidocSignatureSpan">mississippi.duplex.super_.prototype.</span>write (chunk, encoding, cb)](#apidoc.element.mississippi.duplex.super_.prototype.write)
- description and source-code
```javascript
write = function (chunk, encoding, cb) {
  var state = this._writableState;
  var ret = false;
  var isBuf = Buffer.isBuffer(chunk);

  if (typeof encoding === 'function') {
    cb = encoding;
    encoding = null;
  }

  if (isBuf) encoding = 'buffer';else if (!encoding) encoding = state.defaultEncoding;

  if (typeof cb !== 'function') cb = nop;

  if (state.ended) writeAfterEnd(this, cb);else if (isBuf || validChunk(this, state, chunk, cb)) {
    state.pendingcb++;
    ret = writeOrBuffer(this, state, isBuf, chunk, encoding, cb);
  }

  return ret;
}
```
- example usage
```shell
...
'''js
var ws = miss.to(write, flush)

ws.on('finish', function () {
console.log('finished')
})

ws.write('hello')
ws.write('world')
ws.end()

function write (data, enc, cb) {
// i am your normal ._write method
console.log('writing', data.toString())
cb()
...
```



# <a name="apidoc.module.mississippi.duplex.super_.super_.prototype"></a>[module mississippi.duplex.super_.super_.prototype](#apidoc.module.mississippi.duplex.super_.super_.prototype)

#### <a name="apidoc.element.mississippi.duplex.super_.super_.prototype._read"></a>[function <span class="apidocSignatureSpan">mississippi.duplex.super_.super_.prototype.</span>_read (n)](#apidoc.element.mississippi.duplex.super_.super_.prototype._read)
- description and source-code
```javascript
_read = function (n) {
  this.emit('error', new Error('_read() is not implemented'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.duplex.super_.super_.prototype.addListener"></a>[function <span class="apidocSignatureSpan">mississippi.duplex.super_.super_.prototype.</span>addListener (ev, fn)](#apidoc.element.mississippi.duplex.super_.super_.prototype.addListener)
- description and source-code
```javascript
addListener = function (ev, fn) {
  var res = Stream.prototype.on.call(this, ev, fn);

  if (ev === 'data') {
    // Start flowing on next tick if stream isn't explicitly paused
    if (this._readableState.flowing !== false) this.resume();
  } else if (ev === 'readable') {
    var state = this._readableState;
    if (!state.endEmitted && !state.readableListening) {
      state.readableListening = state.needReadable = true;
      state.emittedReadable = false;
      if (!state.reading) {
        processNextTick(nReadingNextTick, this);
      } else if (state.length) {
        emitReadable(this, state);
      }
    }
  }

  return res;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.duplex.super_.super_.prototype.isPaused"></a>[function <span class="apidocSignatureSpan">mississippi.duplex.super_.super_.prototype.</span>isPaused ()](#apidoc.element.mississippi.duplex.super_.super_.prototype.isPaused)
- description and source-code
```javascript
isPaused = function () {
  return this._readableState.flowing === false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.duplex.super_.super_.prototype.on"></a>[function <span class="apidocSignatureSpan">mississippi.duplex.super_.super_.prototype.</span>on (ev, fn)](#apidoc.element.mississippi.duplex.super_.super_.prototype.on)
- description and source-code
```javascript
on = function (ev, fn) {
  var res = Stream.prototype.on.call(this, ev, fn);

  if (ev === 'data') {
    // Start flowing on next tick if stream isn't explicitly paused
    if (this._readableState.flowing !== false) this.resume();
  } else if (ev === 'readable') {
    var state = this._readableState;
    if (!state.endEmitted && !state.readableListening) {
      state.readableListening = state.needReadable = true;
      state.emittedReadable = false;
      if (!state.reading) {
        processNextTick(nReadingNextTick, this);
      } else if (state.length) {
        emitReadable(this, state);
      }
    }
  }

  return res;
}
```
- example usage
```shell
...
'miss.to' is provided by ['require('flush-write-stream')'](https://www.npmjs.com/package/flush-write-stream)

#### example

'''js
var ws = miss.to(write, flush)

ws.on('finish', function () {
  console.log('finished')
})

ws.write('hello')
ws.write('world')
ws.end()
...
```

#### <a name="apidoc.element.mississippi.duplex.super_.super_.prototype.pause"></a>[function <span class="apidocSignatureSpan">mississippi.duplex.super_.super_.prototype.</span>pause ()](#apidoc.element.mississippi.duplex.super_.super_.prototype.pause)
- description and source-code
```javascript
pause = function () {
  debug('call pause flowing=%j', this._readableState.flowing);
  if (false !== this._readableState.flowing) {
    debug('pause');
    this._readableState.flowing = false;
    this.emit('pause');
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.duplex.super_.super_.prototype.pipe"></a>[function <span class="apidocSignatureSpan">mississippi.duplex.super_.super_.prototype.</span>pipe (dest, pipeOpts)](#apidoc.element.mississippi.duplex.super_.super_.prototype.pipe)
- description and source-code
```javascript
pipe = function (dest, pipeOpts) {
  var src = this;
  var state = this._readableState;

  switch (state.pipesCount) {
    case 0:
      state.pipes = dest;
      break;
    case 1:
      state.pipes = [state.pipes, dest];
      break;
    default:
      state.pipes.push(dest);
      break;
  }
  state.pipesCount += 1;
  debug('pipe count=%d opts=%j', state.pipesCount, pipeOpts);

  var doEnd = (!pipeOpts || pipeOpts.end !== false) && dest !== process.stdout && dest !== process.stderr;

  var endFn = doEnd ? onend : cleanup;
  if (state.endEmitted) processNextTick(endFn);else src.once('end', endFn);

  dest.on('unpipe', onunpipe);
  function onunpipe(readable) {
    debug('onunpipe');
    if (readable === src) {
      cleanup();
    }
  }

  function onend() {
    debug('onend');
    dest.end();
  }

  // when the dest drains, it reduces the awaitDrain counter
  // on the source.  This would be more elegant with a .once()
  // handler in flow(), but adding and removing repeatedly is
  // too slow.
  var ondrain = pipeOnDrain(src);
  dest.on('drain', ondrain);

  var cleanedUp = false;
  function cleanup() {
    debug('cleanup');
    // cleanup event handlers once the pipe is broken
    dest.removeListener('close', onclose);
    dest.removeListener('finish', onfinish);
    dest.removeListener('drain', ondrain);
    dest.removeListener('error', onerror);
    dest.removeListener('unpipe', onunpipe);
    src.removeListener('end', onend);
    src.removeListener('end', cleanup);
    src.removeListener('data', ondata);

    cleanedUp = true;

    // if the reader is waiting for a drain event from this
    // specific writer, then it would cause it to never start
    // flowing again.
    // So, if this is awaiting a drain, then we just call it now.
    // If we don't know, then assume that we are waiting for one.
    if (state.awaitDrain && (!dest._writableState || dest._writableState.needDrain)) ondrain();
  }

  // If the user pushes more data while we're writing to dest then we'll end up
  // in ondata again. However, we only want to increase awaitDrain once because
  // dest will only emit one 'drain' event for the multiple writes.
  // => Introduce a guard on increasing awaitDrain.
  var increasedAwaitDrain = false;
  src.on('data', ondata);
  function ondata(chunk) {
    debug('ondata');
    increasedAwaitDrain = false;
    var ret = dest.write(chunk);
    if (false === ret && !increasedAwaitDrain) {
      // If the user unpiped during 'dest.write()', it is possible
      // to get stuck in a permanently paused state if that write
      // also returned false.
      // => Check whether 'dest' is still a piping destination.
      if ((state.pipesCount === 1 && state.pipes === dest || state.pipesCount > 1 && indexOf(state.pipes, dest) !== -1) && !cleanedUp
) {
        debug('false write response, pause', src._readableState.awaitDrain);
        src._readableState.awaitDrain++;
        increasedAwaitDrain = true;
      }
      src.pause();
    }
  }

  // if the dest has an error, then stop piping into it.
  // however, don't suppress the throwing behavior for this.
  function onerror(er) {
    debug('onerror', er);
    unpipe();
    dest.removeListener('error', onerror);
    if (EElistenerCount(dest, 'error') === 0) dest.emit('error', er);
  }

  // Make sure our error handler is attached before userland ones.
  prependListener(dest, 'error', onerror);

  // Both close and finish should trigger unpipe, but only once.
  function onclose() {
    dest.removeListener('finish', onfinish);
    unpipe();
  }
  dest.once('close', onclose);
  function onfinish() {
    debug('onfinish');
    dest.removeListener('close', onclose);
    unpipe();
  }
  dest.once('finish', onfinish);

  function unpipe() {
    debug('unpipe');
    src.unpipe(dest);
  }

  // tell the dest that it's being piped to
  dest.emit('pipe', src);

  // start the flow if it hasn't been started already.
  if (!state.flowing) {
    debug('pipe resume');
    src.resume();
  }

  return dest;
}
```
- example usage
```shell
...
- [to](#to)
- [concat](#concat)
- [finished](#finished)
- [parallel](#parallel)

### pipe

##### 'miss.pipe(stream1, stream2, stream3, ..., cb)'

Pipes streams together and destroys all of them if one of them closes. Calls 'cb' with '(error)' if there was an error in any of
 the streams.

When using standard 'source.pipe(destination)' the source will _not_ be destroyed if the destination emits close or error. You are
 also not able to provide a callback to tell when the pipe has finished.

'miss.pipe' does these two things for you, ensuring you handle stream errors 100% of the time (unhandled errors are probably the
 most common bug in most node streams code)
...
```

#### <a name="apidoc.element.mississippi.duplex.super_.super_.prototype.push"></a>[function <span class="apidocSignatureSpan">mississippi.duplex.super_.super_.prototype.</span>push (chunk, encoding)](#apidoc.element.mississippi.duplex.super_.super_.prototype.push)
- description and source-code
```javascript
push = function (chunk, encoding) {
  var state = this._readableState;

  if (!state.objectMode && typeof chunk === 'string') {
    encoding = encoding || state.defaultEncoding;
    if (encoding !== state.encoding) {
      chunk = bufferShim.from(chunk, encoding);
      encoding = '';
    }
  }

  return readableAddChunk(this, state, chunk, encoding, false);
}
```
- example usage
```shell
...

#####'var transformer = miss.through([options, transformFunction, flushFunction])'

Make a custom [transform stream](https://nodejs.org/docs/latest/api/stream.html#stream_class_stream_transform).

The 'options' object is passed to the internal transform stream and can be used to create an 'objectMode' stream (or use the shortcut
 'miss.through.obj([...])')

The 'transformFunction' is called when data is available for the writable side and has the signature '(chunk, encoding, cb)'. Within
 the function, add data to the readable side any number of times with 'this.push(data)'. Call 'cb()' to indicate processing of the
 'chunk' is complete. Or to easily emit a single error or chunk, call 'cb(err, chunk)'

The 'flushFunction', with signature '(cb)', is called just before the stream is complete and should be used to wrap up stream processing
.

#### original module

'miss.through' is provided by ['require('through2')'](https://www.npmjs.com/package/through2)
...
```

#### <a name="apidoc.element.mississippi.duplex.super_.super_.prototype.read"></a>[function <span class="apidocSignatureSpan">mississippi.duplex.super_.super_.prototype.</span>read (n)](#apidoc.element.mississippi.duplex.super_.super_.prototype.read)
- description and source-code
```javascript
read = function (n) {
  debug('read', n);
  n = parseInt(n, 10);
  var state = this._readableState;
  var nOrig = n;

  if (n !== 0) state.emittedReadable = false;

  // if we're doing read(0) to trigger a readable event, but we
  // already have a bunch of data in the buffer, then just trigger
  // the 'readable' event and move on.
  if (n === 0 && state.needReadable && (state.length >= state.highWaterMark || state.ended)) {
    debug('read: emitReadable', state.length, state.ended);
    if (state.length === 0 && state.ended) endReadable(this);else emitReadable(this);
    return null;
  }

  n = howMuchToRead(n, state);

  // if we've ended, and we're now clear, then finish it up.
  if (n === 0 && state.ended) {
    if (state.length === 0) endReadable(this);
    return null;
  }

  // All the actual chunk generation logic needs to be
  // *below* the call to _read.  The reason is that in certain
  // synthetic stream cases, such as passthrough streams, _read
  // may be a completely synchronous operation which may change
  // the state of the read buffer, providing enough data when
  // before there was *not* enough.
  //
  // So, the steps are:
  // 1. Figure out what the state of things will be after we do
  // a read from the buffer.
  //
  // 2. If that resulting state will trigger a _read, then call _read.
  // Note that this may be asynchronous, or synchronous.  Yes, it is
  // deeply ugly to write APIs this way, but that still doesn't mean
  // that the Readable class should behave improperly, as streams are
  // designed to be sync/async agnostic.
  // Take note if the _read call is sync or async (ie, if the read call
  // has returned yet), so that we know whether or not it's safe to emit
  // 'readable' etc.
  //
  // 3. Actually pull the requested chunks out of the buffer and return.

  // if we need a readable event, then we need to do some reading.
  var doRead = state.needReadable;
  debug('need readable', doRead);

  // if we currently have less than the highWaterMark, then also read some
  if (state.length === 0 || state.length - n < state.highWaterMark) {
    doRead = true;
    debug('length less than watermark', doRead);
  }

  // however, if we've ended, then there's no point, and if we're already
  // reading, then it's unnecessary.
  if (state.ended || state.reading) {
    doRead = false;
    debug('reading or ended', doRead);
  } else if (doRead) {
    debug('do read');
    state.reading = true;
    state.sync = true;
    // if the length is currently zero, then we *need* a readable event.
    if (state.length === 0) state.needReadable = true;
    // call internal read method
    this._read(state.highWaterMark);
    state.sync = false;
    // If _read pushed data synchronously, then 'reading' will be false,
    // and we need to re-evaluate how much data we can return to the user.
    if (!state.reading) n = howMuchToRead(nOrig, state);
  }

  var ret;
  if (n > 0) ret = fromList(n, state);else ret = null;

  if (ret === null) {
    state.needReadable = true;
    n = 0;
  } else {
    state.length -= n;
  }

  if (state.length === 0) {
    // If we have nothing in the buffer, then we want to know
    // as soon as we *do* get something into the buffer.
    if (!state.ended) state.needReadable = true;

    // If we tried to read() past the EOF, then emit end on the next tick.
    if (nOrig !== n && state.ended) endReadable(this);
  }

  if (ret !== null) this.emit('data', ret);

  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.duplex.super_.super_.prototype.resume"></a>[function <span class="apidocSignatureSpan">mississippi.duplex.super_.super_.prototype.</span>resume ()](#apidoc.element.mississippi.duplex.super_.super_.prototype.resume)
- description and source-code
```javascript
resume = function () {
  var state = this._readableState;
  if (!state.flowing) {
    debug('resume');
    state.flowing = true;
    resume(this, state);
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.duplex.super_.super_.prototype.setEncoding"></a>[function <span class="apidocSignatureSpan">mississippi.duplex.super_.super_.prototype.</span>setEncoding (enc)](#apidoc.element.mississippi.duplex.super_.super_.prototype.setEncoding)
- description and source-code
```javascript
setEncoding = function (enc) {
  if (!StringDecoder) StringDecoder = require('string_decoder/').StringDecoder;
  this._readableState.decoder = new StringDecoder(enc);
  this._readableState.encoding = enc;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.duplex.super_.super_.prototype.unpipe"></a>[function <span class="apidocSignatureSpan">mississippi.duplex.super_.super_.prototype.</span>unpipe (dest)](#apidoc.element.mississippi.duplex.super_.super_.prototype.unpipe)
- description and source-code
```javascript
unpipe = function (dest) {
  var state = this._readableState;

  // if we're not piping anywhere, then do nothing.
  if (state.pipesCount === 0) return this;

  // just one destination.  most common case.
  if (state.pipesCount === 1) {
    // passed in one, but it's not the right one.
    if (dest && dest !== state.pipes) return this;

    if (!dest) dest = state.pipes;

    // got a match.
    state.pipes = null;
    state.pipesCount = 0;
    state.flowing = false;
    if (dest) dest.emit('unpipe', this);
    return this;
  }

  // slow case. multiple pipe destinations.

  if (!dest) {
    // remove all.
    var dests = state.pipes;
    var len = state.pipesCount;
    state.pipes = null;
    state.pipesCount = 0;
    state.flowing = false;

    for (var i = 0; i < len; i++) {
      dests[i].emit('unpipe', this);
    }return this;
  }

  // try to find the right one.
  var index = indexOf(state.pipes, dest);
  if (index === -1) return this;

  state.pipes.splice(index, 1);
  state.pipesCount -= 1;
  if (state.pipesCount === 1) state.pipes = state.pipes[0];

  dest.emit('unpipe', this);

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.duplex.super_.super_.prototype.unshift"></a>[function <span class="apidocSignatureSpan">mississippi.duplex.super_.super_.prototype.</span>unshift (chunk)](#apidoc.element.mississippi.duplex.super_.super_.prototype.unshift)
- description and source-code
```javascript
unshift = function (chunk) {
  var state = this._readableState;
  return readableAddChunk(this, state, chunk, '', true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.duplex.super_.super_.prototype.wrap"></a>[function <span class="apidocSignatureSpan">mississippi.duplex.super_.super_.prototype.</span>wrap (stream)](#apidoc.element.mississippi.duplex.super_.super_.prototype.wrap)
- description and source-code
```javascript
wrap = function (stream) {
  var state = this._readableState;
  var paused = false;

  var self = this;
  stream.on('end', function () {
    debug('wrapped end');
    if (state.decoder && !state.ended) {
      var chunk = state.decoder.end();
      if (chunk && chunk.length) self.push(chunk);
    }

    self.push(null);
  });

  stream.on('data', function (chunk) {
    debug('wrapped data');
    if (state.decoder) chunk = state.decoder.write(chunk);

    // don't skip over falsy values in objectMode
    if (state.objectMode && (chunk === null || chunk === undefined)) return;else if (!state.objectMode && (!chunk || !chunk.length
)) return;

    var ret = self.push(chunk);
    if (!ret) {
      paused = true;
      stream.pause();
    }
  });

  // proxy all the other methods.
  // important when wrapping filters and duplexes.
  for (var i in stream) {
    if (this[i] === undefined && typeof stream[i] === 'function') {
      this[i] = function (method) {
        return function () {
          return stream[method].apply(stream, arguments);
        };
      }(i);
    }
  }

  // proxy certain important events.
  var events = ['error', 'close', 'destroy', 'pause', 'resume'];
  forEach(events, function (ev) {
    stream.on(ev, self.emit.bind(self, ev));
  });

  // when we try to consume some more bytes, simply unpause the
  // underlying stream.
  self._read = function (n) {
    debug('wrapped _read', n);
    if (paused) {
      paused = false;
      stream.resume();
    }
  };

  return self;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mississippi.from"></a>[module mississippi.from](#apidoc.module.mississippi.from)

#### <a name="apidoc.element.mississippi.from.from"></a>[function <span class="apidocSignatureSpan">mississippi.</span>from (opts, read)](#apidoc.element.mississippi.from.from)
- description and source-code
```javascript
function from2(opts, read) {
  if (typeof opts !== 'object' || Array.isArray(opts)) {
    read = opts
    opts = {}
  }

  var rs = new Proto(opts)
  rs._from = Array.isArray(read) ? toFunction(read) : (read || noop)
  return rs
}
```
- example usage
```shell
...
  if (err) return console.error('Trouble uppercasing!')
  console.log('Splendid uppercasing!')
})
'''

### from

#####'miss.from([opts], read)'

Make a custom [readable stream](https://nodejs.org/docs/latest/api/stream.html#stream_class_stream_readable).

'opts' contains the options to pass on to the ReadableStream constructor e.g. for creating a readable object stream (or use the
shortcut 'miss.from.obj([...])').

Returns a readable stream that calls 'read(size, next)' when data is requested from the stream.
...
```

#### <a name="apidoc.element.mississippi.from.ctor"></a>[function <span class="apidocSignatureSpan">mississippi.from.</span>ctor (opts, read)](#apidoc.element.mississippi.from.ctor)
- description and source-code
```javascript
function ctor(opts, read) {
  if (typeof opts === 'function') {
    read = opts
    opts = {}
  }

  opts = defaults(opts)

  inherits(Class, Readable)
  function Class(override) {
    if (!(this instanceof Class)) return new Class(override)
    this._reading = false
    this._callback = check
    this.destroyed = false
    Readable.call(this, override || opts)

    var self = this
    var hwm = this._readableState.highWaterMark

    function check(err, data) {
      if (self.destroyed) return
      if (err) return self.destroy(err)
      if (data === null) return self.push(null)
      self._reading = false
      if (self.push(data)) self._read(hwm)
    }
  }

  Class.prototype._from = read || noop
  Class.prototype._read = function(size) {
    if (this._reading || this.destroyed) return
    this._reading = true
    this._from(size, this._callback)
  }

  Class.prototype.destroy = function(err) {
    if (this.destroyed) return
    this.destroyed = true

    var self = this
    process.nextTick(function() {
      if (err) self.emit('error', err)
      self.emit('close')
    })
  }

  return Class
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.from.obj"></a>[function <span class="apidocSignatureSpan">mississippi.from.</span>obj (opts, read)](#apidoc.element.mississippi.from.obj)
- description and source-code
```javascript
function obj(opts, read) {
  if (typeof opts === 'function' || Array.isArray(opts)) {
    read = opts
    opts = {}
  }

  opts = defaults(opts)
  opts.objectMode = true
  opts.highWaterMark = 16

  return from2(opts, read)
}
```
- example usage
```shell
...

### through

#####'var transformer = miss.through([options, transformFunction, flushFunction])'

Make a custom [transform stream](https://nodejs.org/docs/latest/api/stream.html#stream_class_stream_transform).

The 'options' object is passed to the internal transform stream and can be used to create an 'objectMode' stream (or use the shortcut
 'miss.through.obj([...])')

The 'transformFunction' is called when data is available for the writable side and has the signature '(chunk, encoding, cb)'. Within
 the function, add data to the readable side any number of times with 'this.push(data)'. Call 'cb()' to indicate processing of the
 'chunk' is complete. Or to easily emit a single error or chunk, call 'cb(err, chunk)'

The 'flushFunction', with signature '(cb)', is called just before the stream is complete and should be used to wrap up stream processing
.

#### original module
...
```



# <a name="apidoc.module.mississippi.pipeline"></a>[module mississippi.pipeline](#apidoc.module.mississippi.pipeline)

#### <a name="apidoc.element.mississippi.pipeline.pipeline"></a>[function <span class="apidocSignatureSpan">mississippi.</span>pipeline ()](#apidoc.element.mississippi.pipeline.pipeline)
- description and source-code
```javascript
pipeline = function () {
  var streams = toArray(arguments)
  if (!(this instanceof Pumpify)) return new Pumpify(streams)
  Duplexify.call(this, null, null, opts)
  if (streams.length) this.setPipeline(streams)
}
```
- example usage
```shell
...

'''js
var fs = require('fs')
var split = require('split2')

var newLineSeparatedNumbers = fs.createReadStream('numbers.txt')

var pipeline = miss.pipeline(newLineSeparatedNumbers, split())
var each = miss.each(pipeline, eachLine, done)
var sum = 0

function eachLine (line, next) {
  sum += parseInt(line.toString())
  next()
}
...
```

#### <a name="apidoc.element.mississippi.pipeline.obj"></a>[function <span class="apidocSignatureSpan">mississippi.pipeline.</span>obj ()](#apidoc.element.mississippi.pipeline.obj)
- description and source-code
```javascript
obj = function () {
  var streams = toArray(arguments)
  if (!(this instanceof Pumpify)) return new Pumpify(streams)
  Duplexify.call(this, null, null, opts)
  if (streams.length) this.setPipeline(streams)
}
```
- example usage
```shell
...

### through

#####'var transformer = miss.through([options, transformFunction, flushFunction])'

Make a custom [transform stream](https://nodejs.org/docs/latest/api/stream.html#stream_class_stream_transform).

The 'options' object is passed to the internal transform stream and can be used to create an 'objectMode' stream (or use the shortcut
 'miss.through.obj([...])')

The 'transformFunction' is called when data is available for the writable side and has the signature '(chunk, encoding, cb)'. Within
 the function, add data to the readable side any number of times with 'this.push(data)'. Call 'cb()' to indicate processing of the
 'chunk' is complete. Or to easily emit a single error or chunk, call 'cb(err, chunk)'

The 'flushFunction', with signature '(cb)', is called just before the stream is complete and should be used to wrap up stream processing
.

#### original module
...
```

#### <a name="apidoc.element.mississippi.pipeline.super_"></a>[function <span class="apidocSignatureSpan">mississippi.pipeline.</span>super_ (writable, readable, opts)](#apidoc.element.mississippi.pipeline.super_)
- description and source-code
```javascript
super_ = function (writable, readable, opts) {
  if (!(this instanceof Duplexify)) return new Duplexify(writable, readable, opts)
  stream.Duplex.call(this, opts)

  this._writable = null
  this._readable = null
  this._readable2 = null

  this._forwardDestroy = !opts || opts.destroy !== false
  this._forwardEnd = !opts || opts.end !== false
  this._corked = 1 // start corked
  this._ondrain = null
  this._drained = false
  this._forwarding = false
  this._unwrite = null
  this._unread = null
  this._ended = false

  this.destroyed = false

  if (writable) this.setWritable(writable)
  if (readable) this.setReadable(readable)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mississippi.pipeline.obj"></a>[module mississippi.pipeline.obj](#apidoc.module.mississippi.pipeline.obj)

#### <a name="apidoc.element.mississippi.pipeline.obj.obj"></a>[function <span class="apidocSignatureSpan">mississippi.pipeline.</span>obj ()](#apidoc.element.mississippi.pipeline.obj.obj)
- description and source-code
```javascript
obj = function () {
  var streams = toArray(arguments)
  if (!(this instanceof Pumpify)) return new Pumpify(streams)
  Duplexify.call(this, null, null, opts)
  if (streams.length) this.setPipeline(streams)
}
```
- example usage
```shell
...

### through

#####'var transformer = miss.through([options, transformFunction, flushFunction])'

Make a custom [transform stream](https://nodejs.org/docs/latest/api/stream.html#stream_class_stream_transform).

The 'options' object is passed to the internal transform stream and can be used to create an 'objectMode' stream (or use the shortcut
 'miss.through.obj([...])')

The 'transformFunction' is called when data is available for the writable side and has the signature '(chunk, encoding, cb)'. Within
 the function, add data to the readable side any number of times with 'this.push(data)'. Call 'cb()' to indicate processing of the
 'chunk' is complete. Or to easily emit a single error or chunk, call 'cb(err, chunk)'

The 'flushFunction', with signature '(cb)', is called just before the stream is complete and should be used to wrap up stream processing
.

#### original module
...
```

#### <a name="apidoc.element.mississippi.pipeline.obj.super_"></a>[function <span class="apidocSignatureSpan">mississippi.pipeline.obj.</span>super_ (writable, readable, opts)](#apidoc.element.mississippi.pipeline.obj.super_)
- description and source-code
```javascript
super_ = function (writable, readable, opts) {
  if (!(this instanceof Duplexify)) return new Duplexify(writable, readable, opts)
  stream.Duplex.call(this, opts)

  this._writable = null
  this._readable = null
  this._readable2 = null

  this._forwardDestroy = !opts || opts.destroy !== false
  this._forwardEnd = !opts || opts.end !== false
  this._corked = 1 // start corked
  this._ondrain = null
  this._drained = false
  this._forwarding = false
  this._unwrite = null
  this._unread = null
  this._ended = false

  this.destroyed = false

  if (writable) this.setWritable(writable)
  if (readable) this.setReadable(readable)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mississippi.pipeline.obj.prototype"></a>[module mississippi.pipeline.obj.prototype](#apidoc.module.mississippi.pipeline.obj.prototype)

#### <a name="apidoc.element.mississippi.pipeline.obj.prototype.setPipeline"></a>[function <span class="apidocSignatureSpan">mississippi.pipeline.obj.prototype.</span>setPipeline ()](#apidoc.element.mississippi.pipeline.obj.prototype.setPipeline)
- description and source-code
```javascript
setPipeline = function () {
  var streams = toArray(arguments)
  var self = this
  var ended = false
  var w = streams[0]
  var r = streams[streams.length-1]

  r = r.readable ? r : null
  w = w.writable ? w : null

  var onclose = function() {
    streams[0].emit('error', new Error('stream was destroyed'))
  }

  this.on('close', onclose)
  this.on('prefinish', function() {
    if (!ended) self.cork()
  })

  pump(streams, function(err) {
    self.removeListener('close', onclose)
    if (err) return self.destroy(err)
    ended = true
    self.uncork()
  })

  if (this.destroyed) return onclose()
  this.setWritable(w)
  this.setReadable(r)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mississippi.pipeline.prototype"></a>[module mississippi.pipeline.prototype](#apidoc.module.mississippi.pipeline.prototype)

#### <a name="apidoc.element.mississippi.pipeline.prototype.setPipeline"></a>[function <span class="apidocSignatureSpan">mississippi.pipeline.prototype.</span>setPipeline ()](#apidoc.element.mississippi.pipeline.prototype.setPipeline)
- description and source-code
```javascript
setPipeline = function () {
  var streams = toArray(arguments)
  var self = this
  var ended = false
  var w = streams[0]
  var r = streams[streams.length-1]

  r = r.readable ? r : null
  w = w.writable ? w : null

  var onclose = function() {
    streams[0].emit('error', new Error('stream was destroyed'))
  }

  this.on('close', onclose)
  this.on('prefinish', function() {
    if (!ended) self.cork()
  })

  pump(streams, function(err) {
    self.removeListener('close', onclose)
    if (err) return self.destroy(err)
    ended = true
    self.uncork()
  })

  if (this.destroyed) return onclose()
  this.setWritable(w)
  this.setReadable(r)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mississippi.through"></a>[module mississippi.through](#apidoc.module.mississippi.through)

#### <a name="apidoc.element.mississippi.through.through"></a>[function <span class="apidocSignatureSpan">mississippi.</span>through (options, transform, flush)](#apidoc.element.mississippi.through.through)
- description and source-code
```javascript
through = function (options, transform, flush) {
  if (typeof options == 'function') {
    flush     = transform
    transform = options
    options   = {}
  }

  if (typeof transform != 'function')
    transform = noop

  if (typeof flush != 'function')
    flush = null

  return construct(options, transform, flush)
}
```
- example usage
```shell
...

// duplexCurl will write to stdin and read from stdout
var duplexCurl = miss.duplex(curl.stdin, curl.stdout)
'''

### through

#####'var transformer = miss.through([options, transformFunction, flushFunction])'

Make a custom [transform stream](https://nodejs.org/docs/latest/api/stream.html#stream_class_stream_transform).

The 'options' object is passed to the internal transform stream and can be used to create an 'objectMode' stream (or use the shortcut
 'miss.through.obj([...])')

The 'transformFunction' is called when data is available for the writable side and has the signature '(chunk, encoding, cb)'. Within
 the function, add data to the readable side any number of times with 'this.push(data)'. Call 'cb()' to indicate processing of the
 'chunk' is complete. Or to easily emit a single error or chunk, call 'cb(err, chunk)'
...
```

#### <a name="apidoc.element.mississippi.through.ctor"></a>[function <span class="apidocSignatureSpan">mississippi.through.</span>ctor (options, transform, flush)](#apidoc.element.mississippi.through.ctor)
- description and source-code
```javascript
ctor = function (options, transform, flush) {
  if (typeof options == 'function') {
    flush     = transform
    transform = options
    options   = {}
  }

  if (typeof transform != 'function')
    transform = noop

  if (typeof flush != 'function')
    flush = null

  return construct(options, transform, flush)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.through.obj"></a>[function <span class="apidocSignatureSpan">mississippi.through.</span>obj (options, transform, flush)](#apidoc.element.mississippi.through.obj)
- description and source-code
```javascript
obj = function (options, transform, flush) {
  if (typeof options == 'function') {
    flush     = transform
    transform = options
    options   = {}
  }

  if (typeof transform != 'function')
    transform = noop

  if (typeof flush != 'function')
    flush = null

  return construct(options, transform, flush)
}
```
- example usage
```shell
...

### through

#####'var transformer = miss.through([options, transformFunction, flushFunction])'

Make a custom [transform stream](https://nodejs.org/docs/latest/api/stream.html#stream_class_stream_transform).

The 'options' object is passed to the internal transform stream and can be used to create an 'objectMode' stream (or use the shortcut
 'miss.through.obj([...])')

The 'transformFunction' is called when data is available for the writable side and has the signature '(chunk, encoding, cb)'. Within
 the function, add data to the readable side any number of times with 'this.push(data)'. Call 'cb()' to indicate processing of the
 'chunk' is complete. Or to easily emit a single error or chunk, call 'cb(err, chunk)'

The 'flushFunction', with signature '(cb)', is called just before the stream is complete and should be used to wrap up stream processing
.

#### original module
...
```



# <a name="apidoc.module.mississippi.to"></a>[module mississippi.to](#apidoc.module.mississippi.to)

#### <a name="apidoc.element.mississippi.to.to"></a>[function <span class="apidocSignatureSpan">mississippi.</span>to (opts, write, flush)](#apidoc.element.mississippi.to.to)
- description and source-code
```javascript
function WriteStream(opts, write, flush) {
  if (!(this instanceof WriteStream)) return new WriteStream(opts, write, flush)

  if (typeof opts === 'function') {
    flush = write
    write = opts
    opts = {}
  }

  stream.Writable.call(this, opts)

  this.destroyed = false
  this._worker = write || null
  this._flush = flush || null
}
```
- example usage
```shell
...
// pipe "hello world" out
// to stdout.
fromString('hello world').pipe(process.stdout)
'''

### to

#####'miss.to([options], write, [flush])'

Make a custom [writable stream](https://nodejs.org/docs/latest/api/stream.html#stream_class_stream_writable).

'opts' contains the options to pass on to the WritableStream constructor e.g. for creating a readable object stream (or use the
shortcut 'miss.to.obj([...])').

Returns a writable stream that calls 'write(data, enc, cb)' when data is written to the stream.
...
```

#### <a name="apidoc.element.mississippi.to.obj"></a>[function <span class="apidocSignatureSpan">mississippi.to.</span>obj (opts, worker, flush)](#apidoc.element.mississippi.to.obj)
- description and source-code
```javascript
obj = function (opts, worker, flush) {
  if (typeof opts === 'function') return WriteStream.obj(null, opts, worker)
  if (!opts) opts = {}
  opts.objectMode = true
  return new WriteStream(opts, worker, flush)
}
```
- example usage
```shell
...

### through

#####'var transformer = miss.through([options, transformFunction, flushFunction])'

Make a custom [transform stream](https://nodejs.org/docs/latest/api/stream.html#stream_class_stream_transform).

The 'options' object is passed to the internal transform stream and can be used to create an 'objectMode' stream (or use the shortcut
 'miss.through.obj([...])')

The 'transformFunction' is called when data is available for the writable side and has the signature '(chunk, encoding, cb)'. Within
 the function, add data to the readable side any number of times with 'this.push(data)'. Call 'cb()' to indicate processing of the
 'chunk' is complete. Or to easily emit a single error or chunk, call 'cb(err, chunk)'

The 'flushFunction', with signature '(cb)', is called just before the stream is complete and should be used to wrap up stream processing
.

#### original module
...
```

#### <a name="apidoc.element.mississippi.to.super_"></a>[function <span class="apidocSignatureSpan">mississippi.to.</span>super_ (options)](#apidoc.element.mississippi.to.super_)
- description and source-code
```javascript
function Writable(options) {
  Duplex = Duplex || require('./_stream_duplex');

  // Writable ctor is applied to Duplexes, too.
  // 'realHasInstance' is necessary because using plain 'instanceof'
  // would return false, as no '_writableState' property is attached.

  // Trying to use the custom 'instanceof' for Writable here will also break the
  // Node.js LazyTransform implementation, which has a non-trivial getter for
  // '_writableState' that would lead to infinite recursion.
  if (!realHasInstance.call(Writable, this) && !(this instanceof Duplex)) {
    return new Writable(options);
  }

  this._writableState = new WritableState(options, this);

  // legacy.
  this.writable = true;

  if (options) {
    if (typeof options.write === 'function') this._write = options.write;

    if (typeof options.writev === 'function') this._writev = options.writev;
  }

  Stream.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mississippi.to.prototype"></a>[module mississippi.to.prototype](#apidoc.module.mississippi.to.prototype)

#### <a name="apidoc.element.mississippi.to.prototype._write"></a>[function <span class="apidocSignatureSpan">mississippi.to.prototype.</span>_write (data, enc, cb)](#apidoc.element.mississippi.to.prototype._write)
- description and source-code
```javascript
_write = function (data, enc, cb) {
  if (SIGNAL_FLUSH === data) this._flush(cb)
  else this._worker(data, enc, cb)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.to.prototype.destroy"></a>[function <span class="apidocSignatureSpan">mississippi.to.prototype.</span>destroy (err)](#apidoc.element.mississippi.to.prototype.destroy)
- description and source-code
```javascript
destroy = function (err) {
  if (this.destroyed) return
  this.destroyed = true
  if (err) this.emit('error', err)
  this.emit('close')
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mississippi.to.prototype.end"></a>[function <span class="apidocSignatureSpan">mississippi.to.prototype.</span>end (data, enc, cb)](#apidoc.element.mississippi.to.prototype.end)
- description and source-code
```javascript
end = function (data, enc, cb) {
  if (!this._flush) return stream.Writable.prototype.end.apply(this, arguments)
  if (typeof data === 'function') return this.end(null, null, data)
  if (typeof enc === 'function') return this.end(data, null, enc)
  if (data) this.write(data)
  if (!this._writableState.ending) this.write(SIGNAL_FLUSH)
  return stream.Writable.prototype.end.call(this, cb)
}
```
- example usage
```shell
...

ws.on('finish', function () {
  console.log('finished')
})

ws.write('hello')
ws.write('world')
ws.end()

function write (data, enc, cb) {
  // i am your normal ._write method
  console.log('writing', data.toString())
  cb()
}
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
