placebear
===========

Simple CLI node utility that downloads files from [placebear.com](http://placebear.com).

Installation
------------

Installing is quite simple

```
npm install -g placebear
```

If you want to reuse the file fetching logic, you can also install placebear as a dependency of your own module

```
npm install --save placebear
```

Usage
-----

Placebear is pretty easy to use.

```
placebear [-d path/to/download/folder] width[/height] [...]
```

Here are some concrete usage examples

```bash
placebear 200/100 # Download a 200x100 image
placebear 100/300 200 # Download a 100x300 image and a 200x200 image
placebear -d bears 800/600 # Download a 800x600 image into the bears folder
```

In order for the -d (a.k.a. --directory) flag to work, the folder must already exist.
Otherwise placebear will just return an error.
