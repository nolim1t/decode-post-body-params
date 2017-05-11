# Decode Post Body Params

[![npm version](https://badge.fury.io/js/decode-post-body-params.svg)](https://badge.fury.io/js/decode-post-body-params)

## About

I created this library because I felt the need for parsing post body params through AWS Lambda without having to write a complex parser (although that is still possible).

That way I can use a framework such as the Serverless framework to deploy without worrying about logging into the console.

Therefore speeding up development

## Installing

```bash
npm i decode-post-body-params
```

## Contributing

All contributions are welcome and appreciated. Open Source is a meritocracy who doesn't care who you are.

* Issues
* Pull Requests
* Donations (BTC: [14qd36n1viYAWzajZgaTQq4tPUZcEUtfcz](http://blockr.io/address/info/14qd36n1viYAWzajZgaTQq4tPUZcEUtfcz) / LTC: [LSGfxUoJSC3qYsTC6DwyvKvYfDwTVXrcE2](http://ltc.blockr.io/address/info/LSGfxUoJSC3qYsTC6DwyvKvYfDwTVXrcE2) / [Dollars](https://donate.nolim1t.co))

## Usage:

### Example: Grab a post param called 'address'

event.body being the post body received from AWS Lambda.

```javascript
var decodebodyparams = require('decode-post-body-params');
var data_address = decodebodyparams('address', "http://localhost/?" + event.body);
```
