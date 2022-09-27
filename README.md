# [Open Source SoftWare] - Git Bash Lecture Note    

---



##### **pwd : Shows the current path in a hierarachical directory**
    
```sh
$ pwd
$ /c/Users/58766
$
```
   
\! 현재의 Path 혹은 Directory를 보여주는 명령어    
   Linux 체제와 Windows 체제의 보여지는 방식에 차이가 있음   
     
     
 ---
 
     
##### **cd : change directory**  
##### **ls : list files and directories**       
     
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
\/\[directory name\] :  여러 파일 한 번에 들어갈 때 중괄호에 이름 넣기     
..\/[directory name] : 한 단계 위 파일에 있는 파일 중 중괄호에 들어간 파일로 가기    


---

##### **cp : copy files and directories**      


```sh
$ pwd
/c/Users/58766/OSS/transformers
$ ls
README.md   classfication_experiment.py   module.py
$ cp module.py   backup_module.py    //cp  원본  복사경로
$ ls
README.md   backup_module.py   classfication_experiment.py   module.py    //파일 복사 됨
$ cp -r ..\/neuralintlab .        // -r 옵션을 써서 해당 디렉토리 안의 하위 파일도 복사하라는 의미 상위 디렉토리를 현재 디렉토리에 복사하는 코드
$ ls
README.md   backup_module.py   classfication_experiment.py   module.py   neuralintlab
$ cd neuralintlab
$ ls
README.md
$ pwd
/c/Users/58766/OSS/transformers/neuralintlab
$
```
    
    
/! 디렉토리나 파일을 복사한다.
    
   
   

---

##### **mv : move files and directories or rename them**    
   
   
```sh
$ pwd
/c/Users/58766/OSS/transformers
$ ls
README.md   backup_module.py   classfication_experiment.py   module.py   neuralintlab
$ mv module.py new_module.py    //파일 이름 바꿈
README.md   backup_module.py   classfication_experiment.py   neuralintlab   new_module.py   //module.py가 사라지고 new_module.py가 생김
$ mv. new_module.py ..\/neuralintlab   //파일을 현 디렉토리에서 상위 디렉토리로 옮김
$ cd ..\/neuralintlab
$ ls
README.md   new_module.py   
$ cd ..\/transformers
$ mv neuralintlab nil   //디렉토리 이름을 바꿔줌
$ ls
README.md   backup_module.py   classification_experiment.py   nil
$
```
    
       
\! 디렉토리나 파일의 이름을 바꾸거나, 디렉토리나 파일의 위치를 바꾼다
   
   
---  
         
##### **rm : delete files and directories permantely and irreversevely!!!**   
    
\! 파일이나 디렉토리를 영구적이고 복구가 불가능하게 지워버림    
    
        
---
    
##### **mkdir : make a new directory**    
        
```sh
$ ls
neuralintlab   transformers   
$ mkdir new_directory
$ ls
neuralintlab   new_directory
$
```
     
\! 현재 디렉토리 안에 새로운 디렉토리 만들기




