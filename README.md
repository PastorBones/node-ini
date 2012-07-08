# node-ini

A simple .ini config parser that supports sections, comments, arrays, and objects.

To parse a .ini file asynchronously:
<pre>
var ini = require('node-ini');
ini.parse('./config.ini', function(err,data){
  if(err) {
    console.log(err);
  } else {
    console.log(data);
  }
});
</pre>

To parse a .ini file synchronously:
<pre>
var ini = require('node-ini');
var cfg = ini.parseSync('./config.ini');
</pre>

The file encoding defaults to `utf-8`, but can be changed.
<pre>
var ini = require('node-ini');
ini.encoding = 'utf-16';
var cfg = ini.parseSync('./config.ini');
</pre>

## Installation
npm:

`npm install node-ini`

## License

(The MIT License)

Copyright (c) 2009-2010 Jordy van Gelder &lt;jordyvangelder@gmail.com&gt;

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
