FireSim-Emscripten
===========

FireSim compiled to JavaScript. 

##Requirements:
  * [Emscripten](https://github.com/kripken/emscripten/wiki/Tutorial)
  * [program-editor](https://github.com/crowdprocess/program-editor)

##Recommended reading:
 * [Mustache manual](http://mustache.github.io/mustache.5.html)

#####See: [template](https://github.com/sergio2540/FireSim-Emscripten/blob/master/crowdprocess/pre/template/template.mustache)


##Usage:

####Compile c code: 
  `make c CC=gcc`
 
####Run c code: 
   
  `make run-c`
   or 
  `make run-c ARGV='100 5 1 135 malcataSlope_100.grass malcataAspect_100.grass '`

####Compile js code: 
  `make cp EMCC=path/to/emscripten/emcc`

####Run js with [program-editor](https://github.com/crowdprocess/program-editor): 
   `make run-editor`

#####See: [Makefile](https://github.com/sergio2540/FireSim-Emscripten/blob/master/Makefile)
