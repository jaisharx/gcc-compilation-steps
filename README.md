# Understanding how GCC carries out compilation

### Steps involved in GCC compilation:
<br>

1 **Preprocessing**
```sh
gcc -E -o step-1-preporcessing.c main.c
```

2 **Compilation**
```sh
gcc -S -o step-2-compilation.s step-1-preprocessing.c
```
    
3 **Assembly**
```sh
gcc -c -o step-3-assembly.o step-2-compilation.s
```

4 **Linking**
```sh
gcc -o step-4-linking step-3-assembly.o
```

5 **Running**
```sh
.\step-4-linking.exe
```

### ***This repo is inspired by an YT video. Check it out [here](https://www.youtube.com/watch?v=lrx5dcB_4Oo). Thanks!***