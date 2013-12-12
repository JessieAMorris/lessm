lessm
=====

`lessm` is very similar unto lessc except for the fact that it accepts multiple input files.

`lessm` essentially takes the input files passed to it and creates a file with `@import` statements for each file. It creates these `@import`'s in the order that the files were passed to it. Since order does indeed matter in LESS land, this is important and order is guaranteed.

Right now usage is as follows:

```
lessm foo.less bar.less bing.less -o out.css
```

The -o argument is optional. If specified, it will write the output to that file, otherwise it will output to stdout.
