## docker-study

#### 도커가 무엇이며 도커를 설치하고 사용하는 법까지 익혀보자

<hr>

<img src="https://user-images.githubusercontent.com/118269278/218919796-d4e866e4-edec-4ee8-a2d5-776916782761.png" width=200 height=200>

* 도커(Docker): 컨테이너 기반의 오픈소스 가상화 플랫폼이다.

  * 다양한 프로그램, 실행환경을 컨테이너로 추상화 하고 동일한 인터페이스를 제공하여 프로그램의 배포 및 관리를 단순하게 해준다.
  
  * 백엔드 프로그램, 데이터베이스 서버, 메시지 큐등 어떤 프로그램도 Container를 추상화 할 수 있고,<br>PC, AWS, Google Cloud 등 어디에서든 실행 가능하다.
  
<hr>

<img src="https://user-images.githubusercontent.com/118269278/218923208-4424ce88-0570-4527-a3b2-1d0895a1e397.png" width=400 height=300/>

<img src="https://subicura.com/generated/assets/article_images/2017-01-19-docker-guide-for-beginners-1/vm-vs-docker-1000-895d2c06e.webp" width=400 height=300/>

- Container
  * 이전 방식 Vmware 등은 사용법이 간단하지만, 무겁고 느리다.
  * CPU의 가상화 기술을 이용한 반 가상화 방식 Xen을 사용
  * 전체 OS를 가상화 하지 않고 Host OS를 가상화
  * 하나의 서버에 여러 개의 Container 가능
  
- Image
  * Container에 필요한 파일과 설정 값 등을 포함
  * Image 안에 여러 개의 Container
  * Docker hub을 통해 필요한 Image를 다운 가능
  
  
<hr>


* Docker 설치
   * 가상화가 사용 가능하다면 Docker가 실행이 가능하다


Docker Desktop for Windows<br>
https://docs.docker.com/desktop/install/windows-install/
<br>

### 설치가 완료되면 Docker Desktop를 실행 후 Tutorial를 진행하면 된다.
   
<img width="500" alt="docker-tutorial" src="https://user-images.githubusercontent.com/118269278/218971909-babdabfe-94b0-4d45-b567-8979ff63c798.png">

그리고 cmd 창에 아래 설명을 통해 입력하면 Docker 버전을 확인할 수 있다.

'''
docker -v
'''
