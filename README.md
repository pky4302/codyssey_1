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

6. 도커파일 생성 빌드

   6-1. 실습폴더생성: mkdir docker-study

   <img width="322" height="46" alt="image" src="https://github.com/user-attachments/assets/96b4064d-d443-4602-9c0e-02325085656c" />

   6-2. 도커파일작성하기: nano Dokerfile (DockerFile 오타로 mv DockerFile Dockerfile 명령어로 수정)

도커파일 작성: FROM ubuntu:latest(우분트에서 이미 만 기본 이미지)
CMD["echo", "Hello Dockerfile!"] (컨테이너실행시 보이는 것) => 문자를 출력하는 이미지 만들기 위함.


도커파일빌드하는 법(만약 하나의 dir에 a_file, b_file 있을 때: docker build -t image1 . => a_file,
     docker build -t image2 -f b_file . => b_file)  (" . "은 현재 dir 빌드 컨텍스트로 지정한다는 뜻)

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

7. 내 컴퓨터의 hello.txt를 Docker 이미지 내부의 /app/hello.txt로 복사하기

<img width="351" height="152" alt="image" src="https://github.com/user-attachments/assets/5867512e-b7c2-47eb-9449-5c28b3115385" />

nano Dockerfile로 도커파일 수정하기 (만약 빌드하고했는 데 파일에 오타가 있으면 파일 수정 후 다시 빌드하고 기존 컨테이너 삭제 후 다시 컨테이너 생성 실행 해야함)
   
<img width="742" height="59" alt="image" src="https://github.com/user-attachments/assets/34903ef3-9774-47c2-a8a2-9fc940e7e76d" />


8. 도커파일에서 작업 디렉토리 지정

 컨테이너 실행이 이미지 내부 /app 디렉토리에서 이루어지게 할 때

 <img width="226" height="201" alt="image" src="https://github.com/user-attachments/assets/4e26f9c3-e3d3-4ffb-9dbd-ad269a6fb2bd" />

 pwd를 실행했으니 /app 현위치 나옴

<img width="1071" height="50" alt="image" src="https://github.com/user-attachments/assets/b86f5516-c791-4e9d-91b0-c935a2d202d8" />

  새 컨테이너 실행하고 Bash 실행: docker run -it --name workdir-test my-docker-study bash (-i 컨테이너입력, -t 터미널 환경 )

<img width="1211" height="145" alt="image" src="https://github.com/user-attachments/assets/d5a6eaf7-eca7-4281-9741-d9daac9d922e" />

WORKDIR /app이 컨테이너의 기본 작업 위치로 적용된다는 것을 직접 확인할 수 있음 ↑


<img width="686" height="205" alt="image" src="https://github.com/user-attachments/assets/503d65cd-5222-4d92-8932-219ace94920e" />

같은 이미지로 여러 컨테이너를 생성할 수 있고 서로 독립적임.↑

9. 도커볼륨 (웹 서비스에서 DB 같은 것)

  9-1. 도커볼륨생성: docker volume create study-volume

  <img width="914" height="119" alt="image" src="https://github.com/user-attachments/assets/ce9b2760-c063-44ed-bb25-a60ec11260b6" />

  9-2.불륨을 컨테이너 내부와 연결하기: docker run -it --name volume-test -v study-volume:/data ubuntu:latest bash

  -v: 볼륨을 컨테이너 내부 /data에 연결 (볼륨생성도 같이됨)

   그 후 컨테이너 내부에서 데이터 저장하기: echo "Docker Volume Data" > /data/hello.txt

<img width="495" height="49" alt="image" src="https://github.com/user-attachments/assets/d5b3c25d-2187-481a-ae7b-23afa3af4079" />

  9-3.컨테이너 삭제 후 데이터 확인하기

      기존 컨테이너 삭제 후,
      
      새로운 컨테이너를 생성하고 study-volume과 연결하여 확인: docker run -it --name volume-test2 -v study-volume:/data ubuntu:latest bash

<img width="1440" height="76" alt="image" src="https://github.com/user-attachments/assets/279dcc1f-4ad3-496c-884b-75d8ccf9e337" />

볼륨에 저장된 것을 받아옴 확인↑

 9-4.볼륨삭제: docker volume rm study-volume

10. 도커 -p(포트) 옵션으로 컨테이너 포트를 외부에 연결하기

  10-1.Winodows 8080 포트로 들어온 요청을 컨테이너 80 포트로 전달하기: docker run -d --name web-test -p 8080:80 nginx:latest

<img width="1186" height="355" alt="image" src="https://github.com/user-attachments/assets/cba8c041-25e3-4446-9e20-0af25c474a3f" />

<img width="1839" height="74" alt="image" src="https://github.com/user-attachments/assets/2bd9604e-d347-48d7-9eb3-332a3791d41a" />

  그리고 localhost:8080 에서 Nginx연결 확인 => Docker 컨테이너 내부에서 실행되는 웹 서버에 Windows 웹 브라우저로 접속하는 데 성공했다는 뜻, Nginx가 실행되고 있더라도 -p 옵션으로 포트연결하지 않으면 외부에 접속할 수 있도록 공개하지 않음

   10-2. 도커 네트워크 확인법: docker network ls

    bridge 기본, host 호스트, none 연결X

    bridge는 Docker가 기본으로 제공하는 네트워크, 컨테이너 끼리 이름으로 통신 편함

    10-3.사용자 정의 네트워크 만들기: docker network create study-network

<img width="939" height="192" alt="image" src="https://github.com/user-attachments/assets/19663ca1-77f3-4b09-9f85-75e0c468fa71" />

    10-4. 생성한 네트워크에 컨테이너 2개 연결하기: 
      docker run -dit --name network-test1 --network study-network ubuntu:latest bash
      docker run -dit --name network-test2 --network study-network ubuntu:latest bash

      컨테이너 생성 후 네트워크 연결확인: docker network inspect study-network

<img width="545" height="552" alt="image" src="https://github.com/user-attachments/assets/d4084e07-3cbe-4e63-8038-ea1c89c65c7a" />

    10-5. 첫번째 컨테이너에서 두번째 컨테이너 찾기

        첫번째 컨테이너 접속: docker exec -it network-test1 bash

        접속 후 ping이라는 네트워크 통신 테스트 프로그램을 설치하고 컨테이너 간 통신 테스트하기

<img width="1094" height="361" alt="image" src="https://github.com/user-attachments/assets/46620448-fbdc-4a91-aa3c-84d8eb1e9407" />

         network-test2 컨테이너와 연결됨을 확임↑ 
         (4번 통신 후 종료: ping -c 4 network-test2)


11. 도커 컴포즈

    도커컴포즈 설치확인: docker compose version => Docker Compose version v5.6.1

    11-1 도커컴포즈폴더 만들고 그곳에서 nano compose.yaml 작성 (도커컴포즈환경설정)

<img width="386" height="170" alt="image" src="https://github.com/user-attachments/assets/29ef9468-146e-437e-8862-e5b68314e6af" />


    11-2. 도커컴포즈 설정확인: docker compose config

<img width="941" height="382" alt="image" src="https://github.com/user-attachments/assets/8ea62e9f-2a46-45f4-9e85-efa72284569e" />

    11-3. 도커컴포즈 설정에 따라 실행: docker compose up -d (만약 다른 yaml파일이 있으면 docker compose -f X.yaml up -d)

<img width="949" height="122" alt="image" src="https://github.com/user-attachments/assets/f28d11fc-c1b4-4fb3-bebd-83f803e827ba" />

    Docker Compose는 컨테이너뿐만 아니라 네트워크도 자동으로 생성,직접 했던 작업을 Compose가 대신 처리한다

     11-4. 컨테이너 실행상태확인: docker compose ps, 만약 컨테이너 종료되면 다시 실행

<img width="1742" height="70" alt="image" src="https://github.com/user-attachments/assets/197713a0-c6be-4a56-9bc8-b04dc69644a7" />

     11-5. 컨테이너 실행 중지와 재시작(삭제는 안됨): docker compose stop, docker compose start

<img width="821" height="267" alt="image" src="https://github.com/user-attachments/assets/05aca1c5-e159-4140-a5d5-dc2bf113ba26" />

     11-6. 컨테이너 중지 후 삭제(이미지까지 삭제하지 않음): docker compose down

<img width="944" height="144" alt="image" src="https://github.com/user-attachments/assets/d797dd75-48bb-40ee-8434-4f32106d0dc4" />

    11-7. 삭제된 컨테이너를 컴포즈설정에 따라 다시 생성 실행: docker compose up -d

 <img width="1656" height="166" alt="image" src="https://github.com/user-attachments/assets/82a38951-145a-493d-8a84-d8352af484f6" />


12. 컴포즈로 개발환경과 운영환경 분리

    12-1. 운영환경,개발환경 yaml만들고 실행 : docker compose -f compose.yaml up -d 그리고 docker compose -f compose-dev.yaml up -d

    하지만 두  yaml파일이 같은 컴포즈 프로젝트 이름을 사용하고 있으면 두 yaml파일을 같은 프로젝트로 인식해 운영환경을 실행하면 개발환경이 꺼지고 개발환경을 실행하면 운영환경이 꺼지는 증상이 생김. 

<img width="842" height="121" alt="image" src="https://github.com/user-attachments/assets/7baa25ba-03eb-4da7-bfd1-74ff026348ea" />

    이를 해결하기 위해 -p로 프로젝트 이름을 분리해야 한다. 컴포즈 프로젝트 이름을 분리하면 같은 디렉터리의 설정 파일을 사용하더라도 서로 독립적으로 관리할 수 있어.

    운영: docker compose -p main -f compose.yaml up -d
    개발: docker compose -p dev -f compose.yaml up -d

    실행 후 별도 프로젝트를 조회해야함
    
<img width="1182" height="467" alt="image" src="https://github.com/user-attachments/assets/c99e2cee-ae5a-4b2d-b810-589375361eee" />

<img width="1159" height="466" alt="image" src="https://github.com/user-attachments/assets/2b3f069f-3f80-486c-9fcf-641923e343dc" />

<img width="899" height="73" alt="image" src="https://github.com/user-attachments/assets/ab43f45b-2de4-4f9c-ab28-787ac29b18d5" />

     12-2. 컴포즈 환경변수 사용하기

           compose-env.yaml 파일 만든 후 생성 실행하기
           
 <img width="431" height="250" alt="image" src="https://github.com/user-attachments/assets/e2d1663e-821c-467f-81c5-aad21a2c013d" />

<img width="1713" height="80" alt="image" src="https://github.com/user-attachments/assets/787bbe2c-6aec-403d-9a6b-dcea823f2a31" />

    12-3. 컨테이너 내부로 들어가 환경변수 확인하기

<img width="523" height="98" alt="image" src="https://github.com/user-attachments/assets/fe527c8d-0aef-4f34-b82c-db7bd18e37ec" />

       compose-env.yaml의 environment에 설정한 값이 컨테이너 내부의 환경변수로 전달된 것을 확인할 수 있음.

    12-4. 컨테이너 내부의 환경변수를 직접 가지고 있지 않고 .env를 만들고 그곳에서 가져오기

       .env 파일 ↓
             
  <img width="255" height="93" alt="image" src="https://github.com/user-attachments/assets/0345f845-9b0a-4a64-8de4-506ba5bcf186" />

        compose-env.yaml 수정 ↓
       
<img width="441" height="245" alt="image" src="https://github.com/user-attachments/assets/2432a47a-6f8a-4b02-817a-550b20b72a7e" />

         다시 컴포즈 생성 실행 후 컨테이너에 들어가면 .env에서 가져오는 것을 확인할 수 있음

<img width="505" height="99" alt="image" src="https://github.com/user-attachments/assets/3212ce7b-c6ab-4814-9baf-43bd5d576b7d" />


13. 컴포즈로 두 개의 컨테이너를 연결하기 (웹서버 Nginx와 데이터베이스 컨테이너)
    
    13-1. 웹서버와 데이터베이스 컨테이너 만드는 .yaml파일 생성
  
    <img width="447" height="553" alt="image" src="https://github.com/user-attachments/assets/140ebc3c-a7f2-4e6b-97cd-b5f6e96d4334" />

    13-2. docker compose -f compose-mysql.yaml config를 확인하여 두 컨테이너가 같은 네트워크에 있는 지 확인

<img width="610" height="470" alt="image" src="https://github.com/user-attachments/assets/be9688fe-430e-42c7-9909-6f00913e92b2" />

      네트워크는 프로젝트에 사용할 네트워크를 자동 생성하고 프로젝트 이름을 따서 생성, db 서비스는 yaml에 데이터저장위치에 도커볼륨
      을 연결하겠다 했으니 mysql-data라는 볼륨을 프로젝트 명 뒤에 붙여생성 ↑

<img width="554" height="74" alt="image" src="https://github.com/user-attachments/assets/96f5ba6c-480d-4f03-b7c3-c22b10e4fbfe" />


    13-3. docker compose -f compose-mysql.yaml up -d 컨테이너, 네트워크, 볼륨 동시 생성

<img width="872" height="206" alt="image" src="https://github.com/user-attachments/assets/54835dda-c2f6-4028-baea-a6fbec7f7ea8" />

    13-4. web컨테이너 Nginx 내부에서 MysSQL컨테이너 서비스이름(db) 찾기: getent hosts db

<img width="1135" height="71" alt="image" src="https://github.com/user-attachments/assets/0a589f40-74f3-433d-beb6-9debec84794f" />

         mysql-study-web 컨테이너에서 db서비스 이름을 조회했을 때 도커가 MySQL 컨테이너의 내부 IP 주소를 알려준 것

    13-5. MySQL 컨테이너에 study_user 계정으로 접속확인 후 member 테이블 생성(MySQL-study-db 컨테이너에서 MySQL 서버 접속):
    docker exec -it mysql-study-db mysql -u study_user -p study_db

<img width="1433" height="357" alt="image" src="https://github.com/user-attachments/assets/8f35b1f1-0406-4aa5-a1a0-57cef5120539" />

    13-6. 컨테이너 삭제하기: docker compose -f compose-mysql.yaml down

<img width="1224" height="288" alt="image" src="https://github.com/user-attachments/assets/ffef7fa7-d6ba-4df8-846a-56e73bae9802" />

    13-7. 컨테이너 삭제 후 볼륨 영속성확인

<img width="875" height="74" alt="image" src="https://github.com/user-attachments/assets/f98d06bd-43d4-474e-809c-1141af83efd4" />

    컴포즈로 생성 실행했을 때 만든 볼륨이 존재함 ↑

   
   13-8. 이전 컨테이너 삭제하고 다시 컨테이너 생성해도 볼륨은 기존 것 재사용됨

     => 만약 볼륨이 없었더라면 MySQL 컨테이너 안에 데이터가 저장된다 해도 컨테이너 삭제 하면 컨테이너 내부에만 저장된 데이터는
     사라질 수 있음
        하지만, 볼륨을 사용하면 MySQL 서버가 볼륨에 데이터를 읽고 쓰는 역할을 하기 때문에 컨테이너를 삭제해도 볼륨의 영속성 때문에
        데이터를 보존할 수 있음
     =>  MySQL 서버는 데이터를 관리하는 프로그램이고, Docker 볼륨은 그 데이터가 지속적으로 저장되는 공간임.

<img width="1432" height="816" alt="image" src="https://github.com/user-attachments/assets/a3bf87d3-8fc4-47a3-a601-d3caa2bbb658" />

        맨처음 컨테이너 만들었을 때 MySQL서버에서 member 테이블을 만든 것이 컨테이너 삭제 후 다시 생성해도 볼륨을 읽어들여
        볼 수 있음을 확인할 수 있음.


   13-9. 임시로 만든 클라이언트 컨테이너에서 MySQL 서버 접속 :
   docker run --rm -it --network compose-study_default mysql:8.4 mysql -h db -u study_user -p study_db

<img width="1873" height="652" alt="image" src="https://github.com/user-attachments/assets/e272631b-bed7-45c4-8756-7763bac8d03e" />

   기존 컴포즈 네트워크를 쓰고 MySql서버 service이름(db)를 찾아 Mysql 접속 후 임시컨테이너 종료되면 자동삭제하는 명령어 ↑
   

14. MySQL 서버 로그 및 Nginx 웹서버 로그 확인

    14-1. MySQL 서비스 로그확인: docker compose -f compose-mysql.yaml logs db --tail 20

<img width="431" height="60" alt="image" src="https://github.com/user-attachments/assets/23c0cb7f-bb22-4d4d-ada0-ddf7faed3a57" />

<img width="1337" height="26" alt="image" src="https://github.com/user-attachments/assets/37f385a7-5b3f-48fa-b015-b9699c24592e" />

    14-2. Nginx 웹 서버 접속 확인: curl http://localhost:8085

 <img width="991" height="669" alt="image" src="https://github.com/user-attachments/assets/199967fd-b3e2-4f81-8caf-0be52359fae8" />

----------------------------------------------------------------------------------------------------------------------------------------

깃 허브 연동
