## Use

```js
// Read the markdown file written using the Gitdown syntactic sugar.
var gitdown = Gitdown.fromFile('./README.gitdown.md');

// Output the markdown file.
gitdown.save('./README.md');
```

### File Size

Calculates the size of a file. Returns size formatted to a human friendly format.

| Method | Description |
| --- | --- |
| `gitdown.filesize` | Size of a file. |
| `gitdown.filesize.gzip` | Size of a gzipped file. |

```Handlebars
{{gitdown.filesize}}./dist/foo.js{{gitdown.filesize}}
{{gitdown.filesize.gzip}}./dist/foo.js{{gitdown.filesize.gzip}}
```