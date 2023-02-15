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

<br>
  
### 단어 정리<br>
#### VMWare: Virtual Machine 이라는 개념 즉, 가상의 기계장치
#### Xen: 오픈소스 하이퍼바이저 중 하나로, 하드웨어 위에서 실행되는 Type1의 형태 또는 베어 메탈 형태의 가상화 기술<br>
#### HostOS: 물리 머신위에 직접동작하는 OS<br>

  
<hr>


* Docker 설치
   * 가상화가 사용 가능하다면 Docker가 실행이 가능하다


Docker Desktop for Windows<br>
https://docs.docker.com/desktop/install/windows-install/
<br>

### 설치가 완료되면 Docker Desktop를 실행 후 Tutorial를 진행하면 된다.
   
   
<img width="500" alt="docker-tutorial" src="https://user-images.githubusercontent.com/118269278/218971909-babdabfe-94b0-4d45-b567-8979ff63c798.png">

<br>

cmd 창에 아래 설명을 통해 입력하면 Docker 버전을 확인할 수 있다.

```
docker -v
```

<img src="https://user-images.githubusercontent.com/118269278/218973919-9c9cab75-3eaf-4f03-bbf2-a019da0c0b26.png" width=800 height=300 />

<hr>

<br>
<div>
위에서 말했던 것처럼 Image와 Container로 구성되어 있다고 했다.

그래서 Docker의 Image 목록을 찾기 위해서는 Docker hub을 통해서 찾아야 한다.
</div>

<br><br>
예를 들어 Docker의 CentOS Image를 다운받고 싶으면 CentOS 검색을 통해서 다운 받으면 된다.

![cent-os](https://user-images.githubusercontent.com/118269278/218975613-fc39bd1b-f601-4414-9b9d-5a177c5138ff.png)

또한 cmd 아래의 명령어를 통해 검색이 가능하다

```
docker search centos
```

<br>

원하는 이미지를 찾았다면 Image를 아래의 명령어를 통해 다운받으면 된다.

```
docker pull centos:7.5
```

<hr>

-- 작업 중 --
