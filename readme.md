# gravatar-url [![Build Status](https://travis-ci.org/sindresorhus/gravatar-url.svg?branch=master)](https://travis-ci.org/sindresorhus/gravatar-url)

> Get the URL to a Gravatar image from an email


## Install

```
$ npm install --save gravatar-url
```


## Usage

```js
var gravatarUrl = require('gravatar-url');

gravatarUrl('sindresorhus@gmail.com', {size: 200});
//=> 'https://gravatar.com/avatar/d36a92237c75c5337c17b60d90686bf9?size=200'
```


## API

### gravatarUrl(email, [options])

#### email

*Required*  
Type: `string`

Email matching a Gravatar profile.

#### options

##### size

Type: `number`  
Default: `80`  
Values: `1..2048`

[Size](https://en.gravatar.com/site/implement/images/#size) of the image.

##### default

Type: `string`  
Default: [This image](http://www.gravatar.com/avatar/00000000000000000000000000000000)  
Values: Custom URL or `404`, `mm`, `identicon`, `monsterid`, `wavatar`, `retro`, `blank`

[Image](https://en.gravatar.com/site/implement/images/#default-image) to return if the email didn't match any Gravatar profile.

##### rating

Type: `string`  
Default: `g`  
Values: `g`, `pg`, `r`, `x`

Allowed [rating](https://en.gravatar.com/site/implement/images/#rating) of the image.


## Related

- [get-gravatar](https://github.com/sindresorhus/get-gravatar) - Get a Gravatar image


## License

MIT © [Sindre Sorhus](http://sindresorhus.com)
