# Lab for practice with vi editor


Step 1. Create a new file

In a Linux/Macos there are several ways how to create a new file

- touch newfile.txt
- vi newfile.txt

First command just creates ea new file

Second command creates a new file and opens editor vi


Step 2. Populate new file with following context

```
Hi, I'm working on Macos in VI editor
```

???+ note

     for start typing you need to activate INSERT mode, ESC+i


Step 3. Save such file and close at the same time

???+ note

     use following combination ESC + :wq ENTER

Step 4. Read your file

```
cat newfile.txt
```

???+ note

     **cat** is Linux/Macos command to read files

Step 5. Open you file and modify content

```
vi newfile.txt
```

Change content to:

```
Hi, I'm working second time on Macos in VI editor.
```

Step 6. Delete such file

```
rm newfile.txt
```

???+ note

     **rm** is Linux/Macos command for delete files or directories.
      In some cases it asks to confirm deletion operation in terminal
