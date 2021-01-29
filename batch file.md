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

- > @echo off  
    notepad 
  
 입력하고 저장
 (실행해 보면 콘솔창에 메세지가 뜨지 않고 메모장이 나옴)
  
 #### Echo를 이용해서 콘솔창에 출력  
 - > @echo off  
     echo Test  
     notepad  
   
입력하고 저장  
(실행해 보면 콘솔창에 메세지가 뜨지 않고 메모장이 나옴)

#### Echo를 이용해서 빈줄(Enter) 출력  
 - > @echo off  
     echo Test  
     echo.
     echo Test  
     notepad    
 
echo. 부분에 빈줄이 출력 됨
