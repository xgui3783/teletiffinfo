# remote-metadata

Read metadata of remote TIFF according to [TIFF6 spec](https://www.adobe.io/open/standards/TIFF.html) (currently only reads width and height.)

## Requirements

server must support [RANGE request](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Range).

## Why?

For large TIFF files, it is often not feasible to download the full TIFF file in order to access the metadata. 

## Usage

```python
from teletiffinfo import try_tiff
try_tiff('https://file-examples-com.github.io/uploads/2017/10/file_example_TIFF_10MB.tiff') # returns (1950, 1301)
```

## License

MIT
