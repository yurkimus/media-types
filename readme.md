# Media types

Enumeration of supported HTTP statuses.

All the types are coming from
[IANA/media-types](https://www.iana.org/assignments/media-types/media-types.xhtml)

Last revision of the package (related to the document revision date above):
2024-08-19

## Table of Contents

- [Installation](#installation)
- [Exports](#exports)
  - [MediaTypes](#mediatypes)
- [More](#more)
- [License](#license)

## Installation

### npm

```
npm install @yurkimus/media-types
```

### urls

```
"@yurkimus/media-types": "npm:@yurkimus/media-types"
```

```
"@yurkimus/media-types": "github:yurkimus/media-types"
```

```
"@yurkimus/media-types": "https://raw.githubusercontent.com/yurkimus/media-types/main/source/index.js"
```

## Exports

### MediaTypes

#### Definition:

```
MediaTypes :: Enumeration { <media type name> <=> <media type value> }
```

#### Example:

```javascript
MediaTypes.get('json') // => 'application/json'
MediaTypes.get('application/json') // => 'json'

MediaTypes.get('application/node') // => 'node'
MediaTypes.get('node') // => 'application/node'

MediaTypes.has('pdf') // => true
MediaTypes.has('application/wasm') // => true
```

## More

This package utilises [Enumeration](https://github.com/yurkimus/enumeration) to
provide a better developer experience and extendability for the media types
listed in presented enumeration

## License

[MIT](LICENSE)
