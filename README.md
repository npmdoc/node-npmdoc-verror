# api documentation for  [verror (v1.9.0)](https://github.com/davepacheco/node-verror#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-verror.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-verror) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-verror.svg)](https://travis-ci.org/npmdoc/node-npmdoc-verror)
#### richer JavaScript errors

[![NPM](https://nodei.co/npm/verror.png?downloads=true)](https://www.npmjs.com/package/verror)

[![apidoc](https://npmdoc.github.io/node-npmdoc-verror/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-verror_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-verror/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-verror/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-verror/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "bugs": {
        "url": "https://github.com/davepacheco/node-verror/issues"
    },
    "dependencies": {
        "assert-plus": "^1.0.0",
        "core-util-is": "1.0.2",
        "extsprintf": "^1.2.0"
    },
    "description": "richer JavaScript errors",
    "devDependencies": {},
    "directories": {},
    "dist": {
        "shasum": "107a8a2d14c33586fc4bb830057cd2d19ae2a6ee",
        "tarball": "https://registry.npmjs.org/verror/-/verror-1.9.0.tgz"
    },
    "engines": [
        "node >=0.6.0"
    ],
    "gitHead": "29b7ce4dc7c4e488b00355db5a41a11496633679",
    "homepage": "https://github.com/davepacheco/node-verror#readme",
    "license": "MIT",
    "main": "./lib/verror.js",
    "maintainers": [
        {
            "name": "dap",
            "email": "dap@cs.brown.edu"
        }
    ],
    "name": "verror",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/davepacheco/node-verror.git"
    },
    "scripts": {
        "test": "make test"
    },
    "version": "1.9.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module verror](#apidoc.module.verror)
1.  [function <span class="apidocSignatureSpan">verror.</span>MultiError (errors)](#apidoc.element.verror.MultiError)
1.  [function <span class="apidocSignatureSpan">verror.</span>SError ()](#apidoc.element.verror.SError)
1.  [function <span class="apidocSignatureSpan">verror.</span>VError ()](#apidoc.element.verror.VError)
1.  [function <span class="apidocSignatureSpan">verror.</span>WError ()](#apidoc.element.verror.WError)
1.  [function <span class="apidocSignatureSpan">verror.</span>cause (err)](#apidoc.element.verror.cause)
1.  [function <span class="apidocSignatureSpan">verror.</span>findCauseByName (err, name)](#apidoc.element.verror.findCauseByName)
1.  [function <span class="apidocSignatureSpan">verror.</span>fullStack (err)](#apidoc.element.verror.fullStack)
1.  [function <span class="apidocSignatureSpan">verror.</span>hasCauseWithName (err, name)](#apidoc.element.verror.hasCauseWithName)
1.  [function <span class="apidocSignatureSpan">verror.</span>info (err)](#apidoc.element.verror.info)
1.  [function <span class="apidocSignatureSpan">verror.</span>super_ ()](#apidoc.element.verror.super_)
1.  object <span class="apidocSignatureSpan">verror.</span>MultiError.prototype
1.  object <span class="apidocSignatureSpan">verror.</span>WError.prototype

#### [module verror.MultiError](#apidoc.module.verror.MultiError)
1.  [function <span class="apidocSignatureSpan">verror.</span>MultiError (errors)](#apidoc.element.verror.MultiError.MultiError)
1.  [function <span class="apidocSignatureSpan">verror.MultiError.</span>super_ ()](#apidoc.element.verror.MultiError.super_)

#### [module verror.MultiError.prototype](#apidoc.module.verror.MultiError.prototype)
1.  [function <span class="apidocSignatureSpan">verror.MultiError.prototype.</span>errors ()](#apidoc.element.verror.MultiError.prototype.errors)
1.  string <span class="apidocSignatureSpan">verror.MultiError.prototype.</span>name

#### [module verror.SError](#apidoc.module.verror.SError)
1.  [function <span class="apidocSignatureSpan">verror.</span>SError ()](#apidoc.element.verror.SError.SError)
1.  [function <span class="apidocSignatureSpan">verror.SError.</span>super_ ()](#apidoc.element.verror.SError.super_)

#### [module verror.WError](#apidoc.module.verror.WError)
1.  [function <span class="apidocSignatureSpan">verror.</span>WError ()](#apidoc.element.verror.WError.WError)
1.  [function <span class="apidocSignatureSpan">verror.WError.</span>super_ ()](#apidoc.element.verror.WError.super_)

#### [module verror.WError.prototype](#apidoc.module.verror.WError.prototype)
1.  [function <span class="apidocSignatureSpan">verror.WError.prototype.</span>cause (c)](#apidoc.element.verror.WError.prototype.cause)
1.  [function <span class="apidocSignatureSpan">verror.WError.prototype.</span>toString ()](#apidoc.element.verror.WError.prototype.toString)
1.  string <span class="apidocSignatureSpan">verror.WError.prototype.</span>name

#### [module verror.super_](#apidoc.module.verror.super_)
1.  [function <span class="apidocSignatureSpan">verror.</span>super_ ()](#apidoc.element.verror.super_.super_)
1.  [function <span class="apidocSignatureSpan">verror.super_.</span>captureStackTrace ()](#apidoc.element.verror.super_.captureStackTrace)
1.  number <span class="apidocSignatureSpan">verror.super_.</span>stackTraceLimit



# <a name="apidoc.module.verror"></a>[module verror](#apidoc.module.verror)

#### <a name="apidoc.element.verror.MultiError"></a>[function <span class="apidocSignatureSpan">verror.</span>MultiError (errors)](#apidoc.element.verror.MultiError)
- description and source-code
```javascript
function MultiError(errors)
{
	mod_assertplus.array(errors, 'list of errors');
	mod_assertplus.ok(errors.length > 0, 'must be at least one error');
	this.ase_errors = errors;

	VError.call(this, {
	    'cause': errors[0]
	}, 'first of %d error%s', errors.length, errors.length == 1 ? '' : 's');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.verror.SError"></a>[function <span class="apidocSignatureSpan">verror.</span>SError ()](#apidoc.element.verror.SError)
- description and source-code
```javascript
function SError()
{
	var args, obj, parsed, options;

	args = Array.prototype.slice.call(arguments, 0);
	if (!(this instanceof SError)) {
		obj = Object.create(SError.prototype);
		SError.apply(obj, arguments);
		return (obj);
	}

	parsed = parseConstructorArguments({
	    'argv': args,
	    'strict': true
	});

	options = parsed.options;
	VError.call(this, options, '%s', parsed.shortmessage);

	return (this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.verror.VError"></a>[function <span class="apidocSignatureSpan">verror.</span>VError ()](#apidoc.element.verror.VError)
- description and source-code
```javascript
function VError()
{
	var args, obj, parsed, cause, ctor, message, k;

	args = Array.prototype.slice.call(arguments, 0);

	<span class="apidocCodeCommentSpan">/*
	 * This is a regrettable pattern, but JavaScript's built-in Error class
	 * is defined to work this way, so we allow the constructor to be called
	 * without "new".
	 */
</span>	if (!(this instanceof VError)) {
		obj = Object.create(VError.prototype);
		VError.apply(obj, arguments);
		return (obj);
	}

	/*
	 * For convenience and backwards compatibility, we support several
	 * different calling forms.  Normalize them here.
	 */
	parsed = parseConstructorArguments({
	    'argv': args,
	    'strict': false
	});

	/*
	 * If we've been given a name, apply it now.
	 */
	if (parsed.options.name) {
		mod_assertplus.string(parsed.options.name,
		    'error\'s "name" must be a string');
		this.name = parsed.options.name;
	}

	/*
	 * For debugging, we keep track of the original short message (attached
	 * this Error particularly) separately from the complete message (which
	 * includes the messages of our cause chain).
	 */
	this.jse_shortmsg = parsed.shortmessage;
	message = parsed.shortmessage;

	/*
	 * If we've been given a cause, record a reference to it and update our
	 * message appropriately.
	 */
	cause = parsed.options.cause;
	if (cause) {
		mod_assertplus.ok(mod_isError(cause), 'cause is not an Error');
		this.jse_cause = cause;

		if (!parsed.options.skipCauseMessage) {
			message += ': ' + cause.message;
		}
	}

	/*
	 * If we've been given an object with properties, shallow-copy that
	 * here.  We don't want to use a deep copy in case there are non-plain
	 * objects here, but we don't want to use the original object in case
	 * the caller modifies it later.
	 */
	this.jse_info = {};
	if (parsed.options.info) {
		for (k in parsed.options.info) {
			this.jse_info[k] = parsed.options.info[k];
		}
	}

	this.message = message;
	Error.call(this, message);

	if (Error.captureStackTrace) {
		ctor = parsed.options.constructorOpt || this.constructor;
		Error.captureStackTrace(this, ctor);
	}

	return (this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.verror.WError"></a>[function <span class="apidocSignatureSpan">verror.</span>WError ()](#apidoc.element.verror.WError)
- description and source-code
```javascript
function WError()
{
	var args, obj, parsed, options;

	args = Array.prototype.slice.call(arguments, 0);
	if (!(this instanceof WError)) {
		obj = Object.create(WError.prototype);
		WError.apply(obj, args);
		return (obj);
	}

	parsed = parseConstructorArguments({
	    'argv': args,
	    'strict': false
	});

	options = parsed.options;
	options['skipCauseMessage'] = true;
	VError.call(this, options, '%s', parsed.shortmessage);

	return (this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.verror.cause"></a>[function <span class="apidocSignatureSpan">verror.</span>cause (err)](#apidoc.element.verror.cause)
- description and source-code
```javascript
cause = function (err)
{
	mod_assertplus.ok(mod_isError(err), 'err must be an Error');
	return (mod_isError(err.jse_cause) ? err.jse_cause : null);
}
```
- example usage
```shell
...
    sort: open failed: /nonexistent: No such file or directory

To match the Unixy feel, when you print out the error, just prepend the
program's name to the VError's 'message'.  Or just call
[node-cmdutil.fail(your_verror)](https://github.com/joyent/node-cmdutil), which
does this for you.

You can get the next-level Error using 'err.cause()':

'''javascript
console.error(err2.cause().message);
'''

prints:
...
```

#### <a name="apidoc.element.verror.findCauseByName"></a>[function <span class="apidocSignatureSpan">verror.</span>findCauseByName (err, name)](#apidoc.element.verror.findCauseByName)
- description and source-code
```javascript
findCauseByName = function (err, name)
{
	var cause;

	mod_assertplus.ok(mod_isError(err), 'err must be an Error');
	mod_assertplus.string(name, 'name');
	mod_assertplus.ok(name.length > 0, 'name cannot be empty');

	for (cause = err; cause !== null; cause = VError.cause(cause)) {
		mod_assertplus.ok(mod_isError(cause));
		if (cause.name == name) {
			return (cause);
		}
	}

	return (null);
}
```
- example usage
```shell
...
booleans, strings, and objects and arrays containing only other plain objects).

### 'VError.fullStack(err)'

Returns a string containing the full stack trace, with all nested errors recursively
reported as ''caused by:' + err.stack'.

### 'VError.findCauseByName(err, name)'

The 'findCauseByName()' function traverses the cause chain for 'err', looking
for an error whose 'name' property matches the passed in 'name' value. If no
match is found, 'null' is returned.

If all you want is to know _whether_ there's a cause (and you don't care what it
is), you can use 'VError.hasCauseWithName(err, name)'.
...
```

#### <a name="apidoc.element.verror.fullStack"></a>[function <span class="apidocSignatureSpan">verror.</span>fullStack (err)](#apidoc.element.verror.fullStack)
- description and source-code
```javascript
fullStack = function (err)
{
	mod_assertplus.ok(mod_isError(err), 'err must be an Error');

	var cause = VError.cause(err);

	if (cause) {
		return (err.stack + '\ncaused by: ' + VError.fullStack(cause));
	}

	return (err.stack);
}
```
- example usage
```shell
...
These properties are intended to provide programmatically-accessible metadata
about the error.  For an error that indicates a failure to resolve a DNS name,
informational properties might include the DNS name to be resolved, or even the
list of resolvers used to resolve it.  The values of these properties should
generally be plain objects (i.e., consisting only of null, undefined, numbers,
booleans, strings, and objects and arrays containing only other plain objects).

### 'VError.fullStack(err)'

Returns a string containing the full stack trace, with all nested errors recursively
reported as ''caused by:' + err.stack'.

### 'VError.findCauseByName(err, name)'

The 'findCauseByName()' function traverses the cause chain for 'err', looking
...
```

#### <a name="apidoc.element.verror.hasCauseWithName"></a>[function <span class="apidocSignatureSpan">verror.</span>hasCauseWithName (err, name)](#apidoc.element.verror.hasCauseWithName)
- description and source-code
```javascript
hasCauseWithName = function (err, name)
{
	return (VError.findCauseByName(err, name) !== null);
}
```
- example usage
```shell
...
### 'VError.findCauseByName(err, name)'

The 'findCauseByName()' function traverses the cause chain for 'err', looking
for an error whose 'name' property matches the passed in 'name' value. If no
match is found, 'null' is returned.

If all you want is to know _whether_ there's a cause (and you don't care what it
is), you can use 'VError.hasCauseWithName(err, name)'.

If a vanilla error or a non-VError error is passed in, then there is no cause
chain to traverse. In this scenario, the function will check the 'name'
property of only 'err'.

### 'VError.hasCauseWithName(err, name)'
...
```

#### <a name="apidoc.element.verror.info"></a>[function <span class="apidocSignatureSpan">verror.</span>info (err)](#apidoc.element.verror.info)
- description and source-code
```javascript
info = function (err)
{
	var rv, cause, k;

	mod_assertplus.ok(mod_isError(err), 'err must be an Error');
	cause = VError.cause(err);
	if (cause !== null) {
		rv = VError.info(cause);
	} else {
		rv = {};
	}

	if (typeof (err.jse_info) == 'object' && err.jse_info !== null) {
		for (k in err.jse_info) {
			rv[k] = err.jse_info[k];
		}
	}

	return (rv);
}
```
- example usage
```shell
...
    name: FastServerError
    message: "server error: user 'bob' is not authorized"
    cause:
        name: UnauthorizedError
        message: "user 'bob' is not authorized"
        rpcUser: "bob"

When the caller uses 'VError.info()', the information properties are collapsed
so that it looks like this:

message: "request failed: server error: user 'bob' is not authorized"
rpcMsgid: <unique identifier for this request>
rpcMethod: GetObject
rpcUser: "bob"
...
```

#### <a name="apidoc.element.verror.super_"></a>[function <span class="apidocSignatureSpan">verror.</span>super_ ()](#apidoc.element.verror.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.verror.MultiError"></a>[module verror.MultiError](#apidoc.module.verror.MultiError)

#### <a name="apidoc.element.verror.MultiError.MultiError"></a>[function <span class="apidocSignatureSpan">verror.</span>MultiError (errors)](#apidoc.element.verror.MultiError.MultiError)
- description and source-code
```javascript
function MultiError(errors)
{
	mod_assertplus.array(errors, 'list of errors');
	mod_assertplus.ok(errors.length > 0, 'must be at least one error');
	this.ase_errors = errors;

	VError.call(this, {
	    'cause': errors[0]
	}, 'first of %d error%s', errors.length, errors.length == 1 ? '' : 's');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.verror.MultiError.super_"></a>[function <span class="apidocSignatureSpan">verror.MultiError.</span>super_ ()](#apidoc.element.verror.MultiError.super_)
- description and source-code
```javascript
function VError()
{
	var args, obj, parsed, cause, ctor, message, k;

	args = Array.prototype.slice.call(arguments, 0);

	<span class="apidocCodeCommentSpan">/*
	 * This is a regrettable pattern, but JavaScript's built-in Error class
	 * is defined to work this way, so we allow the constructor to be called
	 * without "new".
	 */
</span>	if (!(this instanceof VError)) {
		obj = Object.create(VError.prototype);
		VError.apply(obj, arguments);
		return (obj);
	}

	/*
	 * For convenience and backwards compatibility, we support several
	 * different calling forms.  Normalize them here.
	 */
	parsed = parseConstructorArguments({
	    'argv': args,
	    'strict': false
	});

	/*
	 * If we've been given a name, apply it now.
	 */
	if (parsed.options.name) {
		mod_assertplus.string(parsed.options.name,
		    'error\'s "name" must be a string');
		this.name = parsed.options.name;
	}

	/*
	 * For debugging, we keep track of the original short message (attached
	 * this Error particularly) separately from the complete message (which
	 * includes the messages of our cause chain).
	 */
	this.jse_shortmsg = parsed.shortmessage;
	message = parsed.shortmessage;

	/*
	 * If we've been given a cause, record a reference to it and update our
	 * message appropriately.
	 */
	cause = parsed.options.cause;
	if (cause) {
		mod_assertplus.ok(mod_isError(cause), 'cause is not an Error');
		this.jse_cause = cause;

		if (!parsed.options.skipCauseMessage) {
			message += ': ' + cause.message;
		}
	}

	/*
	 * If we've been given an object with properties, shallow-copy that
	 * here.  We don't want to use a deep copy in case there are non-plain
	 * objects here, but we don't want to use the original object in case
	 * the caller modifies it later.
	 */
	this.jse_info = {};
	if (parsed.options.info) {
		for (k in parsed.options.info) {
			this.jse_info[k] = parsed.options.info[k];
		}
	}

	this.message = message;
	Error.call(this, message);

	if (Error.captureStackTrace) {
		ctor = parsed.options.constructorOpt || this.constructor;
		Error.captureStackTrace(this, ctor);
	}

	return (this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.verror.MultiError.prototype"></a>[module verror.MultiError.prototype](#apidoc.module.verror.MultiError.prototype)

#### <a name="apidoc.element.verror.MultiError.prototype.errors"></a>[function <span class="apidocSignatureSpan">verror.MultiError.prototype.</span>errors ()](#apidoc.element.verror.MultiError.prototype.errors)
- description and source-code
```javascript
function me_errors()
{
	return (this.ase_errors.slice(0));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.verror.SError"></a>[module verror.SError](#apidoc.module.verror.SError)

#### <a name="apidoc.element.verror.SError.SError"></a>[function <span class="apidocSignatureSpan">verror.</span>SError ()](#apidoc.element.verror.SError.SError)
- description and source-code
```javascript
function SError()
{
	var args, obj, parsed, options;

	args = Array.prototype.slice.call(arguments, 0);
	if (!(this instanceof SError)) {
		obj = Object.create(SError.prototype);
		SError.apply(obj, arguments);
		return (obj);
	}

	parsed = parseConstructorArguments({
	    'argv': args,
	    'strict': true
	});

	options = parsed.options;
	VError.call(this, options, '%s', parsed.shortmessage);

	return (this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.verror.SError.super_"></a>[function <span class="apidocSignatureSpan">verror.SError.</span>super_ ()](#apidoc.element.verror.SError.super_)
- description and source-code
```javascript
function VError()
{
	var args, obj, parsed, cause, ctor, message, k;

	args = Array.prototype.slice.call(arguments, 0);

	<span class="apidocCodeCommentSpan">/*
	 * This is a regrettable pattern, but JavaScript's built-in Error class
	 * is defined to work this way, so we allow the constructor to be called
	 * without "new".
	 */
</span>	if (!(this instanceof VError)) {
		obj = Object.create(VError.prototype);
		VError.apply(obj, arguments);
		return (obj);
	}

	/*
	 * For convenience and backwards compatibility, we support several
	 * different calling forms.  Normalize them here.
	 */
	parsed = parseConstructorArguments({
	    'argv': args,
	    'strict': false
	});

	/*
	 * If we've been given a name, apply it now.
	 */
	if (parsed.options.name) {
		mod_assertplus.string(parsed.options.name,
		    'error\'s "name" must be a string');
		this.name = parsed.options.name;
	}

	/*
	 * For debugging, we keep track of the original short message (attached
	 * this Error particularly) separately from the complete message (which
	 * includes the messages of our cause chain).
	 */
	this.jse_shortmsg = parsed.shortmessage;
	message = parsed.shortmessage;

	/*
	 * If we've been given a cause, record a reference to it and update our
	 * message appropriately.
	 */
	cause = parsed.options.cause;
	if (cause) {
		mod_assertplus.ok(mod_isError(cause), 'cause is not an Error');
		this.jse_cause = cause;

		if (!parsed.options.skipCauseMessage) {
			message += ': ' + cause.message;
		}
	}

	/*
	 * If we've been given an object with properties, shallow-copy that
	 * here.  We don't want to use a deep copy in case there are non-plain
	 * objects here, but we don't want to use the original object in case
	 * the caller modifies it later.
	 */
	this.jse_info = {};
	if (parsed.options.info) {
		for (k in parsed.options.info) {
			this.jse_info[k] = parsed.options.info[k];
		}
	}

	this.message = message;
	Error.call(this, message);

	if (Error.captureStackTrace) {
		ctor = parsed.options.constructorOpt || this.constructor;
		Error.captureStackTrace(this, ctor);
	}

	return (this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.verror.WError"></a>[module verror.WError](#apidoc.module.verror.WError)

#### <a name="apidoc.element.verror.WError.WError"></a>[function <span class="apidocSignatureSpan">verror.</span>WError ()](#apidoc.element.verror.WError.WError)
- description and source-code
```javascript
function WError()
{
	var args, obj, parsed, options;

	args = Array.prototype.slice.call(arguments, 0);
	if (!(this instanceof WError)) {
		obj = Object.create(WError.prototype);
		WError.apply(obj, args);
		return (obj);
	}

	parsed = parseConstructorArguments({
	    'argv': args,
	    'strict': false
	});

	options = parsed.options;
	options['skipCauseMessage'] = true;
	VError.call(this, options, '%s', parsed.shortmessage);

	return (this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.verror.WError.super_"></a>[function <span class="apidocSignatureSpan">verror.WError.</span>super_ ()](#apidoc.element.verror.WError.super_)
- description and source-code
```javascript
function VError()
{
	var args, obj, parsed, cause, ctor, message, k;

	args = Array.prototype.slice.call(arguments, 0);

	<span class="apidocCodeCommentSpan">/*
	 * This is a regrettable pattern, but JavaScript's built-in Error class
	 * is defined to work this way, so we allow the constructor to be called
	 * without "new".
	 */
</span>	if (!(this instanceof VError)) {
		obj = Object.create(VError.prototype);
		VError.apply(obj, arguments);
		return (obj);
	}

	/*
	 * For convenience and backwards compatibility, we support several
	 * different calling forms.  Normalize them here.
	 */
	parsed = parseConstructorArguments({
	    'argv': args,
	    'strict': false
	});

	/*
	 * If we've been given a name, apply it now.
	 */
	if (parsed.options.name) {
		mod_assertplus.string(parsed.options.name,
		    'error\'s "name" must be a string');
		this.name = parsed.options.name;
	}

	/*
	 * For debugging, we keep track of the original short message (attached
	 * this Error particularly) separately from the complete message (which
	 * includes the messages of our cause chain).
	 */
	this.jse_shortmsg = parsed.shortmessage;
	message = parsed.shortmessage;

	/*
	 * If we've been given a cause, record a reference to it and update our
	 * message appropriately.
	 */
	cause = parsed.options.cause;
	if (cause) {
		mod_assertplus.ok(mod_isError(cause), 'cause is not an Error');
		this.jse_cause = cause;

		if (!parsed.options.skipCauseMessage) {
			message += ': ' + cause.message;
		}
	}

	/*
	 * If we've been given an object with properties, shallow-copy that
	 * here.  We don't want to use a deep copy in case there are non-plain
	 * objects here, but we don't want to use the original object in case
	 * the caller modifies it later.
	 */
	this.jse_info = {};
	if (parsed.options.info) {
		for (k in parsed.options.info) {
			this.jse_info[k] = parsed.options.info[k];
		}
	}

	this.message = message;
	Error.call(this, message);

	if (Error.captureStackTrace) {
		ctor = parsed.options.constructorOpt || this.constructor;
		Error.captureStackTrace(this, ctor);
	}

	return (this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.verror.WError.prototype"></a>[module verror.WError.prototype](#apidoc.module.verror.WError.prototype)

#### <a name="apidoc.element.verror.WError.prototype.cause"></a>[function <span class="apidocSignatureSpan">verror.WError.prototype.</span>cause (c)](#apidoc.element.verror.WError.prototype.cause)
- description and source-code
```javascript
function we_cause(c)
{
	if (mod_isError(c))
		this.jse_cause = c;

	return (this.jse_cause);
}
```
- example usage
```shell
...
    sort: open failed: /nonexistent: No such file or directory

To match the Unixy feel, when you print out the error, just prepend the
program's name to the VError's 'message'.  Or just call
[node-cmdutil.fail(your_verror)](https://github.com/joyent/node-cmdutil), which
does this for you.

You can get the next-level Error using 'err.cause()':

'''javascript
console.error(err2.cause().message);
'''

prints:
...
```

#### <a name="apidoc.element.verror.WError.prototype.toString"></a>[function <span class="apidocSignatureSpan">verror.WError.prototype.</span>toString ()](#apidoc.element.verror.WError.prototype.toString)
- description and source-code
```javascript
function we_toString()
{
	var str = (this.hasOwnProperty('name') && this.name ||
		this.constructor.name || this.constructor.prototype.name);
	if (this.message)
		str += ': ' + this.message;
	if (this.jse_cause && this.jse_cause.message)
		str += '; caused by ' + this.jse_cause.toString();

	return (str);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.verror.super_"></a>[module verror.super_](#apidoc.module.verror.super_)

#### <a name="apidoc.element.verror.super_.super_"></a>[function <span class="apidocSignatureSpan">verror.</span>super_ ()](#apidoc.element.verror.super_.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.verror.super_.captureStackTrace"></a>[function <span class="apidocSignatureSpan">verror.super_.</span>captureStackTrace ()](#apidoc.element.verror.super_.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace() { [native code] }
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
