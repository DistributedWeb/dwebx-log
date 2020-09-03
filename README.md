# dwebx-log

view history of a dwebx in the CLI

[![npm][npm-image]][npm-url]
[![travis][travis-image]][travis-url]
[![standard][standard-image]][standard-url]

`dwebx-log` prints all changes, the file versions, and information about the dwebx:

```
❯ dwebx-log dwebx://64375abb733a62fa301b1f124427e825d292a6d3ba25a26c9d4303a7987bec65
1 [put] / 0 B (0 blocks)
2 [put] /README 175 B (1 block)
3 [put] /dwebx.json 309 B (1 block)
4 [put] /far-manzanar.csv 2.0 MB (31 blocks)
5 [put] /far-minidoka.csv 2.1 MB (33 blocks)
6 [put] /far-poston.csv 3.6 MB (55 blocks)
7 [put] /wra-master.csv 73 MB (1111 blocks)

Log synced with network

Archive has 7 changes (puts: +7, dels: -0)
Current Size: 80 MB
Total Size:
- Metadata 436 B
- Content 80 MB
Blocks:
- Metadata 8
- Content 1232
```

## Install

If you already have `dwebx` installed, run it with `dwebx log`!

```
npm install -g dwebx-log
```

## Usage

You can view history for a local dwebx (any directory with a `.dwebx` folder):

```sh
dwebx-log /my-data
```

Or view history for a remote dwebx using the dwebx link:

```sh
dwebx-log dwebx://64375abb733a62fa301b1f124427e825d292a6d3ba25a26c9d4303a7987bec65 
```

Options: 

* `--live, -l`: Keep process running and view live history

## License

[MIT](LICENSE.md)

[npm-image]: https://img.shields.io/npm/v/dwebx-log.svg?style=flat-square
[npm-url]: https://www.npmjs.com/package/dwebx-log
[travis-image]: https://img.shields.io/travis/joehand/dwebx-log.svg?style=flat-square
[travis-url]: https://travis-ci.org/joehand/dwebx-log
[standard-image]: https://img.shields.io/badge/code%20style-standard-brightgreen.svg?style=flat-square
[standard-url]: http://npm.im/standard
