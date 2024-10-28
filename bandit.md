
# OverTheWire Bandit Guide

## Bandit0 -> 1
```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
ls
cat readme
```

## Bandit1 -> 2
```bash
ls
cat ./.
```

## Bandit2 -> 3
```bash
ls
cat "entre comillas si hay espacios separados"
```

## Bandit3 -> 4
```bash
ls -a    # Para ver archivos ocultos
```

## Bandit4 -> 5
```bash
ls -a
file ./*   # Para ver el tipo de datos que contiene cada archivo
```

## Bandit5 -> 6
```bash
du -b -a | grep 1033
cat ./maybehere07/.file2
```

## Bandit6 -> 7
```bash
find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
cat /var/lib/dpkg/info/bandit7.password
```

## Bandit7 -> 8
```bash
ls
cat data.txt
grep millionth data.txt
```

## Bandit8 -> 9
```bash
ls
sort data.txt | uniq -u
```

## Bandit9 -> 10
```bash
ls
strings data.txt
strings data.txt | grep '=*[^=]'
```

## Bandit10 -> 11
```bash
ls
cat data.txt
base64 -d data.txt
```

## Bandit11 -> 12
```bash
ls
cat data.txt
cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'
```

## Bandit12 -> 13
```bash
ls
head data.txt
cp data.txt /home
mv data.txt data
xxd -r data > binary
mv binary binary.gz
gunzip binary.gz
tar -xf binary
tar -xf data5.bin
bunzip2 data6.bin
tar -xf data6.bin.out
mv data8.bin data8.gz
gunzip data8.gz
cat data8
```

## Bandit13 -> 14
```bash
ls -la
ssh -i sshkey.private -p 2220 bandit14@localhost
```

## Bandit14 -> 15
```bash
cat /etc/bandit_pass/bandit14
telnet localhost 30000
```

## Bandit15 -> 16
```bash
cat /etc/bandit_pass/bandit15
openssl s_client -connect localhost:30001
```
