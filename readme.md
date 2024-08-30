# Media types

Relation of supported Media Types.

All the types are coming from
[IANA/media-types](https://www.iana.org/assignments/media-types/media-types.xhtml)

Last revision of the package (related to the document revision date above):
2024-08-19

## Table of Contents

- [Installation](#installation)
- [Exports](#exports)
  - [MediaTypesMap](#mediatypesmap)
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

### MediaTypesMap

#### Definition:

```
MediaTypesMap :: Object {
  <media type name> => <media type list>
}
```

#### Example:

```javascript
MediaTypesMap['mp4'] // => [ 'application/mp4', 'audio/mp4', 'video/mp4' ]
MediaTypesMap['plain'] // => [ 'text/plain' ]
```

### MediaTypes

#### Definition:

```
MediaTypes :: Relation {
  <media type name> <=> <media type value>
}
```

#### Example:

```javascript
MediaTypes.has('javascript') // => true
MediaTypes.has('text/javascript') // => true

MediaTypes.get('mp4') // => [ 'application/mp4', 'audio/mp4', 'video/mp4' ]
MediaTypes.get('audio/mp4') // => 'mp4'

MediaTypes
  .addNode('my', 'a/my', 'b/my')
  .get('b/my') // => 'my'

MediaTypes
  .get('my') // => [ 'a/my', 'b/my' ]

MediaTypes
  .get(MediaTypes.get('my')) // => 'my'

MediaTypes
  .addEdge('mp4', 'example/mp4')
  .get('example/mp4') // => 'mp4'

MediaTypes
  .get('mp4') // => [ 'application/mp4', 'audio/mp4', 'video/mp4', 'example/mp4' ]
```

## More

This package utilises [Relation](https://github.com/yurkimus/relation) to
provide a better developer experience and extendability

## License

[MIT](LICENSE)
