# Flag
`hsctf{wow_much_png}`

# Guide

```bash
binwalk doge.png                                    # This tells us there are 2 png in this png file... weird
dd if=./doge.png of=./flag.png bs=1 skip=206707     # Extracting...
xdg-open flag.png                                   # Reading...
```
