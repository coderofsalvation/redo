redo (makefile alternative) in ~18 lines of shellscript #permacomputing #minimalist 

## Usage

```bash
$ ./redo 
.redo/default.do.o a.o
.redo/default.do.o b.o
.redo/default.do
rebuild of myapp

$ ./redo                    
$                           # nothing to do! \o/

$ touch a.o                 # simulate modification
$ ./redo
.redo/default.do.o a.o
.redo/default.do
rebuild of myapp
```

for original see: https://redo.readthedocs.io/en/latest/

## Notes 

* few changes to the paradigm have been made (to keep the code small)
* no fancy circular dependency checking..linear pipelines only for now
