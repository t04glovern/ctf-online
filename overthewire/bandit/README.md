## Levels

#### Level 0
`ssh bandit0@bandit.labs.overthewire.org -p 2220`

**User:** bandit0

**Pass:** bandit0

```
$ cat readme
boJ9jbbUNNfktd78OOpsqOltutMc3MY1
```

#### Level 1
`ssh bandit1@bandit.labs.overthewire.org -p 2220`

**User:** bandit1

**Pass:** boJ9jbbUNNfktd78OOpsqOltutMc3MY1

```
$ cat ./-
CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9
```

#### Level 2
`ssh bandit2@bandit.labs.overthewire.org -p 2220`

**User:** bandit2

**Pass:** CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9

```
$ cat spaces\ in\ this\ filename
UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK
```

#### Level 3
`ssh bandit3@bandit.labs.overthewire.org -p 2220`

**User:** bandit3

**Pass:** UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK

```
$ cd inhere/
$ cat .hidden
pIwrPrtPN36QITSp3EQaw936yaFoFgAB
```

#### Level 4
`ssh bandit4@bandit.labs.overthewire.org -p 2220`

**User:** bandit4

**Pass:** pIwrPrtPN36QITSp3EQaw936yaFoFgAB

```
$ cd inhere/
$ file ./*

./-file00: data
./-file01: data
./-file02: data
./-file03: data
./-file04: data
./-file05: data
./-file06: data
./-file07: ASCII text
./-file08: data
./-file09: data

$ cat ./-file07
koReBOKuIDDepwhWk7jZC0RTdopnAYKh
```

#### Level 5
`ssh bandit5@bandit.labs.overthewire.org -p 2220`

**User:** bandit5

**Pass:** koReBOKuIDDepwhWk7jZC0RTdopnAYKh

```
$ cd inhere/
$ find ./ -type f -size 1033c -exec ls {} \;
./maybehere07/.file2

$ cat ./maybehere07/.file2
DXjZPULLxYr17uwoI01bNLQbtFemEgo7
```

#### Level 6
`ssh bandit6@bandit.labs.overthewire.org -p 2220`

**User:** bandit6

**Pass:** DXjZPULLxYr17uwoI01bNLQbtFemEgo7

```
$ find / -type f -size 33c -group bandit6 -user bandit7 -exec ls {} \;
/var/lib/dpkg/info/bandit7.password

$ cat /var/lib/dpkg/info/bandit7.password
HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs
```

#### Level 7
`ssh bandit7@bandit.labs.overthewire.org -p 2220`

**User:** bandit7

**Pass:** HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs

```
$ grep millionth data.txt
millionth	cvX2JJa4CFALtqS87jk27qwqGhBM9plV
```

#### Level 8
`ssh bandit8@bandit.labs.overthewire.org -p 2220`

**User:** bandit8

**Pass:** cvX2JJa4CFALtqS87jk27qwqGhBM9plV

```
$ sort data.txt |  uniq -u
UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR
```

#### Level 9
`ssh bandit9@bandit.labs.overthewire.org -p 2220`

**User:** bandit9

**Pass:** UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR

```
$ strings data.txt | grep ====
========== theOkM
========== password
========== is
)========== truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk
```

#### Level 10
`ssh bandit10@bandit.labs.overthewire.org -p 2220`

**User:** bandit10

**Pass:** truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk

```
$ cat data.txt | base64 -d -i
The password is IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR
```
