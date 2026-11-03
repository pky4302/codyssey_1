# codyssey_1
코디세이 1주 과제

Windows 11 OS PowerShell 명령어 실습

파일경로

C:\
 └─ Users
     └─ pky61476147
         ├─ codyssey_test
         │   └─ XXXX
         │
         └─ move
             └─ XXXX
         

1.현재위치찾기
  명령어: pwd
  
  <img width="415" height="139" alt="image" src="https://github.com/user-attachments/assets/6b50bbe1-6f71-4250-9734-993a564f1790" />

2.현재폴더의 파일 목록 확인
  명령어: ls
  
  <img width="870" height="545" alt="image" src="https://github.com/user-attachments/assets/e3657a96-0475-4aed-ab80-7919ff485148" />

3. 숨김파일까지 확인
   명령어: ls - force
   
   <img width="932" height="550" alt="image" src="https://github.com/user-attachments/assets/0943f1e3-248a-458b-9e41-4ce32b666c9d" />

4. 작업폴더생성
   명령어: mkdir
   
   <img width="454" height="441" alt="image" src="https://github.com/user-attachments/assets/93a52652-ceea-4f66-bb4b-97ae597b68ca" />

5. 빈파일생성 (codyssey_test 폴더로 이동 후 목록 빈파일 생성)
   명령어: New-Item hello.txt -ItemType File
   
   <img width="1022" height="601" alt="image" src="https://github.com/user-attachments/assets/e6694ae3-cd46-4be1-bed5-cafec3fc8d88" />

6. 파일내용작성하기 & 작성내용보기
   명령어: Set-Content hello.txt "Hello codyssey" 와 Get-Content hello.txt
   
   <img width="1095" height="91" alt="image" src="https://github.com/user-attachments/assets/595360bc-1b71-445d-966d-ddb6822a48d9" />

7. 파일복사 (hello.txt를 hello_codyssey.txt로 복사)
   명령어: Copy-Item hello.txt hello_codyssey.txt

   <img width="545" height="157" alt="image" src="https://github.com/user-attachments/assets/648f87f3-affc-4180-b066-862898d1aa28" />

8. 파일이름변경 (hello_codyssey 파일이름을 hello_cody로 바꾸기)
   명령어: Rename-Item hello_codyssey.txt hello_cody.txt

   <img width="1191" height="314" alt="image" src="https://github.com/user-attachments/assets/df86054a-8866-402f-8680-014c37653f47" />

9. 파일이동 (codyssey_test 폴더에 있는 복사본 hello_cody.txt 파일을 상위폴더에 있는 move 폴더로 이동)
   명령어: Move-Item hello_cody.txt "C:\Users\pky61476147\move" 또는 Move-Item ".\hello_cody.txt" "..\move" (hello_cody.txt는 현재 내가 작업하고 있는 폴더를 기준으로 찾는 상대 경로, 만약 "C:\Users\pky61476147\codyssey_test\hello_cody.txt" 직접입력하면 절대경로)

  <img width="1290" height="364" alt="image" src="https://github.com/user-attachments/assets/7f2ec551-b4bd-4050-8760-bde88b24a692" />

10. 복사했던 내용삭제
    
    명령어: Remove-Item move\hello_cody.txt

    <img width="807" height="176" alt="image" src="https://github.com/user-attachments/assets/49cbc6c2-7191-41b8-8da5-20effe0b4690" />
----------------------------------------------------------------------------------------------------------------------------------------

Ubuntu Linux 터미널 명령어

1. 현재위치: pwd
   
   <img width="661" height="45" alt="image" src="https://github.com/user-attachments/assets/5ac1d0c7-2108-40e1-b5f4-bb28d6dc01aa" />

2. ~ 기호는 현재 Linux 사용자의 홈 디렉토리 (pwd의 결과는 Windows 사용자 폴더와 별개인 Linux 사용자 공간입니다.) : cd ~

   <img width="667" height="70" alt="image" src="https://github.com/user-attachments/assets/c37a5bcb-f07b-4825-97d3-ac326e6f0509" />

3. 폴더생성 : mkdir -p ~/codyssey/practice (-p는 상위폴더 없이도 생성)

   <img width="691" height="96" alt="image" src="https://github.com/user-attachments/assets/86d48d5a-9923-46ec-95e9-dada8919e212" />

4. 





  

   




  


