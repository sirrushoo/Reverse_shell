# Reverse_shell

## :one: Reverse Shell x86 :fr:

Warning, this reverse shell is not portable, just for show example how does a reverse shell in x86 in assembly code, this method is really old

- Ligne 78 v2 : LoadLibraryA replace it by your own offset
- Ligne 79 v2 : GetProcAddress replace it by your own offset
- Ligne 193 v2: SOKADDR_IN set you own port and IP address

### Architecture

Win32 plateform

- XP 
- Win 7
- Win 10 - Windows Defender Detects it's bad for you

### Compilation 

```
$nasm -f win32 reverse_shell.s -o reverse_shell.o
$ld -m i386 reverse_shell.o -o reverse_shell32.exe

```
### Show Hex

```
$nasm -f bin reverse_shell.s -o reverse_shell_bin.o
$cat reverse_shell_bin | hexdump -C

```

<img src="https://zupimages.net/up/18/52/3s63.png">
<img src="https://zupimages.net/up/18/52/y6mk.png">
