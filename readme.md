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
MediaTypes.get('node') // => 'application/node'
```

## More

This package utilises
[Enumeration package](https://github.com/yurkimus/enumeration) to provide a
better developer experience and extendability of the media types listed in the
presented enumeration

## License

[MIT](LICENSE)
