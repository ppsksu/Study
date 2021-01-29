- 윈도우 키 + R => notepad 입력 (메모장 열림)  
  notepad라고 입력 후 .bat으로 저장 => 메모장 실행 됨  


  mspaint (그림판)  
  ncpa.cpl (네트워크 연결)  
  devmgmt.msc (장치 관리자)  
  sysdm.cpl (시스템 속성)  
  explorer.exe c:\ (윈도우 탐색기)  
  diskmgmt.msc (디스크 관리자)  
  lusrmgr.msc (로컬 사용자 및 그룹)  
  eventvwr.msc (이벤트 뷰어)  
  control (제어판)  
  firewall.cpl (방화벽)  
  appwiz.cpl (프로그램 추가 및 제거)  
  services.msc (서비스 관리창)  

  이런 것들을 입력 해 보고 실행 해 봄  
  
- #### Echo에 대해  
> @echo off  
  notepad 
  
 입력하고 저장
 (실행해 보면 콘솔창에 메세지가 뜨지 않고 메모장이 나옴)
  
- #### Echo를 이용해서 콘솔창에 출력  
> @echo off  
   echo Test  
   notepad  
   
입력하고 저장  
(실행해 보면 콘솔창에 메세지가 뜨지 않고 메모장이 나옴)

- #### Echo를 이용해서 빈줄(Enter) 출력  
> @echo off  
   echo Test  
   echo.
   echo Test  
   notepad    
 
echo. 부분에 빈줄이 출력 됨

> #### 요약  
@echo off는 자신이 입력한 배치파일 명령어를 출력하지 않는기능을 한다.  
@echo off 를 하더라도 echo 명령어를 사용함으로써 자신이 원하는 문장을 출력할수 있게 하는 기능을 한다.



- #### Set(변수설정  
배치파일에서 변수를 설정하기 위해 Set 명령어를 이용  

|명령어|사용법|설명|
|:---|:---|:---|
|set  |set 변수 = 값  |변수에 값을 넣습니다.  |
|set/a  |set/a 변수 = 계산식  |변수에 계산한 값을 넣습니다.  |
|set/p  |set/p 변수 = [화면출력  |변수에 사용자로부터 입력받은 값을 넣습니다.  |

- #### set  
> @echo off
set var=10
echo %var%
notepad  

메모장과 함께 정상적으로 출력됨  
화면에 변수를 출력해주기 위해서는 %변수% 가 필요하다.
%없이 변수명만 입력을 한다면, 변수명만 화면에 출력이 된다.
주의 : var=10 붙여 쓸 것 = 사이에 공백 넣으면 안됨  

- #### set/


