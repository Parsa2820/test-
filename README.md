```bash
CPU_ARCH=$(lscpu| grep Architecture| tr -s ' '| cut -d ' ' -f 2) && gcc -D CPU_ARCH="\"$CPU_ARCH\"" main.c -o "$CPU_ARCH.out"
```
