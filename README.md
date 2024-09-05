# linux-compilation
linux commands for personal use

File compression using gzip

To compress a file:
```
$ gzip -v sample-file.txt
```

Output:
```
sample-file.gz
```

To compress a file:
```
$ gunzip -v sample-file.gz
```

Output:
```
sample-file.txt
```

To archive a file:
```
$ tar cf archive.tar sample-file1.txt sample-file2.txt sample-file3.txt 
```

*Note: Total size of files archive will be equal to the output*

To check the content of the archived file:
```
$ tar tvf archive.tar
sample-file1.txt
sample-file2.txt
sample-file3.txt 
```

To compress the content of the archived file to smaller size:
```
$ tar czf compressed-archive.tar.gz sample-*
```

Output:
```
compressed-archived.tar.gz
```

To extract the content of the archived file:
```
$ tar xvf compressed-archive.tar.gz -C sample-directory
```

Output:
*List of all files inside the archived file*

