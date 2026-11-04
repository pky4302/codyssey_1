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

Ubuntu Linux 터미널 기본 명령어 실습

1. 현재위치: pwd
   
   <img width="661" height="45" alt="image" src="https://github.com/user-attachments/assets/5ac1d0c7-2108-40e1-b5f4-bb28d6dc01aa" />

2. ~ 기호는 현재 Linux 사용자의 홈 디렉토리 (pwd의 결과는 Windows 사용자 폴더와 별개인 Linux 사용자 공간): cd ~

   <img width="667" height="70" alt="image" src="https://github.com/user-attachments/assets/c37a5bcb-f07b-4825-97d3-ac326e6f0509" />

3. 폴더생성: mkdir -p ~/codyssey/practice (-p는 상위폴더 없이도 생성)

   <img width="691" height="96" alt="image" src="https://github.com/user-attachments/assets/86d48d5a-9923-46ec-95e9-dada8919e212" />

4. 숨김 파일 포함 목록 확인: ls -la (-l은 상세정보표시, -a는 숨김파일확인)

   <img width="696" height="122" alt="image" src="https://github.com/user-attachments/assets/c7581ff0-b5cb-4978-98db-1a521b811c99" />

5. 파일생성: touch hello.txt

   <img width="752" height="100" alt="image" src="https://github.com/user-attachments/assets/1dad5bf9-8c3a-4599-a889-a40fc9d60e63" />

6. 파일내용작성하기: echo "Hello Linux" > hello.txt ( > 기존 내용 덮어쓰기, >> 기존 내용 뒤에 추가) & 파일내용확인하기: cat hello.txt

   <img width="932" height="67" alt="image" src="https://github.com/user-attachments/assets/a5d868ba-550c-44b4-bf68-d09fc9e1f099" />

7. 파일복사: cp hello.txt hello_copy.txt

   <img width="900" height="121" alt="image" src="https://github.com/user-attachments/assets/a9459d43-28c4-4cde-af89-e548aaacb653" />

8. 파일이름변경: mv hello_copy.txt linux_copy.txt (리눅스에서 mv는 파일이동과 이름변경 모두 가능)

   <img width="957" height="119" alt="image" src="https://github.com/user-attachments/assets/c34870da-a859-46ad-9769-241c202c3b4a" />

9. 파일삭제: rm linux.txt_copy.txt

   <img width="777" height="93" alt="image" src="https://github.com/user-attachments/assets/c1f45825-a467-4e8a-9825-fda1c898471d" />

10. 권한실습파일 생성: echo "Permission Test" > permission.txt (파일과 파일내용을 동시에 생성)

   <img width="1034" height="167" alt="image" src="https://github.com/user-attachments/assets/c86acb11-e745-4e89-a5e8-57add87c391b" />

   권한정보

   <img width="811" height="44" alt="image" src="https://github.com/user-attachments/assets/ca20523e-a590-498a-a55b-031d6f00a7f2" />

11. 권한변경: chmod 600 permission.txt (600, 소유자만 읽고 쓰기 가능)

    <img width="860" height="73" alt="image" src="https://github.com/user-attachments/assets/1bb21f31-e431-47e5-8de4-cdc7bf23cc60" />

---------------------------------------------------------------------------------------------------------------------

Docker 설치

<img width="1330" height="496" alt="image" src="https://github.com/user-attachments/assets/1525c2ba-7cec-4dfb-b38f-1f2bdc27938e" />

<img width="631" height="535" alt="image" src="https://github.com/user-attachments/assets/c46c5151-43f6-4387-9838-de5a146b0257" />

1. Docker 엔진이 Ubuntu에서도 작동확인: docker --version

   <img width="554" height="50" alt="image" src="https://github.com/user-attachments/assets/64652a1c-c4ca-4b15-9407-759976af8707" />

2. 현재 Ubuntu 사용자가 Docker 엔진에 접근할 권한 관련 명령어
   
   2-1. ls -l /var/run/docker.sock => Docker 엔진에 접근하는 소켓 파일의 소유자와 권한
        (root소켓소유자, docker소켓접근가능그룹, 현재사용자)
   
   <img width="1506" height="94" alt="image" src="https://github.com/user-attachments/assets/fe11963a-7870-4914-81ee-02e8b44621ba" />

   2-2. 우분트 도커 그룹에 추가: sudo usermod -aG docker $USER

   2-3. 현재 터미널에서 그룹 변경적용: newgrp docker

   2-4. 다음 getent group docker 입력 후 윈도우 파워셀에서 wsl --shutdown하고 다시 우분트에서 id확인

   <img width="1667" height="815" alt="image" src="https://github.com/user-attachments/assets/247aefa2-861f-4304-b45a-31d88b63ce19" />

3. 우분트에서 도커 정상 작동되면

   3-1.첫 번째 컨테이너 생성 및 실행 명령어: docker run hello-world

   <img width="510" height="334" alt="image" src="https://github.com/user-attachments/assets/080a67e2-24b0-40f2-b0de-8566601f0394" />

   3-2.이미지와 컨테이너 구분하기: docker images = docker image ls

   <img width="1041" height="605" alt="image" src="https://github.com/user-attachments/assets/f17f0b95-1caa-4cd4-bf8d-0d16ed58f4fb" />

    3-3.컨테이너 확인하기: docker ps -a
        docker ps: 현재 실행 중인 컨테이너 확인
        docker ps -a: 종료된 컨테이너까지 모두 확인
        exit(0) => 컨테이너 실행 정상적 종료
   <img width="1318" height="76" alt="image" src="https://github.com/user-attachments/assets/de65bca0-e8ba-42e1-9dc5-2dd5303030b0" />

   3-4.my-hello라는 이름의 새 컨테이너 만들기: docker run --name my-hello hello-world

   <img width="1318" height="653" alt="image" src="https://github.com/user-attachments/assets/87d8f0a6-3fc0-4f7b-96c9-aa37809763d6" />

    3-5. 최근에 만든 이미지로 컨테이너이름(my-ubuntu) 지정 후 백그라운에서 종료하지 않고 계속 대기하는 컨테이너 생성 및 실행: docker run -d --name my-ubuntu ubuntu:latest sleep infinity

    <img width="1437" height="598" alt="image" src="https://github.com/user-attachments/assets/7a40753d-4469-4102-bc92-19e55b353636" />

4. 우분트 안에서 또다른 우분트 환경에 들어가기 (도커 컨테이너 내부 들어가기)

   4-1. docker exec -it my-ubuntu bash (실행 중인 컨테이너에서 계속 입력 받고 터미널 환경제공, 접속할 컨테이너 명, 실행할 셀 프로그램)

   root@xxxxxxxxxxxx: Docker 컨테이너 내부 환경으로 이동, root는 컨테이너 내부의 관리자 계정, /는 컨테이너의 최상위 디렉터리
   
   <img width="715" height="50" alt="image" src="https://github.com/user-attachments/assets/df698c70-8acd-488b-b4fd-97d962fcc6e6" />

   

   4-2. 컨테이너 내부접근: 현재위치확인: pwd, Linux버전: cat /etc/os-release, 파일목록확인: ls -la(숨긴파일까지)
   
<img width="1005" height="983" alt="image" src="https://github.com/user-attachments/assets/b2f58144-6771-44c6-8d82-cd53706bd577" />     

   4-3. 컨테이너 내부에 파일 만들기: echo "Hello Docker" > hello.txt

<img width="376" height="276" alt="image" src="https://github.com/user-attachments/assets/d1ba6faa-602e-43ab-819e-4152d7b849f9" />

   4-4. 파일내용확인: cat hello.txt
   
   <img width="413" height="47" alt="image" src="https://github.com/user-attachments/assets/519d1449-1e0a-46fa-bbe9-ba34781be176" />

   4-5. 컨테이너 접속 종료: exit

   <img width="230" height="35" alt="image" src="https://github.com/user-attachments/assets/0423aa31-a823-48dd-9669-d47aabf8e814" />

5. 실행중인 컨테이너 확인하고 중지하고 다시 실행하고 삭제하기

   5-1. my-ubuntu 컨테이너 확인: docker ps

   <img width="1235" height="69" alt="image" src="https://github.com/user-attachments/assets/771b0dc6-0b0d-4832-805f-7dd08ced6195" />

   5-2. 컨테이너 중지: docker stop my-ubuntu

   <img width="852" height="96" alt="image" src="https://github.com/user-attachments/assets/cb55fbce-016a-4639-ad4d-20e63016d0c0" />

   5-3. 컨테이너 다시 실행: docker start my-ubuntu

   <img width="1224" height="116" alt="image" src="https://github.com/user-attachments/assets/82dc0401-4892-48a7-9131-76e64ea97a73" />

   5-4. 컨테이너 삭제: docker rm -f my-ubuntu

   <img width="619" height="45" alt="image" src="https://github.com/user-attachments/assets/6b4045ff-37dc-49b5-9d79-5a7b7f106582" />

   <img width="1383" height="99" alt="image" src="https://github.com/user-attachments/assets/d3cdfe37-b623-464a-bb4b-ab6405146ab9" />

   컨테이너를 삭제해도 이미지는 남아있음

   <img width="421" height="74" alt="image" src="https://github.com/user-attachments/assets/85341a15-2359-43ef-add0-6aedafc003f7" />

   5-5. 남아있는 이미지 삭제: docker image rm ubuntu:latest

   <img width="970" height="194" alt="image" src="https://github.com/user-attachments/assets/1490b42f-9017-4394-9b74-3b23aa0dd024" />

6. 도커파일 실습

   6-1. 실습폴더생성: mkdir docker-study

   <img width="322" height="46" alt="image" src="https://github.com/user-attachments/assets/96b4064d-d443-4602-9c0e-02325085656c" />

   6-2. 도커파일작성하기: nano Dokerfile (DockerFile 오타로 mv DockerFile Dockerfile 명령어로 수정)

         도커파일 작성: FROM ubuntu:latest(우분트에서 이미 만 기본 이미지)
                       CMD["echo", "Hello Dockerfile!"] (컨테이너실행시 보이는 것) => 문자를 출력하는 이미지 만들기 위함.

         도커파일빌드하는 법(만약 하나의 dir에 a_file, b_file 있을 때: docker build -t image1 . => a_file,  docker build -t image2 -f b_file . => b_file)  (" . "은 현재 dir 빌드 컨텍스트로 지정한다는 뜻) 

   <img width="721" height="434" alt="image" src="https://github.com/user-attachments/assets/3ad89ec8-2ade-4664-b2cc-cf4ff8bb6abd" />

   6-3. 빌드 후 이미지 생성이 확인되면 이미지로 컨테이너 만들고 실행하기: docker run --name my-study-container my-docker-study
        
<img width="832" height="86" alt="image" src="https://github.com/user-attachments/assets/baef26a0-927a-4f19-b238-d49f0c42dcbd" />

   6-4. 컨테이너 로그 확인: docker logs my-study-container (컨테이너 출력 로그 확인, 누적된 결과)
        컨테이너 다시 실행: docker start -a my-study-container (-a는 터미널에서 출력내용 보이게 하기)
        
<img width="940" height="95" alt="image" src="https://github.com/user-attachments/assets/4bf0e6dd-6d77-483e-81c1-ea91f23e3929" />

  6-5. 컨테이너 삭제 후 이미지 남아있는 지 확인: docker rm -f my-study-container

<img width="635" height="158" alt="image" src="https://github.com/user-attachments/assets/7f5f4777-9780-4a70-bd6c-56a9fd410fe4" />

  6-6. 빌드한 이미지 삭제: docker image rm my-docker-study:latest (이미지 컨테이너는 도커가 관리하기 때문에 dir랑 상관X, 도커파일은 dir관리)

<img width="982" height="192" alt="image" src="https://github.com/user-attachments/assets/daac697f-e09c-4101-ba67-9c720ab485a9" />















   
