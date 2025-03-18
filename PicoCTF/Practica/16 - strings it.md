#### Descripción
Can you find the flag in file without running it?

PISTA: Enlace a Strings en linux.


#### Solución 
Usando el comando Strings que lo que hace es imprimir una secuencia de 4 o mas caracteres, haciendo que se pueda hacer varias filas de palabras en un archivo. Con eso podemos hacer una busqueda usando Grep para encontrar la flag.
```
s3770
s8681
s8644
s8294
s4981
s4944
s4594
s4096
s8012
s4312
s3374
s6922
s6552
s6517
s2852
s2817
s574
s539
s189
s3278
s3239
s929
s7644
s7274
s3774
s8740
s8370
s4670
s4150
s4115
s9996
s9546
s1396
s7862
s7827
s7492
s7457
s3992
s3957
s611
s241
s7789
s7312
s3812
s778
s3752
s3717
s7622
s7252
s7217
s5590
s5940
s9298
s3412
s6332
s2632
s3250
s3215
s2296
s4178
s4139
s4674
s8744
s8374
.symtab
.strtab
.shstrtab
.interp
.note.ABI-tag
.note.gnu.build-id
.gnu.hash
.dynsym
.dynstr
.gnu.version
.gnu.version_r
.rela.dyn
.rela.plt
.init
.plt.got
.text
.fini
.rodata
.eh_frame_hdr
.eh_frame
.init_array
.fini_array
.dynamic
.data
.bss
.comment
RepugnamShip33-picoctf@webshell:~$ strings --help
Usage: strings [option(s)] [file(s)]
 Display printable strings in [file(s)] (stdin by default)
 The options are:
  -a - --all                Scan the entire file, not just the data section [default]
  -d --data                 Only scan the data sections in the file
  -f --print-file-name      Print the name of the file before each string
  -n <number>               Locate & print any sequence of at least <number>
    --bytes=<number>         displayable characters.  (The default is 4).
  -t --radix={o,d,x}        Print the location of the string in base 8, 10 or 16
  -w --include-all-whitespace Include all whitespace as valid string characters
  -o                        An alias for --radix=o
  -T --target=<BFDNAME>     Specify the binary file format
  -e --encoding={s,S,b,l,B,L} Select character size and endianness:
                            s = 7-bit, S = 8-bit, {b,l} = 16-bit, {B,L} = 32-bit
  --unicode={default|show|invalid|hex|escape|highlight}
  -U {d|s|i|x|e|h}          Specify how to treat UTF-8 encoded unicode characters
  -s --output-separator=<string> String used to separate strings in output.
  @<file>                   Read options from <file>
  -h --help                 Display this information
  -v -V --version           Print the program's version number
strings: supported targets: elf64-x86-64 elf32-i386 elf32-iamcu elf32-x86-64 pei-i386 pe-x86-64 pei-x86-64 elf64-l1om elf64-k1om elf64-little elf64-big elf32-little elf32-big pe-bigobj-x86-64 pe-i386 srec symbolsrec verilog tekhex binary ihex plugin
Report bugs to <https://sourceware.org/bugzilla/>
RepugnamShip33-picoctf@webshell:~$ strings strings | grep "picoCTF"
picoCTF{5tRIng5_1T_d66c7bb7}
```
#### Notas Adicionales


#### Referencias
https://linux.die.net/man/1/strings