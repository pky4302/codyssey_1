# codyssey_1
코디세이 1주 과제

Windows 11 OS

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

9. 파일이동 (codyssey_test 폴더에 있는 복사본 hello_cody.txt 파일을 move 폴더로 이동)
   명령어: Move-Item hello_cody.txt "C:\Users\pky61476147\move" (hello_cody.txt는 현재 작업 폴더를 기준으로 찾는 상대 경로, 만약 "C:\Users\pky61476147\codyssey_test\hello_cody.txt" 직접입력하면 절대경로)
  <img width="1290" height="364" alt="image" src="https://github.com/user-attachments/assets/7f2ec551-b4bd-4050-8760-bde88b24a692" />

10. 
  

   




  


