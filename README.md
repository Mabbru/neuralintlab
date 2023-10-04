# Week4_lecture_note

## Shell Command

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



# Week5_lecture_note


## I/O Redirection

### I/O Redirection(Standard Output) : 
">" : Command 뒤에 ">"을 사용하여 출력을 리디렉션하여 파일에 출력을 생성하고 저장할 수 있다.
"cat" : 텍스트 파일의 내용을 표시한다.
">>" : 출력을 기존 파일에 추가하거나, 파일이 없는 경우에는 새 파일을 만들고 추가한다.

### I/ORedirection(Standard Input) :
"<" : 파일에서 입력된 내용을 리다이렉트 할 수 있다.
Pipeline "ㅣ" : 이전 명령의 출력을 다음 명령의 입력에 공급한다.
추가적으로 특수 문자는 셸 명령이 주어질 때 그 의미를 확장한다. ex) "*", "~"

## Permission
Linux는 multi - user system으로 files 과 directories에는 owner, group, others에 따라 다르게 할당된 permission이 있다.
"chmod" : permission을 바꿈 
ex) chmod 600 some_file : 6은 110 / 0은 0 / 0은 0 = owner에게 rw permission을 줌.
    chmod 777 some_file : 111 / 111 / 111로 owner, group, others 모두에게 rwx permission을 줌 

## Superuser
Superuser는 모든 시스템 관리 권한을 가지며, 일부 명령에는 수퍼유저의 권한이 필요하다.
Superuser라면 명령 앞에 "sudo"를 놓으며, Superuser 세션을 종료하려면 "exit"를 입력한다.

## Text Editors
CLI - based text editors : vi, vim / Emacs / nano
GUI - based text editors : gedit / kwrite


## Tips

### Backslash : 
명령의 행 변경을 무시하고, 여러 행에 Long Command를 입력하는 데 사용할 수 있다.
### History:
이전 명령 기록을 보거나, 이를 텍스트 파일 형식으로 저장할 수 있다.
