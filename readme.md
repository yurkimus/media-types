# Media Types Listing

Listing of supported Media Types.

All the types are coming from
[IANA/media-types](https://www.iana.org/assignments/media-types/media-types.xhtml)

Last revision of the package (related to the document revision date above):
2024-08-19

## Table of Contents

- [Installation](#installation)
- [Exports](#exports)
  - [MediaTypes](#mediatypes)
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
MediaTypes :: Object { <name> => <media type>[] }
```

#### Example:

```javascript
MediaTypes['mp4'] // => [ 'application/mp4', 'audio/mp4', 'video/mp4' ]
MediaTypes['plain'] // => [ 'text/plain' ]
```

## License

[MIT](LICENSE)
