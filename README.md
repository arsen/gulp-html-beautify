# Information
This is a gulp plugin for js-beautify.

# Usage
```javascript
var htmlbeautify = require('gulp-html-beautify');

gulp.task('htmlbeautify', function() {
  var options = {
    {indentSize: 2}
  };
  gulp.src('./src/*.js')
    .pipe(htmlbeautify(options))
    .pipe(gulp.dest('./public/'))
});
```

# Options
Plugin options:
- `use_rc`
  - Default is `true`
  - When `false` do not lookup `.jsbeautifyrc` files, which are JSON encoded configuration files for [js-beautify](https://github.com/beautify-web/js-beautify#options).

You can pass in any other options and it passes them directly to [js-beautify](https://github.com/beautify-web/js-beautify).
```json
{
    "indent_size": 4,
    "indent_char": " ",
    "eol": "\n",
    "indent_level": 0,
    "indent_with_tabs": false,
    "preserve_newlines": true,
    "max_preserve_newlines": 10,
    "jslint_happy": false,
    "space_after_anon_function": false,
    "brace_style": "collapse",
    "keep_array_indentation": false,
    "keep_function_indentation": false,
    "space_before_conditional": true,
    "break_chained_methods": false,
    "eval_code": false,
    "unescape_strings": false,
    "wrap_line_length": 0,
    "wrap_attributes": "auto",
    "wrap_attributes_indent_size": 4,
    "end_with_newline": false
}
```
# LICENSE
(MIT License)

Copyright (c) 2015 Arsen Ghazaryan [arsen.ghazaryan@gmail.com](mailto:arsen.ghazaryan@gmail.com)

Permission is hereby granted, free of charge, to any person obtaining<br>a copy of this software and associated documentation files (the<br>"Software"), to deal in the Software without restriction, including<br>without limitation the rights to use, copy, modify, merge, publish,<br>distribute, sublicense, and/or sell copies of the Software, and to<br>permit persons to whom the Software is furnished to do so, subject to<br>the following conditions:

The above copyright notice and this permission notice shall be<br>included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,<br>EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF<br>MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND<br>NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE<br>LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION<br>OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION<br>WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
