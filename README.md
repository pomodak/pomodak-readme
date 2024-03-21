<h1 align= "center">🐥 뽀모닭: 뽀모도로 타이머</h1>

<p align="center" width="100%">
<img src="https://d2quahb2ygxiv.cloudfront.net/c6b6dc92b5b1ca2b81459.png" alt="main_1 img" width="30%"/>
<img src="./images/screenshot/1.png" alt="main_1 img" width="30%"/>
<img src="https://d2quahb2ygxiv.cloudfront.net/6b6dc92b5b1ca2b81459a.png" alt="main_1 img" width="30%" />
</p>

<br>

- 서비스 URL : https://pomodak.com
- 플레이 스토어 : 비공개 테스트 심사중(2024.03.21 ~)

<br><br>

# 프로젝트 소개


### 💡뽀모도로 / 포커스 / 집중 타이머 + 귀여운 캐릭터 수집

<br>

### 뽀모도로 기법이란?
타이머를 이용해 25분간 집중한 후 5분 휴식하는 시간 관리 방법

<br>

### 뽀모닭의 다양한 기능

1. 타이머 기능 선택
   - 0부터 시작하는 '기본 타이머'와 집중력을 높일 수 있는 '뽀모도로 타이머'
   - 원하는 모드를 선택하여 나의 시간에 집중해보세요 


2. 나의 기록 되돌아 보기
   - 스터디 기록을 시간과 색깔 스트릭으로 확인할 수 있어요
   

3. 동료가 필요할 땐 함께 공부하기
   - 함께 공부하기 모드를 통하여 **최대 9명의 동료가 함께 스터디**를 할 수 있어요
   - 다른 동료의 스터디 시간으로 보며 동기부여 UP!
   

4. 학습 후엔 캐릭터 보상
   - 공부에 재미와 동기부여를 더해줄 캐릭터 보상!
   - 일정 공부 시간이 지나면 뽀모닭의 **다양한 닭 캐릭터를 수집**할 수 있어요

<br><br>

# 팀원 구성


<div align="center">

|                                              **이창우** [📧](mailto:lcwoo3145@gmail.com)                                               |                                              **이지선** [📧](mailto:bhd1171@naver.com)                                               |                                               **노혜지** [📧](mailto:shgpwl509@naver.com)                                               |
|:-----------------------------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------:|
| [<img src="https://avatars.githubusercontent.com/u/100907484?v=4" height=150 width=150> <br/> @woo3145](https://github.com/woo3145) | [<img src="https://avatars.githubusercontent.com/u/149784847?v=4" height=150 width=150> <br/> @js1171](https://github.com/js1171) | [<img src="https://avatars.githubusercontent.com/u/86008693?v=4" height=150 width=150> <br/> @HyeJiRho](https://github.com/HyeJiRoh) |
|                                                           FE / BE (Nest)                                                            |                                                            BE (Spring)                                                            |                                                             BE (Spring)                                                              |

</div>

<br><br>

# 🎨 UI/UX


[디자인 변화 과정](https://woo3145.com/blog/pomodak-dev-story-1) 포스팅

<br><br>

# 🛠 Tech & Architecture


#### 전체 구성
![기술스택](./images/architecture.png)

<br>

### [FE](https://github.com/pomodak/pomodak)

- `React`(18.2.x), `tailwind`, `zustand`, `react-query`
- Infrastructure: `axios`, `firebase(fcm)`
- CI/CD: `vercel`
- Build: `vite`, `vite-plugin-pwa`, `pwa-builder`

### [BE (Nest)](https://github.com/pomodak/pomodak-nest)

- `Nest`(10.0.x)
- Infrastructure: `axios`, `redis`(elastiCache),`mysql8.0(aws-rds)`(dev, prod), `firebase-admin`, `nodemailer`
- CI/CD: `ec2`, `docker`, `docker-compose`, `github-actions`, `git-runner`

### [BE (Spring)](https://github.com/pomodak/pomodak-spring)

- `Spring boot`(3.2.x)
- Infrastructure: `mysql8.0(aws-rds)`(dev, prod)
- CI/CD: `ec2`, `docker`, `docker-compose`, `github-actions`, `scp`

<br><br>

# 🎨 ERD


![erd](./images/erd.png)

<br><br>

# 📅 기간


- **개발(1.0.0) :** 2024/1/10 ~ 3/18
- **플레이 스토어 비공개 테스트 :** 2024/3/18 ~ 진행중

<br><br>

# 🔍프로젝트 정보


뽀모닭 서비스는 **앱 출시 및 실서비스**를 목적으로 제작된 프로젝트입니다.  
실서비스를 하기 위해 `아이디어, 재미, 안정성`이 가장 중요하다고 판단하였습니다. <br><br>

1. 아래와 같은 이유로 초기에 CI/CD를 구축하여 애자일 방법론을 통해 개발을 진행
   - node 풀스택 1 + spring 2로 구성된 소규모 팀
   - 여러 재미있는 아이디어를 시험하고 테스트하기 위해
   - 사용자의 입장에서 빠르게 테스트해보고 재미있는지 판단하기 위해
   - `PWA(Progressive Web App)`이지만 완전한 네이티브 앱처럼 동작하기 위해
   - 불편을 느낄 수 있는 버그에 빠르게 대응하기 위해
   

2. 팀원의 기술 스택을 고려하여 아래와 같이 역할을 분리
   - `react` : 빠르게 개발하고 SPA로 네이티브 앱과 가장 비슷하게 동작
   - `nest` : 타이머, 실시간 통신 및 fcm을 처리
   - `spring` : 캐릭터와 뽑기 등의 컨텐츠를 제공하고 관리 


3. 컨텐츠 제작
   - 모든 컨텐츠 이미지는 AI와 각종 툴, 그림판으로 제작


4. 계획
   - 현재 테스트 기간이라 꾸준한 버전업을 통해 앱을 개선
   - 안정적인 운영을 위해 로깅과 모니터링 시스템을 구축하고 있음

<br><br>

# 프로젝트 특징 및 기능


### 주요 구현 기능

<details>
<summary>인증</summary>

<br/>

[자세한 내용 + 플로우 차트](/docs/authentication.md)

- 회원가입 (메일링)

   - 이메일 입력 후, 메일로 전송된 인증 코드 입력
![emailJoin](./images/auth/join-email.png)

- 로그인 
   - 상단 Email, PW 입력 후 로그인
![emailLogin](./images/auth/login-email.png)

- PW 찾기 (메일링)

   - 이메일 입력 후, 메일로 전송된 인증 코드 입력
   - 변경할 비밀 번호 입력

![findPw](./images/auth/findpw.png)


- OAuth 회원가입, 로그인

   - 각 서비스 oauth 제공자를 통해 로그인&가입

![oauth](./images/auth/login-oauth.png)

</details>

<details>
<summary>타이머 & 푸시 알림</summary>

<br/>

[자세한 내용 + 플로우 차트](/docs/timer.md)

- 일반 타이머

![normal timer]()

- 뽀모도로 타이머

![pomodoro timer]()

</details>

<details>
<summary>아이템 구매, 캐릭터 판매</summary>

</details>

<details>
<summary>캐릭터/스트릭 팔레트 뽑기</summary>

</details>

<details>
<summary>함께 공부하기</summary>

</details>

<details>
<summary>캘린더/스트릭 통계</summary>

</details>

#### 페이지

# ⚙팀 운영


|    노션    |    Jira    |    Git     |
| :--------: | :--------: | :--------: |
| ![image]() | ![image]() | ![image]() |
|   내용1    |   내용2    |   내용3    |

<br><br>

# ✒ 프로젝트 회고


### 이창우

> 회고

### 이지선

> 회고

### 노혜지

> 회고
