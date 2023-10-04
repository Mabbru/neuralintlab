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
