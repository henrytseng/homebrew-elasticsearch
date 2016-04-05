# Homebrew ElasticSearch

A repository for ElasticSearch-related brews.


## Requirements

* [Homebrew](https://github.com/Homebrew/homebrew)
* OSX El Capitan.  Untested everywhere else.
* The Homebrew `versions` tap - `brew tap homebrew/versions`


## Installation

Setup the `homebrew/versions` tap which has dependencies we need:

```sh
$ brew tap homebrew/versions
```

Then, run the following in your command-line:

```sh
$ brew tap henrytseng/homebrew-elasticsearch
```

## Usage

To install ElasticSearch 1.5.2

```sh
$ brew install elasticsearch15
```

To start the service

```sh
brew services start elasticsearch15
```

To stop the service

```sh
brew services stop elasticsearch15
```


And to check if the service is working

```sh
brew services list
```

Check for a reponse from

```sh
curl http://localhost:9200
```


## Troubleshooting

If you've installed another version of ElasticSearch make sure to unlink a previous version, depending on what version:

```sh
brew unlink elasticsearch
```


## Contributing

See [Contributing](CONTRIBUTING.md)


## License

Copyright (c) 2016 Henry Tseng and other contributors

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
