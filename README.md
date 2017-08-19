# pascal-quine-twins
Program that prints source of another program, that prints source of the first program

Compile with Free Pascal.

```
$ fpc twin1.pas
$ ./twin1 > twin2.pas
$ fpc twin2.pas
$ ./twin2 > twin1~.pas
$ diff -s twin1.pas twin1~.pas
Files twin1.pas and twin1~.pas are identical
```
