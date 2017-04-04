# api documentation for  [random-js (v1.0.8)](https://github.com/ckknight/random-js)  [![npm package](https://img.shields.io/npm/v/npmdoc-random-js.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-random-js) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-random-js.svg)](https://travis-ci.org/npmdoc/node-npmdoc-random-js)
#### A mathematically correct random number generator library for JavaScript.

[![NPM](https://nodei.co/npm/random-js.png?downloads=true)](https://www.npmjs.com/package/random-js)

[![apidoc](https://npmdoc.github.io/node-npmdoc-random-js/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-random-js_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-random-js/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-random-js/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-random-js/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Cameron Kenneth Knight",
        "email": "ckknight@gmail.com"
    },
    "bugs": {
        "url": "https://github.com/ckknight/random-js/issues"
    },
    "dependencies": {},
    "description": "A mathematically correct random number generator library for JavaScript.",
    "devDependencies": {
        "karma": "~0.10.9",
        "karma-chrome-launcher": "~0.1.2",
        "karma-coffee-preprocessor": "~0.1.2",
        "karma-coverage": "~0.1.5",
        "karma-firefox-launcher": "~0.1.3",
        "karma-html2js-preprocessor": "~0.1.0",
        "karma-jasmine": "~0.1.5",
        "karma-phantomjs-launcher": "~0.1.1",
        "karma-requirejs": "~0.2.1",
        "karma-script-launcher": "~0.1.0",
        "requirejs": "~2.1.10"
    },
    "directories": {},
    "dist": {
        "shasum": "968fd689a6f25d6c0aac766283de2f688c9c190a",
        "tarball": "https://registry.npmjs.org/random-js/-/random-js-1.0.8.tgz"
    },
    "gitHead": "8a51f321c1fb1725a593fec59299af6ad7118631",
    "homepage": "https://github.com/ckknight/random-js",
    "keywords": [
        "random"
    ],
    "license": "MIT",
    "main": "lib/random",
    "maintainers": [
        {
            "name": "ckknight",
            "email": "ckknight@gmail.com"
        }
    ],
    "name": "random-js",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/ckknight/random-js.git"
    },
    "scripts": {
        "test": "jasmine-node lib/random.js spec/",
        "uglify": "uglifyjs lib/random.js -o lib/random.min.js -m -c"
    },
    "testling": {
        "files": "spec/*.js"
    },
    "version": "1.0.8"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module random-js](#apidoc.module.random-js)
1.  [function <span class="apidocSignatureSpan">random-js.</span>bool (numerator, denominator)](#apidoc.element.random-js.bool)
1.  [function <span class="apidocSignatureSpan">random-js.</span>date (start, end)](#apidoc.element.random-js.date)
1.  [function <span class="apidocSignatureSpan">random-js.</span>dice (sideCount, dieCount)](#apidoc.element.random-js.dice)
1.  [function <span class="apidocSignatureSpan">random-js.</span>die (sideCount)](#apidoc.element.random-js.die)
1.  [function <span class="apidocSignatureSpan">random-js.</span>generateEntropyArray ()](#apidoc.element.random-js.generateEntropyArray)
1.  [function <span class="apidocSignatureSpan">random-js.</span>hex (upper)](#apidoc.element.random-js.hex)
1.  [function <span class="apidocSignatureSpan">random-js.</span>int32 (engine)](#apidoc.element.random-js.int32)
1.  [function <span class="apidocSignatureSpan">random-js.</span>int53 (engine)](#apidoc.element.random-js.int53)
1.  [function <span class="apidocSignatureSpan">random-js.</span>int53Full (engine)](#apidoc.element.random-js.int53Full)
1.  [function <span class="apidocSignatureSpan">random-js.</span>integer (min, max)](#apidoc.element.random-js.integer)
1.  [function <span class="apidocSignatureSpan">random-js.</span>pick (engine, array, begin, end)](#apidoc.element.random-js.pick)
1.  [function <span class="apidocSignatureSpan">random-js.</span>picker (array, begin, end)](#apidoc.element.random-js.picker)
1.  [function <span class="apidocSignatureSpan">random-js.</span>real (left, right, inclusive)](#apidoc.element.random-js.real)
1.  [function <span class="apidocSignatureSpan">random-js.</span>realZeroToOneExclusive (engine)](#apidoc.element.random-js.realZeroToOneExclusive)
1.  [function <span class="apidocSignatureSpan">random-js.</span>realZeroToOneInclusive (engine)](#apidoc.element.random-js.realZeroToOneInclusive)
1.  [function <span class="apidocSignatureSpan">random-js.</span>sample (engine, population, sampleSize)](#apidoc.element.random-js.sample)
1.  [function <span class="apidocSignatureSpan">random-js.</span>shuffle (engine, array, downTo)](#apidoc.element.random-js.shuffle)
1.  [function <span class="apidocSignatureSpan">random-js.</span>string (pool)](#apidoc.element.random-js.string)
1.  [function <span class="apidocSignatureSpan">random-js.</span>uint32 (engine)](#apidoc.element.random-js.uint32)
1.  [function <span class="apidocSignatureSpan">random-js.</span>uint53 (engine)](#apidoc.element.random-js.uint53)
1.  [function <span class="apidocSignatureSpan">random-js.</span>uint53Full (engine)](#apidoc.element.random-js.uint53Full)
1.  [function <span class="apidocSignatureSpan">random-js.</span>uuid4 (engine)](#apidoc.element.random-js.uuid4)
1.  object <span class="apidocSignatureSpan">random-js.</span>engines

#### [module random-js.engines](#apidoc.module.random-js.engines)
1.  [function <span class="apidocSignatureSpan">random-js.engines.</span>mt19937 ()](#apidoc.element.random-js.engines.mt19937)
1.  [function <span class="apidocSignatureSpan">random-js.engines.</span>nativeMath ()](#apidoc.element.random-js.engines.nativeMath)
1.  object <span class="apidocSignatureSpan">random-js.engines.</span>browserCrypto



# <a name="apidoc.module.random-js"></a>[module random-js](#apidoc.module.random-js)

#### <a name="apidoc.element.random-js.bool"></a>[function <span class="apidocSignatureSpan">random-js.</span>bool (numerator, denominator)](#apidoc.element.random-js.bool)
- description and source-code
```javascript
bool = function (numerator, denominator) {
  if (denominator == null) {
    if (numerator == null) {
      return isLeastBitTrue;
    }
    return probability(numerator);
  } else {
    if (numerator <= 0) {
      return returnValue(false);
    } else if (numerator >= denominator) {
      return returnValue(true);
    }
    return lessThan(Random.integer(0, denominator - 1), numerator);
  }
}
```
- example usage
```shell
...

### Distributions

Random.js also provides a set of methods for producing useful data from an engine.

* 'Random.integer(min, max)(engine)': Produce an integer within the inclusive range ['min', 'max']. 'min' can be at its minimum -
9007199254740992 (-2 ** 53). 'max' can be at its maximum 9007199254740992 (2 ** 53).
* 'Random.real(min, max, inclusive)(engine)': Produce a floating point number within the range ['min', 'max') or ['min', 'max'].
Uses 53 bits of randomness.
* 'Random.bool()(engine)': Produce a boolean with a 50% chance of it being 'true'.
* 'Random.bool(percentage)(engine)': Produce a boolean with the specified chance causing it to be 'true'.
* 'Random.bool(numerator, denominator)(engine)': Produce a boolean with 'numerator'/'denominator' chance of it being true.
* 'Random.pick(engine, array[, begin[, end]])': Return a random value within the provided 'array' within the sliced bounds of 'begin
' and 'end'.
* 'Random.picker(array[, begin[, end]])(engine)': Same as 'Random.pick(engine, array, begin, end)'.
* 'Random.shuffle(engine, array)': Shuffle the provided 'array' (in-place). Similar to '.sort()'.
* 'Random.sample(engine, population, sampleSize)': From the 'population' array, produce an array with 'sampleSize' elements that
 are randomly chosen without repeats.
* 'Random.die(sideCount)(engine)': Same as 'Random.integer(1, sideCount)(engine)'
...
```

#### <a name="apidoc.element.random-js.date"></a>[function <span class="apidocSignatureSpan">random-js.</span>date (start, end)](#apidoc.element.random-js.date)
- description and source-code
```javascript
date = function (start, end) {
  if (!(start instanceof Date)) {
    throw new TypeError("Expected start to be a Date, got " + typeof start);
  } else if (!(end instanceof Date)) {
    throw new TypeError("Expected end to be a Date, got " + typeof end);
  }
  var distribution = Random.integer(start.getTime(), end.getTime());
  return function (engine) {
    return new Date(distribution(engine));
  };
}
```
- example usage
```shell
...
 * 'Random.die(sideCount)(engine)': Same as 'Random.integer(1, sideCount)(engine)'
 * 'Random.dice(sideCount, dieCount)(engine)': Produce an array of length 'dieCount' with as many 'die' rolls.
 * 'Random.uuid4(engine)': Produce a [Universally Unique Identifier](http://en.wikipedia.org/wiki/Universally_unique_identifier)
Version 4.
 * 'Random.string()(engine, length)': Produce a random string using numbers, uppercase and lowercase letters, '_', and '-' of length
 'length'.
 * 'Random.string(pool)(engine, length)': Produce a random string using the provided string 'pool' as the possible characters to
 choose from of length 'length'.
 * 'Random.hex()(engine, length)' or 'Random.hex(false)(engine, length)': Produce a random string comprised of numbers or the characters
 'abcdef' of length 'length'.
 * 'Random.hex(true)(engine, length)': Produce a random string comprised of numbers or the characters 'ABCDEF' of length 'length
'.
 * 'Random.date(start, end)(engine)': Produce a random 'Date' within the inclusive range of ['start', 'end']. 'start' and 'end'
must both be 'Date's.

An example of using 'integer' would be as such:

// create a Mersenne Twister-19937 that is auto-seeded based on time and other random values
var engine = Random.engines.mt19937().autoSeed();
// create a distribution that will consistently produce integers within inclusive range [0, 99].
var distribution = Random.integer(0, 99);
...
```

#### <a name="apidoc.element.random-js.dice"></a>[function <span class="apidocSignatureSpan">random-js.</span>dice (sideCount, dieCount)](#apidoc.element.random-js.dice)
- description and source-code
```javascript
dice = function (sideCount, dieCount) {
  var distribution = Random.die(sideCount);
  return function (engine) {
    var result = [];
    result.length = dieCount;
    for (var i = 0; i < dieCount; ++i) {
      result[i] = distribution(engine);
    }
    return result;
  };
}
```
- example usage
```shell
...
* 'Random.bool(percentage)(engine)': Produce a boolean with the specified chance causing it to be 'true'.
* 'Random.bool(numerator, denominator)(engine)': Produce a boolean with 'numerator'/'denominator' chance of it being true.
* 'Random.pick(engine, array[, begin[, end]])': Return a random value within the provided 'array' within the sliced bounds of 'begin
' and 'end'.
* 'Random.picker(array[, begin[, end]])(engine)': Same as 'Random.pick(engine, array, begin, end)'.
* 'Random.shuffle(engine, array)': Shuffle the provided 'array' (in-place). Similar to '.sort()'.
* 'Random.sample(engine, population, sampleSize)': From the 'population' array, produce an array with 'sampleSize' elements that
 are randomly chosen without repeats.
* 'Random.die(sideCount)(engine)': Same as 'Random.integer(1, sideCount)(engine)'
* 'Random.dice(sideCount, dieCount)(engine)': Produce an array of length 'dieCount' with as many 'die' rolls.
* 'Random.uuid4(engine)': Produce a [Universally Unique Identifier](http://en.wikipedia.org/wiki/Universally_unique_identifier)
Version 4.
* 'Random.string()(engine, length)': Produce a random string using numbers, uppercase and lowercase letters, '_', and '-' of length
 'length'.
* 'Random.string(pool)(engine, length)': Produce a random string using the provided string 'pool' as the possible characters to
choose from of length 'length'.
* 'Random.hex()(engine, length)' or 'Random.hex(false)(engine, length)': Produce a random string comprised of numbers or the characters
 'abcdef' of length 'length'.
* 'Random.hex(true)(engine, length)': Produce a random string comprised of numbers or the characters 'ABCDEF' of length 'length'.
* 'Random.date(start, end)(engine)': Produce a random 'Date' within the inclusive range of ['start', 'end']. 'start' and 'end' must
 both be 'Date's.
...
```

#### <a name="apidoc.element.random-js.die"></a>[function <span class="apidocSignatureSpan">random-js.</span>die (sideCount)](#apidoc.element.random-js.die)
- description and source-code
```javascript
die = function (sideCount) {
  return Random.integer(1, sideCount);
}
```
- example usage
```shell
...
* 'Random.bool()(engine)': Produce a boolean with a 50% chance of it being 'true'.
* 'Random.bool(percentage)(engine)': Produce a boolean with the specified chance causing it to be 'true'.
* 'Random.bool(numerator, denominator)(engine)': Produce a boolean with 'numerator'/'denominator' chance of it being true.
* 'Random.pick(engine, array[, begin[, end]])': Return a random value within the provided 'array' within the sliced bounds of 'begin
' and 'end'.
* 'Random.picker(array[, begin[, end]])(engine)': Same as 'Random.pick(engine, array, begin, end)'.
* 'Random.shuffle(engine, array)': Shuffle the provided 'array' (in-place). Similar to '.sort()'.
* 'Random.sample(engine, population, sampleSize)': From the 'population' array, produce an array with 'sampleSize' elements that
 are randomly chosen without repeats.
* 'Random.die(sideCount)(engine)': Same as 'Random.integer(1, sideCount)(engine)'
* 'Random.dice(sideCount, dieCount)(engine)': Produce an array of length 'dieCount' with as many 'die' rolls.
* 'Random.uuid4(engine)': Produce a [Universally Unique Identifier](http://en.wikipedia.org/wiki/Universally_unique_identifier)
Version 4.
* 'Random.string()(engine, length)': Produce a random string using numbers, uppercase and lowercase letters, '_', and '-' of length
 'length'.
* 'Random.string(pool)(engine, length)': Produce a random string using the provided string 'pool' as the possible characters to
choose from of length 'length'.
* 'Random.hex()(engine, length)' or 'Random.hex(false)(engine, length)': Produce a random string comprised of numbers or the characters
 'abcdef' of length 'length'.
* 'Random.hex(true)(engine, length)': Produce a random string comprised of numbers or the characters 'ABCDEF' of length 'length'.
* 'Random.date(start, end)(engine)': Produce a random 'Date' within the inclusive range of ['start', 'end']. 'start' and 'end' must
 both be 'Date's.
...
```

#### <a name="apidoc.element.random-js.generateEntropyArray"></a>[function <span class="apidocSignatureSpan">random-js.</span>generateEntropyArray ()](#apidoc.element.random-js.generateEntropyArray)
- description and source-code
```javascript
generateEntropyArray = function () {
  var array = [];
  var engine = Random.engines.nativeMath;
  for (var i = 0; i < 16; ++i) {
    array[i] = engine() | 0;
  }
  array.push(new Date().getTime() | 0);
  return array;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.random-js.hex"></a>[function <span class="apidocSignatureSpan">random-js.</span>hex (upper)](#apidoc.element.random-js.hex)
- description and source-code
```javascript
hex = function (upper) {
  if (upper) {
    return upperHex;
  } else {
    return lowerHex;
  }
}
```
- example usage
```shell
...
 * 'Random.shuffle(engine, array)': Shuffle the provided 'array' (in-place). Similar to '.sort()'.
 * 'Random.sample(engine, population, sampleSize)': From the 'population' array, produce an array with 'sampleSize' elements that
 are randomly chosen without repeats.
 * 'Random.die(sideCount)(engine)': Same as 'Random.integer(1, sideCount)(engine)'
 * 'Random.dice(sideCount, dieCount)(engine)': Produce an array of length 'dieCount' with as many 'die' rolls.
 * 'Random.uuid4(engine)': Produce a [Universally Unique Identifier](http://en.wikipedia.org/wiki/Universally_unique_identifier)
Version 4.
 * 'Random.string()(engine, length)': Produce a random string using numbers, uppercase and lowercase letters, '_', and '-' of length
 'length'.
 * 'Random.string(pool)(engine, length)': Produce a random string using the provided string 'pool' as the possible characters to
 choose from of length 'length'.
 * 'Random.hex()(engine, length)' or 'Random.hex(false)(engine, length)': Produce a random string comprised of numbers or the characters
 'abcdef' of length 'length'.
 * 'Random.hex(true)(engine, length)': Produce a random string comprised of numbers or the characters 'ABCDEF' of length 'length
'.
 * 'Random.date(start, end)(engine)': Produce a random 'Date' within the inclusive range of ['start', 'end']. 'start' and 'end'
must both be 'Date's.

An example of using 'integer' would be as such:

// create a Mersenne Twister-19937 that is auto-seeded based on time and other random values
var engine = Random.engines.mt19937().autoSeed();
...
```

#### <a name="apidoc.element.random-js.int32"></a>[function <span class="apidocSignatureSpan">random-js.</span>int32 (engine)](#apidoc.element.random-js.int32)
- description and source-code
```javascript
int32 = function (engine) {
  return engine() | 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.random-js.int53"></a>[function <span class="apidocSignatureSpan">random-js.</span>int53 (engine)](#apidoc.element.random-js.int53)
- description and source-code
```javascript
int53 = function (engine) {
  var high = engine() | 0;
  var low = engine() >>> 0;
  return ((high & 0x1fffff) * 0x100000000) + low + (high & 0x200000 ? -0x20000000000000 : 0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.random-js.int53Full"></a>[function <span class="apidocSignatureSpan">random-js.</span>int53Full (engine)](#apidoc.element.random-js.int53Full)
- description and source-code
```javascript
int53Full = function (engine) {
  while (true) {
    var high = engine() | 0;
    if (high & 0x400000) {
      if ((high & 0x7fffff) === 0x400000 && (engine() | 0) === 0) {
        return 0x20000000000000;
      }
    } else {
      var low = engine() >>> 0;
      return ((high & 0x1fffff) * 0x100000000) + low + (high & 0x200000 ? -0x20000000000000 : 0);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.random-js.integer"></a>[function <span class="apidocSignatureSpan">random-js.</span>integer (min, max)](#apidoc.element.random-js.integer)
- description and source-code
```javascript
integer = function (min, max) {
  min = Math.floor(min);
  max = Math.floor(max);
  if (min < -0x20000000000000 || !isFinite(min)) {
    throw new RangeError("Expected min to be at least " + (-0x20000000000000));
  } else if (max > 0x20000000000000 || !isFinite(max)) {
    throw new RangeError("Expected max to be at most " + 0x20000000000000);
  }

  var range = max - min;
  if (range <= 0 || !isFinite(range)) {
    return returnValue(min);
  } else if (range === 0xffffffff) {
    if (min === 0) {
      return Random.uint32;
    } else {
      return add(Random.int32, min + 0x80000000);
    }
  } else if (range < 0xffffffff) {
    return add(downscaleToRange(range), min);
  } else if (range === 0x1fffffffffffff) {
    return add(Random.uint53, min);
  } else if (range < 0x1fffffffffffff) {
    return add(upscaleWithinU53(range), min);
  } else if (max - 1 - min === 0x1fffffffffffff) {
    return add(Random.uint53Full, min);
  } else if (min === -0x20000000000000 && max === 0x20000000000000) {
    return Random.int53Full;
  } else if (min === -0x20000000000000 && max === 0x1fffffffffffff) {
    return Random.int53;
  } else if (min === -0x1fffffffffffff && max === 0x20000000000000) {
    return add(Random.int53, 1);
  } else if (max === 0x20000000000000) {
    return add(upscaleWithinI53AndLoopCheck(min - 1, max - 1), 1);
  } else {
    return upscaleWithinI53AndLoopCheck(min, max);
  }
}
```
- example usage
```shell
...

One can seed a Mersenne Twister with the same value ('mt.seed(value)') or values ('mt.seedWithArray(array)') and discard the number
 of uses ('mt.getUseCount()') to achieve the exact same state.

### Distributions

Random.js also provides a set of methods for producing useful data from an engine.

* 'Random.integer(min, max)(engine)': Produce an integer within the inclusive range ['min', 'max']. 'min' can be at its minimum -
9007199254740992 (-2 ** 53). 'max' can be at its maximum 9007199254740992 (2 ** 53).
* 'Random.real(min, max, inclusive)(engine)': Produce a floating point number within the range ['min', 'max') or ['min', 'max'].
Uses 53 bits of randomness.
* 'Random.bool()(engine)': Produce a boolean with a 50% chance of it being 'true'.
* 'Random.bool(percentage)(engine)': Produce a boolean with the specified chance causing it to be 'true'.
* 'Random.bool(numerator, denominator)(engine)': Produce a boolean with 'numerator'/'denominator' chance of it being true.
* 'Random.pick(engine, array[, begin[, end]])': Return a random value within the provided 'array' within the sliced bounds of 'begin
' and 'end'.
* 'Random.picker(array[, begin[, end]])(engine)': Same as 'Random.pick(engine, array, begin, end)'.
* 'Random.shuffle(engine, array)': Shuffle the provided 'array' (in-place). Similar to '.sort()'.
...
```

#### <a name="apidoc.element.random-js.pick"></a>[function <span class="apidocSignatureSpan">random-js.</span>pick (engine, array, begin, end)](#apidoc.element.random-js.pick)
- description and source-code
```javascript
pick = function (engine, array, begin, end) {
  var length = array.length;
  var start = begin == null ? 0 : convertSliceArgument(toInteger(begin), length);
  var finish = end === void 0 ? length : convertSliceArgument(toInteger(end), length);
  if (start >= finish) {
    return void 0;
  }
  var distribution = Random.integer(start, finish - 1);
  return array[distribution(engine)];
}
```
- example usage
```shell
...
Random.js also provides a set of methods for producing useful data from an engine.

* 'Random.integer(min, max)(engine)': Produce an integer within the inclusive range ['min', 'max']. 'min' can be at its minimum -
9007199254740992 (-2 ** 53). 'max' can be at its maximum 9007199254740992 (2 ** 53).
* 'Random.real(min, max, inclusive)(engine)': Produce a floating point number within the range ['min', 'max') or ['min', 'max'].
Uses 53 bits of randomness.
* 'Random.bool()(engine)': Produce a boolean with a 50% chance of it being 'true'.
* 'Random.bool(percentage)(engine)': Produce a boolean with the specified chance causing it to be 'true'.
* 'Random.bool(numerator, denominator)(engine)': Produce a boolean with 'numerator'/'denominator' chance of it being true.
* 'Random.pick(engine, array[, begin[, end]])': Return a random value within the provided 'array' within the sliced bounds of 'begin
' and 'end'.
* 'Random.picker(array[, begin[, end]])(engine)': Same as 'Random.pick(engine, array, begin, end)'.
* 'Random.shuffle(engine, array)': Shuffle the provided 'array' (in-place). Similar to '.sort()'.
* 'Random.sample(engine, population, sampleSize)': From the 'population' array, produce an array with 'sampleSize' elements that
 are randomly chosen without repeats.
* 'Random.die(sideCount)(engine)': Same as 'Random.integer(1, sideCount)(engine)'
* 'Random.dice(sideCount, dieCount)(engine)': Produce an array of length 'dieCount' with as many 'die' rolls.
* 'Random.uuid4(engine)': Produce a [Universally Unique Identifier](http://en.wikipedia.org/wiki/Universally_unique_identifier)
Version 4.
* 'Random.string()(engine, length)': Produce a random string using numbers, uppercase and lowercase letters, '_', and '-' of length
 'length'.
...
```

#### <a name="apidoc.element.random-js.picker"></a>[function <span class="apidocSignatureSpan">random-js.</span>picker (array, begin, end)](#apidoc.element.random-js.picker)
- description and source-code
```javascript
picker = function (array, begin, end) {
  var clone = slice.call(array, begin, end);
  if (!clone.length) {
    return returnUndefined;
  }
  var distribution = Random.integer(0, clone.length - 1);
  return function (engine) {
    return clone[distribution(engine)];
  };
}
```
- example usage
```shell
...

* 'Random.integer(min, max)(engine)': Produce an integer within the inclusive range ['min', 'max']. 'min' can be at its minimum -
9007199254740992 (-2 ** 53). 'max' can be at its maximum 9007199254740992 (2 ** 53).
* 'Random.real(min, max, inclusive)(engine)': Produce a floating point number within the range ['min', 'max') or ['min', 'max'].
Uses 53 bits of randomness.
* 'Random.bool()(engine)': Produce a boolean with a 50% chance of it being 'true'.
* 'Random.bool(percentage)(engine)': Produce a boolean with the specified chance causing it to be 'true'.
* 'Random.bool(numerator, denominator)(engine)': Produce a boolean with 'numerator'/'denominator' chance of it being true.
* 'Random.pick(engine, array[, begin[, end]])': Return a random value within the provided 'array' within the sliced bounds of 'begin
' and 'end'.
* 'Random.picker(array[, begin[, end]])(engine)': Same as 'Random.pick(engine, array, begin, end)'.
* 'Random.shuffle(engine, array)': Shuffle the provided 'array' (in-place). Similar to '.sort()'.
* 'Random.sample(engine, population, sampleSize)': From the 'population' array, produce an array with 'sampleSize' elements that
 are randomly chosen without repeats.
* 'Random.die(sideCount)(engine)': Same as 'Random.integer(1, sideCount)(engine)'
* 'Random.dice(sideCount, dieCount)(engine)': Produce an array of length 'dieCount' with as many 'die' rolls.
* 'Random.uuid4(engine)': Produce a [Universally Unique Identifier](http://en.wikipedia.org/wiki/Universally_unique_identifier)
Version 4.
* 'Random.string()(engine, length)': Produce a random string using numbers, uppercase and lowercase letters, '_', and '-' of length
 'length'.
* 'Random.string(pool)(engine, length)': Produce a random string using the provided string 'pool' as the possible characters to
choose from of length 'length'.
...
```

#### <a name="apidoc.element.random-js.real"></a>[function <span class="apidocSignatureSpan">random-js.</span>real (left, right, inclusive)](#apidoc.element.random-js.real)
- description and source-code
```javascript
real = function (left, right, inclusive) {
  if (!isFinite(left)) {
    throw new RangeError("Expected left to be a finite number");
  } else if (!isFinite(right)) {
    throw new RangeError("Expected right to be a finite number");
  }
  return add(
    multiply(
      inclusive ? Random.realZeroToOneInclusive : Random.realZeroToOneExclusive,
      right - left),
    left);
}
```
- example usage
```shell
...
One can seed a Mersenne Twister with the same value ('mt.seed(value)') or values ('mt.seedWithArray(array)') and discard the number
 of uses ('mt.getUseCount()') to achieve the exact same state.

### Distributions

Random.js also provides a set of methods for producing useful data from an engine.

* 'Random.integer(min, max)(engine)': Produce an integer within the inclusive range ['min', 'max']. 'min' can be at its minimum -
9007199254740992 (-2 ** 53). 'max' can be at its maximum 9007199254740992 (2 ** 53).
* 'Random.real(min, max, inclusive)(engine)': Produce a floating point number within the range ['min', 'max') or ['min', 'max'].
Uses 53 bits of randomness.
* 'Random.bool()(engine)': Produce a boolean with a 50% chance of it being 'true'.
* 'Random.bool(percentage)(engine)': Produce a boolean with the specified chance causing it to be 'true'.
* 'Random.bool(numerator, denominator)(engine)': Produce a boolean with 'numerator'/'denominator' chance of it being true.
* 'Random.pick(engine, array[, begin[, end]])': Return a random value within the provided 'array' within the sliced bounds of 'begin
' and 'end'.
* 'Random.picker(array[, begin[, end]])(engine)': Same as 'Random.pick(engine, array, begin, end)'.
* 'Random.shuffle(engine, array)': Shuffle the provided 'array' (in-place). Similar to '.sort()'.
* 'Random.sample(engine, population, sampleSize)': From the 'population' array, produce an array with 'sampleSize' elements that
 are randomly chosen without repeats.
...
```

#### <a name="apidoc.element.random-js.realZeroToOneExclusive"></a>[function <span class="apidocSignatureSpan">random-js.</span>realZeroToOneExclusive (engine)](#apidoc.element.random-js.realZeroToOneExclusive)
- description and source-code
```javascript
realZeroToOneExclusive = function (engine) {
  return Random.uint53(engine) / 0x20000000000000;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.random-js.realZeroToOneInclusive"></a>[function <span class="apidocSignatureSpan">random-js.</span>realZeroToOneInclusive (engine)](#apidoc.element.random-js.realZeroToOneInclusive)
- description and source-code
```javascript
realZeroToOneInclusive = function (engine) {
  return Random.uint53Full(engine) / 0x20000000000000;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.random-js.sample"></a>[function <span class="apidocSignatureSpan">random-js.</span>sample (engine, population, sampleSize)](#apidoc.element.random-js.sample)
- description and source-code
```javascript
sample = function (engine, population, sampleSize) {
  if (sampleSize < 0 || sampleSize > population.length || !isFinite(sampleSize)) {
    throw new RangeError("Expected sampleSize to be within 0 and the length of the population");
  }

  if (sampleSize === 0) {
    return [];
  }

  var clone = slice.call(population);
  var length = clone.length;
  if (length === sampleSize) {
    return Random.shuffle(engine, clone, 0);
  }
  var tailLength = length - sampleSize;
  return Random.shuffle(engine, clone, tailLength - 1).slice(tailLength);
}
```
- example usage
```shell
...
* 'Random.real(min, max, inclusive)(engine)': Produce a floating point number within the range ['min', 'max') or ['min', 'max'].
Uses 53 bits of randomness.
* 'Random.bool()(engine)': Produce a boolean with a 50% chance of it being 'true'.
* 'Random.bool(percentage)(engine)': Produce a boolean with the specified chance causing it to be 'true'.
* 'Random.bool(numerator, denominator)(engine)': Produce a boolean with 'numerator'/'denominator' chance of it being true.
* 'Random.pick(engine, array[, begin[, end]])': Return a random value within the provided 'array' within the sliced bounds of 'begin
' and 'end'.
* 'Random.picker(array[, begin[, end]])(engine)': Same as 'Random.pick(engine, array, begin, end)'.
* 'Random.shuffle(engine, array)': Shuffle the provided 'array' (in-place). Similar to '.sort()'.
* 'Random.sample(engine, population, sampleSize)': From the 'population' array, produce an array with 'sampleSize' elements that
 are randomly chosen without repeats.
* 'Random.die(sideCount)(engine)': Same as 'Random.integer(1, sideCount)(engine)'
* 'Random.dice(sideCount, dieCount)(engine)': Produce an array of length 'dieCount' with as many 'die' rolls.
* 'Random.uuid4(engine)': Produce a [Universally Unique Identifier](http://en.wikipedia.org/wiki/Universally_unique_identifier)
Version 4.
* 'Random.string()(engine, length)': Produce a random string using numbers, uppercase and lowercase letters, '_', and '-' of length
 'length'.
* 'Random.string(pool)(engine, length)': Produce a random string using the provided string 'pool' as the possible characters to
choose from of length 'length'.
* 'Random.hex()(engine, length)' or 'Random.hex(false)(engine, length)': Produce a random string comprised of numbers or the characters
 'abcdef' of length 'length'.
* 'Random.hex(true)(engine, length)': Produce a random string comprised of numbers or the characters 'ABCDEF' of length 'length'.
...
```

#### <a name="apidoc.element.random-js.shuffle"></a>[function <span class="apidocSignatureSpan">random-js.</span>shuffle (engine, array, downTo)](#apidoc.element.random-js.shuffle)
- description and source-code
```javascript
shuffle = function (engine, array, downTo) {
  var length = array.length;
  if (length) {
    if (downTo == null) {
      downTo = 0;
    }
    for (var i = (length - 1) >>> 0; i > downTo; --i) {
      var distribution = Random.integer(0, i);
      var j = distribution(engine);
      if (i !== j) {
        var tmp = array[i];
        array[i] = array[j];
        array[j] = tmp;
      }
    }
  }
  return array;
}
```
- example usage
```shell
...
* 'Random.integer(min, max)(engine)': Produce an integer within the inclusive range ['min', 'max']. 'min' can be at its minimum -
9007199254740992 (-2 ** 53). 'max' can be at its maximum 9007199254740992 (2 ** 53).
* 'Random.real(min, max, inclusive)(engine)': Produce a floating point number within the range ['min', 'max') or ['min', 'max'].
Uses 53 bits of randomness.
* 'Random.bool()(engine)': Produce a boolean with a 50% chance of it being 'true'.
* 'Random.bool(percentage)(engine)': Produce a boolean with the specified chance causing it to be 'true'.
* 'Random.bool(numerator, denominator)(engine)': Produce a boolean with 'numerator'/'denominator' chance of it being true.
* 'Random.pick(engine, array[, begin[, end]])': Return a random value within the provided 'array' within the sliced bounds of 'begin
' and 'end'.
* 'Random.picker(array[, begin[, end]])(engine)': Same as 'Random.pick(engine, array, begin, end)'.
* 'Random.shuffle(engine, array)': Shuffle the provided 'array' (in-place). Similar to '.sort()'.
* 'Random.sample(engine, population, sampleSize)': From the 'population' array, produce an array with 'sampleSize' elements that
 are randomly chosen without repeats.
* 'Random.die(sideCount)(engine)': Same as 'Random.integer(1, sideCount)(engine)'
* 'Random.dice(sideCount, dieCount)(engine)': Produce an array of length 'dieCount' with as many 'die' rolls.
* 'Random.uuid4(engine)': Produce a [Universally Unique Identifier](http://en.wikipedia.org/wiki/Universally_unique_identifier)
Version 4.
* 'Random.string()(engine, length)': Produce a random string using numbers, uppercase and lowercase letters, '_', and '-' of length
 'length'.
* 'Random.string(pool)(engine, length)': Produce a random string using the provided string 'pool' as the possible characters to
choose from of length 'length'.
* 'Random.hex()(engine, length)' or 'Random.hex(false)(engine, length)': Produce a random string comprised of numbers or the characters
 'abcdef' of length 'length'.
...
```

#### <a name="apidoc.element.random-js.string"></a>[function <span class="apidocSignatureSpan">random-js.</span>string (pool)](#apidoc.element.random-js.string)
- description and source-code
```javascript
string = function (pool) {
  if (pool == null) {
    pool = DEFAULT_STRING_POOL;
  }

  var length = pool.length;
  if (!length) {
    throw new Error("Expected pool not to be an empty string");
  }

  var distribution = Random.integer(0, length - 1);
  return function (engine, length) {
    var result = "";
    for (var i = 0; i < length; ++i) {
      var j = distribution(engine);
      result += pool.charAt(j);
    }
    return result;
  };
}
```
- example usage
```shell
...
 * 'Random.pick(engine, array[, begin[, end]])': Return a random value within the provided 'array' within the sliced bounds of '
begin' and 'end'.
 * 'Random.picker(array[, begin[, end]])(engine)': Same as 'Random.pick(engine, array, begin, end)'.
 * 'Random.shuffle(engine, array)': Shuffle the provided 'array' (in-place). Similar to '.sort()'.
 * 'Random.sample(engine, population, sampleSize)': From the 'population' array, produce an array with 'sampleSize' elements that
 are randomly chosen without repeats.
 * 'Random.die(sideCount)(engine)': Same as 'Random.integer(1, sideCount)(engine)'
 * 'Random.dice(sideCount, dieCount)(engine)': Produce an array of length 'dieCount' with as many 'die' rolls.
 * 'Random.uuid4(engine)': Produce a [Universally Unique Identifier](http://en.wikipedia.org/wiki/Universally_unique_identifier)
Version 4.
 * 'Random.string()(engine, length)': Produce a random string using numbers, uppercase and lowercase letters, '_', and '-' of length
 'length'.
 * 'Random.string(pool)(engine, length)': Produce a random string using the provided string 'pool' as the possible characters to
 choose from of length 'length'.
 * 'Random.hex()(engine, length)' or 'Random.hex(false)(engine, length)': Produce a random string comprised of numbers or the characters
 'abcdef' of length 'length'.
 * 'Random.hex(true)(engine, length)': Produce a random string comprised of numbers or the characters 'ABCDEF' of length 'length
'.
 * 'Random.date(start, end)(engine)': Produce a random 'Date' within the inclusive range of ['start', 'end']. 'start' and 'end'
must both be 'Date's.

An example of using 'integer' would be as such:
...
```

#### <a name="apidoc.element.random-js.uint32"></a>[function <span class="apidocSignatureSpan">random-js.</span>uint32 (engine)](#apidoc.element.random-js.uint32)
- description and source-code
```javascript
uint32 = function (engine) {
  return engine() >>> 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.random-js.uint53"></a>[function <span class="apidocSignatureSpan">random-js.</span>uint53 (engine)](#apidoc.element.random-js.uint53)
- description and source-code
```javascript
uint53 = function (engine) {
  var high = engine() & 0x1fffff;
  var low = engine() >>> 0;
  return (high * 0x100000000) + low;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.random-js.uint53Full"></a>[function <span class="apidocSignatureSpan">random-js.</span>uint53Full (engine)](#apidoc.element.random-js.uint53Full)
- description and source-code
```javascript
uint53Full = function (engine) {
  while (true) {
    var high = engine() | 0;
    if (high & 0x200000) {
      if ((high & 0x3fffff) === 0x200000 && (engine() | 0) === 0) {
        return 0x20000000000000;
      }
    } else {
      var low = engine() >>> 0;
      return ((high & 0x1fffff) * 0x100000000) + low;
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.random-js.uuid4"></a>[function <span class="apidocSignatureSpan">random-js.</span>uuid4 (engine)](#apidoc.element.random-js.uuid4)
- description and source-code
```javascript
uuid4 = function (engine) {
  var a = engine() >>> 0;
  var b = engine() | 0;
  var c = engine() | 0;
  var d = engine() >>> 0;

  return (
    zeroPad(a.toString(16), 8) +
    "-" +
    zeroPad((b & 0xffff).toString(16), 4) +
    "-" +
    zeroPad((((b >> 4) & 0x0fff) | 0x4000).toString(16), 4) +
    "-" +
    zeroPad(((c & 0x3fff) | 0x8000).toString(16), 4) +
    "-" +
    zeroPad(((c >> 4) & 0xffff).toString(16), 4) +
    zeroPad(d.toString(16), 8));
}
```
- example usage
```shell
...
 * 'Random.bool(numerator, denominator)(engine)': Produce a boolean with 'numerator'/'denominator' chance of it being true.
 * 'Random.pick(engine, array[, begin[, end]])': Return a random value within the provided 'array' within the sliced bounds of '
begin' and 'end'.
 * 'Random.picker(array[, begin[, end]])(engine)': Same as 'Random.pick(engine, array, begin, end)'.
 * 'Random.shuffle(engine, array)': Shuffle the provided 'array' (in-place). Similar to '.sort()'.
 * 'Random.sample(engine, population, sampleSize)': From the 'population' array, produce an array with 'sampleSize' elements that
 are randomly chosen without repeats.
 * 'Random.die(sideCount)(engine)': Same as 'Random.integer(1, sideCount)(engine)'
 * 'Random.dice(sideCount, dieCount)(engine)': Produce an array of length 'dieCount' with as many 'die' rolls.
 * 'Random.uuid4(engine)': Produce a [Universally Unique Identifier](http://en.wikipedia.org/wiki/Universally_unique_identifier)
Version 4.
 * 'Random.string()(engine, length)': Produce a random string using numbers, uppercase and lowercase letters, '_', and '-' of length
 'length'.
 * 'Random.string(pool)(engine, length)': Produce a random string using the provided string 'pool' as the possible characters to
 choose from of length 'length'.
 * 'Random.hex()(engine, length)' or 'Random.hex(false)(engine, length)': Produce a random string comprised of numbers or the characters
 'abcdef' of length 'length'.
 * 'Random.hex(true)(engine, length)': Produce a random string comprised of numbers or the characters 'ABCDEF' of length 'length
'.
 * 'Random.date(start, end)(engine)': Produce a random 'Date' within the inclusive range of ['start', 'end']. 'start' and 'end'
must both be 'Date's.

An example of using 'integer' would be as such:
...
```



# <a name="apidoc.module.random-js.engines"></a>[module random-js.engines](#apidoc.module.random-js.engines)

#### <a name="apidoc.element.random-js.engines.mt19937"></a>[function <span class="apidocSignatureSpan">random-js.engines.</span>mt19937 ()](#apidoc.element.random-js.engines.mt19937)
- description and source-code
```javascript
function mt19937() {
  var data = new Int32Array(624);
  var index = 0;
  var uses = 0;

  function next() {
    if ((index | 0) >= 624) {
      refreshData(data);
      index = 0;
    }

    var value = data[index];
    index = (index + 1) | 0;
    uses += 1;
    return temper(value) | 0;
  }
  next.getUseCount = function() {
    return uses;
  };
  next.discard = function (count) {
    uses += count;
    if ((index | 0) >= 624) {
      refreshData(data);
      index = 0;
    }
    while ((count - index) > 624) {
      count -= 624 - index;
      refreshData(data);
      index = 0;
    }
    index = (index + count) | 0;
    return next;
  };
  next.seed = function (initial) {
    var previous = 0;
    data[0] = previous = initial | 0;

    for (var i = 1; i < 624; i = (i + 1) | 0) {
      data[i] = previous = (imul((previous ^ (previous >>> 30)), 0x6c078965) + i) | 0;
    }
    index = 624;
    uses = 0;
    return next;
  };
  next.seedWithArray = function (source) {
    next.seed(0x012bd6aa);
    seedWithArray(data, source);
    return next;
  };
  next.autoSeed = function () {
    return next.seedWithArray(Random.generateEntropyArray());
  };
  return next;
}
```
- example usage
```shell
...

## API

### Engines

* 'Random.engines.nativeMath': Utilizes 'Math.random()'
* 'Random.engines.browserCrypto': Utilizes 'crypto.getRandomValues()'
* 'Random.engines.mt19937()': Produces a new Mersenne Twister. Must be seeded before use.

### Mersenne Twister API

Assuming one has done 'var mt = Random.engines.mt19937()':

* 'mt()': Produce a 32-bit signed integer.
* 'mt.seed(value)': Seed the twister with an initial 32-bit integer.
...
```

#### <a name="apidoc.element.random-js.engines.nativeMath"></a>[function <span class="apidocSignatureSpan">random-js.engines.</span>nativeMath ()](#apidoc.element.random-js.engines.nativeMath)
- description and source-code
```javascript
nativeMath = function () {
  return (Math.random() * 0x100000000) | 0;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
