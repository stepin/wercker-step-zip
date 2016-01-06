Wercker step zip [![MIT License](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/tcnksm/wercker-step-zip/blob/master/LICENCE)
====

[![wercker status](https://app.wercker.com/status/9f2733b432a0fd76e2846f95da95e3d3/s/master "wercker status")](https://app.wercker.com/project/bykey/9f2733b432a0fd76e2846f95da95e3d3)

This is [wercker](http://wercker.com/) build step script to package your directories as `.zip`. 

## Usage

In the `wercker.yml` of your application use the following step definition:

```yaml
steps:
   - tcnksm/zip:
     input: $WERCKER_OUTPUT_DIR/pkg
     output: $WERCKER_OUTPUT_DIR/dist
```

You must set `input` directory where directories you want to package are in and `output` directory where zip archeives will be generated. Both must be set as absolte path (`$WERCKER_OUTPUT_PATH` is built-in environmental valiable which is used for pass the artifacts between build step and deploy step). 

## Author

[tcnksm](https://github.com/tcnksm)
