FireSim-Emscripten
===========

FireSim compiled to JavaScript. 

##Requirements:
  * [Emscripten](https://github.com/kripken/emscripten/wiki/Tutorial)
  * [program-editor](https://github.com/crowdprocess/program-editor)
  * [crowdprocess-cli](https://github.com/CrowdProcess/crp-cli)

##Recommended reading:
 * [Mustache manual](http://mustache.github.io/mustache.5.html)
 * [Emscripten/wiki/Filesystem Guide](https://github.com/kripken/emscripten/wiki/Filesystem-Guide)
  
#####See: [template.mustache](https://github.com/sergio2540/FireSim-Emscripten/blob/master/crowdprocess/pre/template/template.mustache)

 * [HOWTO: Port a C/C++ Library to JavaScript (xml.js)@blog.mozakai](http://mozakai.blogspot.pt/2012/03/howto-port-cc-library-to-javascript.html)
 * [FireSim@blog.crowdprocess](http://blog.crowdprocess.com/post/57794500198/crowdprocess-is-on-fire-wildfire-actually)


##Usage:

###Install: 

```bash
  cd ./FireSim-Emscripten
  make install
```

###Compile c code: 

```bash
  make c CC=cc
```
###Run c code: 

```bash
  make run-c
  make run-c ARGV='100 5 1 135 malcataSlope_100.grass malcataAspect_100.grass'
```
###Compile js code: 

```bash 
  make cp EMCC=path/to/emscripten/emcc
```
###Generate data.json:

######See: [Explain crowdprocess/pre/data](https://gist.github.com/sergio2540/b5b45f9e13e533ea056d)

###Generate program.js:

######See: [Explain crowdprocess/view/data](https://gist.github.com/sergio2540/fac873fccde43bb98b44)
       
###Run js with [program-editor](https://github.com/crowdprocess/program-editor): 

```bash
   make run-editor
```
###Run js with [crowdprocess-cli](https://github.com/CrowdProcess/crp-cli):
```bash
   make run-io
```

#####See: [Makefile](https://github.com/sergio2540/FireSim-Emscripten/blob/master/Makefile)
