# [Open Source SoftWare] - Git Bash Lecture Note    

---



##### pwd : Shows the current path in a hierarachical directory

```sh
$ pwd
$ /c/Users/58766
$
```

\! 현재의 Path 혹은 Directory를 보여주는 명령어    
   Linux 체제와 Windows 체제의 보여지는 방식에 차이가 있음
   
   


##### cd : change directory
##### ls : list files and directories   

```sh
$ pwd
/c/Users/58766
$ ls
Backup OSS Music Study
$ cd OSS
$ pwd
/c/Users/58766/OSS
$ ls
neuralintlab transformers   
$
```

\! cd는 디렉토리를 변경하고, ls는 파일이나 디렉토리를 출력한다
   이때, 대소문자는 구별된다.
   
\+ cd 뒤에 오는 arguments
\/ : 최상위 폴더
. : 최근 디렉토리
.. : 한 단계 위 디렉토리
\/[directory name] :  여러 파일 한 번에 들어갈 때 중괄호에 이름 넣기
..\/[directory name] : 한 단계 위 파일에 있는 파일 중 중괄호에 들어간 파일로 가기
