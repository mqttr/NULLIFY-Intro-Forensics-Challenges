# Flag
hsctf{wrong_file_ext}

# Guide

```bash
mv flag.exe flag.gz
gunzip flag.gz
7z x flag
cat flag.txt | iconv -f UTF32
```
