# Week6_lecture_note

## Changesvs.Snapshots

![image](https://github.com/Mabbru/neuralintlab/assets/105326662/a3a5075e-9a31-4717-aa85-333442224c97)


### pwd : 
shows the current path in hierarchical direcotory → 현재 위치를 보여주줌
### cd :
change direcotory → 현재 위치를 변경함
### ls :
list files and direcotories → 현재 위치의 files 과 direcotoreies 을 list 형식으로 나열하여 보여줌
### clear :
clear past commands → 화면정리

### 추가적인 부분 
```sh
$ arguments:  [directoryname]  /root  
$ .currentdirectory  
$ ..upper-leveldirectory  
$ ~homeofcurrentuser 
$ /[directoryname]:absolutepath
$ ./[directoryname]:relativepath  
$ ../[directoryname]:relativepath
```

### Option :
```sh
$ l : show detailed information (longformat) 
$ lh : same as above, but size in units
$ ls : list the files in the working directory
$ ls /bin : list the files in the .bin directory (or any other directory)
$ ls -1 : list the files in the working directory in long format
$ ls -1 /etc /bin : list the files in the /bin directory and the /etc directory in long format
$ ls -la : list all files (even ones with names beginning with a preiod character, which are normally hidden) in the parent of the working directory in long format
```

## Manipulation (These commands may delete or overwrite your files and directories!)

### cp :
copy files and directories → 복사하기
```sh
$ cp file1 file2
$ cp -i file1 file2
$ cp file1 dir2
$ cp -R dir1 dir2
```
### mv :
move files and directories or rename them → 옮기기 및 이름 바꾸기
```sh
$ mv file1 file2
$ mv -i file1 file2
$ mv file1 file2 dir1
$ mv dir1 dir2
```
### rm :
delete files and directories permantely and irreversevely  → 삭제하기
```sh
$ rm file1 file2
$ rm -i file1 file2
$ rm -r dir1 dir2
```
### mkdir :
make a new directory → 새로 만들기

## Wildcards
```sh
$ *
$ g*
$ b*.txt
$ Data???
$ cp *.txt text_files
$ mv dir1 ../*.bak dir2
$ rm *~
```

### Tip :
- Autocompletion(자동완성) : "tab" key
- Past Commands(다시쓰기) : "up arrow"
- Help Command : "help" , "man"
- Exiting terminal : "exit"
