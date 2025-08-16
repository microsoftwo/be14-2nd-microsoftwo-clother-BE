# 👕 Clother

### 의류부터 헤어, 메이크업까지 다양한 스타일 정보를 한곳에서! 통합 스타일링 서비스: Clother 👚

<img src="https://github.com/user-attachments/assets/8e8c7919-f4dd-45b0-9c94-faab9ea0231a">

<br><br><br>


---

# 📋 목차

<a href="#1">📁 1. 프로젝트 소개</a>

<a href="#2">🔎 2. DDD (Domain-Driven Design) </a>

<a href="#3">⚙️ 3. 프로젝트 설계 </a>

<a href="#4">🎮 4. 테스트 결과 </a>

<a href="#5">✍🏻 5. 문서 </a>

<a href="#6">🛠 6. 기술 스택 </a>

<a href="#7">🫡 7. 동료평가</a>

<br><br><br>

---

# <p id="1">📁 1. 프로젝트 소개</p>

### 1-1. 프로젝트 기획 배경

#### 1. 스타일 정보를 한 번에 얻기 힘들다.
> 🛍 쇼핑 앱은 대부분 의류 정보만 제공 <br>
💇‍♀️ 헤어, 메이크업 정보는 따로 검색해야 함 <br>
💬 마음에 드는 스타일이 있어도 댓글로 물어보거나, 다시 검색해야 하는 번거로움

#### 2. 기존 스타일 공유 서비스의 한계
> 온더룩: 의류 중심 코디만 제공 <br>
룩업: 남성 위주의 스타일 <br>
인스타그램: 정보가 흩어져 있고, 체계적인 탐색 어려움

### 🌟 그래서 만든 ‘Clother’
‘Clother’는 스타일 정보를 한눈에 확인할 수 있는 통합 스타일 공유 플랫폼입니다.
> 📷 스타일 사진 하나로 의류 브랜드, 헤어샵, 메이크업 제품까지 모두 확인 가능 <br>
👗 같은 아이템으로 다양한 스타일링 사례 확인 <br>
💁🏻‍♀️ 팔로우한 유저의 스타일 변화, 방문한 헤어샵 정보도 함께 확인

### 💡 Clother가 제공하는 경험
단순한 코디 공유를 넘어서, 전체 스타일링을 손쉽게 탐색하고
자신만의 스타일을 만들 수 있는 공간을 제공합니다.

<br>

### 1-2. 프로젝트 주요 기능
<img width="1006" height="458" alt="image" src="https://github.com/user-attachments/assets/dc0e86b2-a61b-4265-802c-99564ed3d48d" />

<img src = "https://github.com/user-attachments/assets/17495b98-d25a-4a48-af5b-3119b567dcf8">

<img src="https://github.com/user-attachments/assets/d7f8324d-d6df-493b-9dfa-0e1a10f3ad1d">

<img src="https://github.com/user-attachments/assets/28caa8f5-c9e0-44b3-b21c-097a86e4cc50">

### 주요 기능

- 코디뿐만 아니라 헤어, 메이크업, 악세서리까지의 스타일링을 공유할 수 있는 SNS.

- 사용자는 자신이 원하는 스타일의 포스팅을 선택하고, 포스팅에 달린 태그를 통해 제품 정보 알 수 있고, 구매링크를 통해 바로 구매 혹은 예약처까지 연결될 수 있다.

- 포스팅 시에는 링크, 등록된 상품 등을 태그로 사용할 수 있고 원하는 상품이 없을 시 상품 등록 신청이 가능하다.

- 스타일쉐어 게시판을 통해 자신의 스타일링에 대한 피드백을 받을 수 있다.

<br><br>

---

# <p id="2">🔎 2. DDD (Domain-Driven Design)</p>

### <p id="2-1">2-1. DDD (Event-Storming)</p>

![KakaoTalk_Photo_2025-03-26-17-32-12](https://github.com/user-attachments/assets/11540776-bc6f-41bd-bc50-08364ce95aaa)

### <p id="2-2">2-2. DDD (Context-Map) </p>

![마이크로소프투-2](https://github.com/user-attachments/assets/171a896c-2645-4830-8e8b-283c8d3a420b)

<br><br>

---

# <p id="3">⚙️ 3. 프로젝트 설계</p>

### <p id="3-1">3-1. 물리 모델링 (ERD)</p>

<img width="949" alt="스크린샷 2025-03-26 15 32 07" src="https://github.com/user-attachments/assets/49a73250-0d5b-4b0f-a478-e53562cf5938" />

### <p id="3-2">3-2. MSA 아키텍쳐 </p>

![image](https://github.com/user-attachments/assets/21b8d5d9-acf6-44f7-8cba-ba36a588056a)
![msa](https://github.com/user-attachments/assets/b67bf7bd-a623-4db1-ba1f-ddb13413db21)

<br>

### <p id="3-3">3-3. 📚 API 명세서 </p>

<details>
    <summary>user-service</summary>
    <div markdown="1">
      <img width="1400" alt="image" src=https://github.com/user-attachments/assets/df5c035d-0402-4e1a-88f2-dfee258b3629>
    </div>
</details>

<details>
    <summary>core-service</summary>
    <div markdown="1">
      <img width="1400" alt="image" src=https://github.com/user-attachments/assets/423c352f-a830-4b8e-8c52-c29c21ff2390>
    </div>
</details>

<br>

### <p id="3-4">3-4. 🧱 Redis를 활용한 이메일 인증 </p>

회원가입 시 이메일로 전송되는 인증 코드는 일정 시간이 지나면 자동으로 무효화되어야 하며, 서버에 불필요한 데이터가 남지 않아야 한다.

따라서 Redis의 TTL(Time To Live) 기능을 사용하여 인증 번호를 저장하고, 5분이 지나면 자동으로 만료되도록 구성하였다.

<br>

<details>
    <summary>📥 1) 인증 절차</summary>
    <div markdown="1">
      <br>
        1. 사용자가 이메일 입력 후 인증 요청<br>
        2. 서버에서 6자리 인증 코드 생성<br>
        3. Redis에 인증 코드 저장 (TTL: 5분)<br>
        4. 사용자 이메일로 인증번호 발송 (SMTP 사용)<br>
        5. 사용자가 인증번호를 입력하여 검증 요청<br>
        6. Redis에서 이메일 키로 인증번호 조회<br>
        7. 인증 성공 또는 실패 판단
    </div>
</details>

<details>
    <summary>🕑 2) TTL 적용 구조 설명</summary>
    <div markdown="1">
<br> 
      
1) 인증 코드의 유효 시간 설정

```java
spring:
  mail:
    auth-code-expiration-millis: 300000  # 5분
```

<br>

2. 이메일 인증번호를 Redis에 저장할 때 TTL로 설정

```java
@Value("${spring.mail.auth-code-expiration-millis}")
private long authCodeExpirationMillis;
```

<br>

3. RedisUtil 클래스 내 TTL 적용 메서드

```java
public void setDataExpire(String key, String value,
                              long duration) {
        ValueOperations<String, String> valueOperations = redisTemplate.opsForValue();
        Duration expireDuration = Duration.ofMinutes(duration);
        valueOperations.set(key, value, expireDuration);
    }
```

이 TTL(Time To Live)이 적용된 키는 해당 시간 이후 자동으로 만료되고 삭제된다.

</div>

</details>

<details>
    <summary>👍🏻 3) TTL 사용 후 효과</summary>
    <div markdown="1">
        <br>1. 설정된 TTL이 지나면 인증번호는 자동 삭제되어, 불필요한 데이터 제거 가능. <br>
        2. 인증번호는 일시적 데이터이므로, 디스크 기반 RDB 대신 인메모리 Redis에서 빠르게 처리 가능.
    </div>
</details>

<details>
    <summary>☄️ 4) Redis 이용 트러블 슈팅 </summary>
    <div markdown="1">
    <br>
      <img width="1180" alt="image" src="https://github.com/user-attachments/assets/963ad2b7-1c8e-43bf-993a-7ba8f8ed0e4b" />

<br>

#### 🔑 이메일을 Key로, 인증 코드를 Value로 둔 이유

📌 1. 이메일은 유일한 식별자이기 때문

- 회원가입 또는 인증 과정에서 이메일은 사용자를 유일하게 식별할 수 있는 정보이다.
- Redis는 Key-Value 구조이기 때문에, 유일한 값을 key로 사용해야 나중에 덮어쓰거나 충돌이 나지 않음.
- 그래서 이메일 → 인증코드 구조로 저장하면, 같은 사람이 다시 인증 요청을 할 때 기존 인증 코드를 덮어쓰기도 쉽고, 빠르게 조회할 수 있다.

📌 2. Value인 인증 코드는 자주 바뀜

- 인증 코드는 6자리 숫자이고 5분이 지나면 사라진다.
- 따라서 Redis의 TTL(Time-To-Live) 기능을 써서 저장해두고 일정 시간 후 삭제되도록 관리하였다.
</div>
</details>

<br><br>

---

# <p id="4">🎮 4. 단위 테스트</p>

### <p id="4-1">4-1. 단위 테스트 결과 </p>

<details>
    <summary>테스트 결과 확인하기</summary>
    <div markdown="1">  
      <img width="1141" alt="댓글생성" src=https://github.com/user-attachments/assets/33e71cb6-d3e1-4574-bf55-d81c0259d1c0 />
      <img width="1141" alt="특정게시글조회" src=https://github.com/user-attachments/assets/b8319b3f-641c-4500-bd28-2c4cc1c960d2 />
      <img width="1141" alt="피드조회" src=https://github.com/user-attachments/assets/c812d542-6af2-458a-82ab-84f18144d06e />
      <img width="1141" alt="하위카테고리검색" src=https://github.com/user-attachments/assets/8404292e-7a5f-4d13-9568-605663d1c7f5 />
      <img width="1141" alt="회원가입" src="https://github.com/user-attachments/assets/38f07e02-c7d1-434a-bcbd-21f706de7acc" />
    </div>
</details>

### <p id="4-2">4-2. API 테스트 </p>

<details>
    <summary>테스트 결과 확인하기</summary>
    <div markdown="1">
    <details>
         <summary>회원 도메인 테스트 결과 확인하기</summary>
                    <summary>인증 번호 전송</summary>
                          <img width="1400" alt="image" src=https://github.com/user-attachments/assets/ef8f8efc-fd62-4958-9439-c38b88db12e5>
                    <summary>인증 번호 검증</summary>
                          <img width="1400" alt="image" src=https://github.com/user-attachments/assets/e078de72-5973-4408-8339-dcad4411c783>
                    <summary>회원 가입</summary>
                          <img width="1400" alt="image" src=https://github.com/user-attachments/assets/210f01ac-43fa-4282-8811-ba2567023ddb>
                    <summary>로그인</summary>
                          <img width="1400" alt="image" src=https://github.com/user-attachments/assets/2838e7e3-78ab-4e3b-94a6-a02f1d097d75>
                    <summary>토큰 미포함 요청</summary>
                          <img width="1400" alt="image" src=https://github.com/user-attachments/assets/a52c71c7-1b9f-4fad-9180-9ae1a060673c>
                    <summary>토큰 포함 요청</summary>
                          <img width="1400" alt="image" src=https://github.com/user-attachments/assets/004bac3a-2bfa-400f-83a4-54af53b04170>
    </details>
     <details>
        <summary>포스팅 도메인 테스트 결과 확인하기</summary>
                    <summary>포스팅 등록</summary>
                          <img width="1400" alt="image" src=https://github.com/user-attachments/assets/7a066c54-2de6-44cc-acbb-05cf9615edd4>
                    <summary>포스팅 조회</summary>
                          <img width="1400" alt="image" src=https://github.com/user-attachments/assets/714f467a-1507-40bf-8d9d-5c1bf310ad98>
     </details>
      <details>
          <summary>훈수 게시판 도메인 테스트 결과 확인하기</summary>
                    <details>
                      <summary>훈수 게시물 등록</summary>
                      <img width="1400" alt="게시물 등록" src="https://github.com/user-attachments/assets/0c9b2556-6ddb-4157-91db-82364666bb05">
                    </details>
                    <details>  
                      <summary>훈수 게시물 수정</summary>
                            <img width="1400" alt="게시물 수정" src="https://github.com/user-attachments/assets/d4e308a0-ced9-4c55-b038-a740545bf679">
                    </details>
                    <details>
                    <summary>훈수 게시물 삭제</summary>
                          <img width="1400" alt="게시물 삭제" src="https://github.com/user-attachments/assets/a465a856-ac17-40c9-855c-71b2b7f0135e" >
                    </details>
                    <details>
                    <summary>훈수 게시판 최신순(기본)조회 - 사용자</summary>
                          <img width="1400" alt="게시판 최신순 조회" src="https://github.com/user-attachments/assets/84757fed-da97-464e-b8f2-a636a58f962a" />
                    </details>
                    <details>
                    <summary>훈수 게시판 좋아요순 조회 - 사용자</summary>
                          <img width="1400" alt="게시판 좋아요순 조회" src="https://github.com/user-attachments/assets/b03d2d95-b1a1-4e6a-a1f3-74dd8a520e97" />
                    </details>
                    <details>
                    <summary>훈수 게시판 키워드별 조회 - 사용자</summary>
                          <img width="1400" alt="키워드별 조회" src="https://github.com/user-attachments/assets/16c564d6-b8ab-4449-be9f-8414fc627e9a" />
                    </details>
     </details>
      <details>
          <summary>상품 도메인 테스트 결과 확인하기</summary>
                  <summary>상품 등록 신청
                          <img width="1400" alt="image" src=https://github.com/user-attachments/assets/44a37510-ca7f-41bd-9ca4-085fe1953816>
                  </summary>
                  <summary>상품 등록 신청 삭제
                          <img width="1400" alt="image" src=https://github.com/user-attachments/assets/ac9a3915-6395-48c8-9555-b637092da3b7>
                  </summary>
                 <summary>상품 등록 신청 수정
                          <img width="1400" alt="image" src="https://github.com/user-attachments/assets/19b7f83c-ca08-4545-b07d-933c043e393b">
                  </summary>
                  <summary>상품 등록 신청 목록 조회
                          <img width="999" src="https://github.com/user-attachments/assets/9221f6d6-39ce-4010-ad8d-f262e7250092" />
                  </summary> 
                  <summary>카테고리별 상품 목록 조회
                        <img width="990" src="https://github.com/user-attachments/assets/1463d44a-8d39-49a5-afdc-df0573e50bc4" />
                  </summary>
                   <summary>하위 카테고리 목록 조회
                         <img width="989" src="https://github.com/user-attachments/assets/a1a3298d-ae03-4cb3-ae14-2770aceb8dfb" />
                  </summary> 
                  <summary>상품 상세 페이지 조회
                          <img width="1007" src="https://github.com/user-attachments/assets/bbe14ffa-fe17-4cc3-91b7-e3a7645572db" />
                  </summary> 
     </details>
       <details>    
          <summary>좋아요 도메인 테스트 결과 확인하기</summary>
                  <summary>좋아요 등록
                          <img width="1400" alt="image" src=https://github.com/user-attachments/assets/a9c5438e-d2d2-4bcb-9b47-9ab3f0fe34f0>
                  </summary>
                  <summary>좋아요 취소
                          <img width="1400" alt="image" src=https://github.com/user-attachments/assets/8a4fe730-8c62-44af-9442-aa0f8f9fdd57>
                  </summary>
                  <summary>회원 좋아요 내역 조회
                          <img width="1400" alt="image" src=https://github.com/user-attachments/assets/cebae2c7-8e18-426e-a8c5-75cbdaad8b9e>
                  </summary>
                  <summary>좋아요 여부 조회
                          <img width="1400" alt="image" src=https://github.com/user-attachments/assets/077e600a-22c8-4427-9e0f-af910739473b>
                  </summary>
     </details>
      <details>
        <summary>댓글 도메인 테스트 결과 확인하기</summary>
                  <summary>댓글 등록
                        <img width="1400" alt="image" src=https://github.com/user-attachments/assets/083b74fe-5565-4fc2-a2c8-c819c0d24bf3>
                  </summary>
                  <summary>댓글 삭제
                        <img width="1400" alt="image" src=https://github.com/user-attachments/assets/dd8168cd-13e4-4fb5-b04a-6977b943be96>
                  </summary>
                  <summary>댓글 조회
                        <img width="1400" alt="image" src=https://github.com/user-attachments/assets/82ae05d4-c5e4-4449-afae-a5c6faf802a9>
                  </summary>
      </details>
    </div>

</details>
<br><br>

---

# <p id="5">✍🏻 5. 문서 </p>

### <p id="5-1">5-1. 📙 요구사항 명세서 </p>

[[🔗요구사항 명세서 Link]](https://docs.google.com/spreadsheets/d/1HQYulWkDctMpm4mhM3wYKbtAY3fCOOigEeM-M-q0jlg/edit?gid=269659385#gid=269659385)
<br>

<img width="783" alt="image" src="https://github.com/user-attachments/assets/96815989-ef5b-4b72-a3cb-ea1563a0188b" />

### <p id="5-2">5-2. 🗓️ WBS (Work Breakdown Structure) </p>

[[🔗 WBS Link]](https://docs.google.com/spreadsheets/d/1HQYulWkDctMpm4mhM3wYKbtAY3fCOOigEeM-M-q0jlg/edit?gid=393359725#gid=393359725)

<img width="1291" alt="image" src="https://github.com/user-attachments/assets/d46f9ea3-64a6-4529-a3e5-dee22989bd26" />

<br><br>

### <p id="5-3">5-3. 📡 와이어프레임 </p>

<details>
    <summary>로그인 화면</summary>

####  로그인 화면 
<img src = "https://github.com/user-attachments/assets/5a6b0043-0e99-47bd-a65a-41b8eba2aba4">
</details>

<details>
    <summary> 포스팅 등록 화면 </summary>
    
####  포스팅 등록 화면
<img src = "https://github.com/user-attachments/assets/8db5e0ec-d20d-4ce6-b3c2-dd3488cb6ac5">
</details>

<details>

<summary> 마이페이지 화면 </summary>

#### 마이페이지 화면

<img src = "https://github.com/user-attachments/assets/60713110-f894-4282-8f37-43186ac94390">
    
</details>

<details>

<summary> 카테고리 별 포스팅 화면 </summary>

#### LOOK 카테고리 선택 시 화면

<img src = "https://github.com/user-attachments/assets/3a45410c-770a-46db-af1b-eb9176cb2dac">


#### MAKEUP 카테고리 선택 시 화면 

<img src = "https://github.com/user-attachments/assets/3fd7271b-cccb-4ee4-a536-2ff9903ad6f0">


#### HAIR 카테고리 선택 시 화면 

<img src = "https://github.com/user-attachments/assets/f0865880-25c9-43c7-a9cf-b2a80c84213a">
  
</details>

<details>

<summary> 스타일 쉐어 게시판 화면 </summary>

#### 스타일 쉐어 게시판 화면

<img src = "https://github.com/user-attachments/assets/8272d581-af3c-4d87-9c04-a489533f15af">

</details>

<details> 
    
<summary> 포스팅 상세 화면 </summary>

#### 포스팅 상세 화면

<img src = "https://github.com/user-attachments/assets/18ea81ca-669f-40a4-8f44-a08e5ce40053">

</details>



<br><br>

### <p id="5-4">5-4. 👀 스토리보드 </p>

<details>
    <summary>랜딩 화면</summary>
  
  #### 랜딩 화면
<img width="1150" alt="스크린샷 2025-04-19 22 19 40" src="https://github.com/user-attachments/assets/d6b9defb-9893-40b9-b1a3-ded0585fe556" />

</details>

<details>
  <summary>회원가입</summary>

  #### 회원가입 화면
  <img width="1150" alt="스크린샷 2025-04-16 07 45 10" src="https://github.com/user-attachments/assets/2557597b-f386-492f-aca0-44c384a8f13b" >


  #### 회원가입 성공 화면
  <img width="1150" alt="스크린샷 2025-04-19 21 56 40" src="https://github.com/user-attachments/assets/7e9e7bf7-2cae-4c88-890d-6adfb7458667" />
</details>

<details>
  <summary>로그인</summary>
  
  #### 로그인 화면
<img width="1150" alt="스크린샷 2025-04-19 22 21 12" src="https://github.com/user-attachments/assets/2ed2f059-6230-456e-b6c6-54e01dd98718" />

  #### 로그인 실패 화면
  <img width="1151" alt="스크린샷 2025-04-19 21 57 56" src="https://github.com/user-attachments/assets/e7d6e588-e83a-4481-a168-557797b07a66" />

</details>

<details>
  <summary>포스팅</summary>
  
  #### 메인페이지 화면
<img width="1150" alt="스크린샷 2025-04-19 22 07 57" src="https://github.com/user-attachments/assets/3e0738ee-8d7a-4840-b9d6-18084f1090a3" />

  #### 포스팅 조회 화면
<img width="1150" alt="스크린샷 2025-04-19 22 10 05" src="https://github.com/user-attachments/assets/59c0889a-9d4c-45db-a40d-28ddbfaf388e" />


  #### 포스팅 등록 화면
<img width="1149" alt="스크린샷 2025-04-19 22 10 43" src="https://github.com/user-attachments/assets/0c53812c-3a11-4919-8402-d24473c15f00" />

</details>

<details>
  <summary>스타일 쉐어</summary>
  
  #### 스타일 쉐어 게시판 화면
<img width="1146" alt="스크린샷 2025-04-19 22 04 16" src="https://github.com/user-attachments/assets/454eae00-12f5-4698-93f7-b0eec96d2a20" />

  #### 스타일 쉐어 게시물 화면
<img width="1145" alt="스크린샷 2025-04-19 22 05 47" src="https://github.com/user-attachments/assets/9a8eca29-4ee4-44f3-88bb-02873c9c0975" />


  #### 스타일 쉐어 게시물 댓글 화면
<img width="1147" alt="스크린샷 2025-04-19 22 07 02" src="https://github.com/user-attachments/assets/cde7f7dd-d594-4fb8-be27-f8832acee1e4" />


  #### 스타일 쉐어 게시물 등록 화면
<img width="1146" alt="스크린샷 2025-04-19 22 22 40" src="https://github.com/user-attachments/assets/ffec02ca-3129-4f84-9751-1ee5e3711bef" />


</details>


<details>
  <summary>마이페이지</summary>
  
  #### 마이페이지 화면
<img width="1152" alt="스크린샷 2025-04-19 22 00 18" src="https://github.com/user-attachments/assets/ec8e04af-46bf-4eba-be47-ac00e8372cf9" />

  #### 회원정보 수정 화면
<img width="1149" alt="스크린샷 2025-04-19 22 01 10" src="https://github.com/user-attachments/assets/dd910f46-2ccf-4ec7-870e-0dc97d62dadb" />

  #### 회원정보 수정 성공 화면
<img width="1150" alt="스크린샷 2025-04-19 22 01 27" src="https://github.com/user-attachments/assets/80fe1850-2a3e-4d5b-a7ac-a21af59681f2" />

  #### 나의 활동 기록
<img width="1147" alt="스크린샷 2025-04-19 22 02 39" src="https://github.com/user-attachments/assets/c8ffa48a-48ed-41ae-bd53-44e3dc6e2930" />

  #### 로그아웃
<img width="1150" alt="스크린샷 2025-04-19 22 24 01" src="https://github.com/user-attachments/assets/a1440732-fe53-4db6-b6ac-5f857129f3e4" />

</details>

<details>
  <summary>공통 레이아웃</summary>
  
  #### 헤더
<img width="1150" alt="스크린샷 2025-04-19 22 16 09" src="https://github.com/user-attachments/assets/5816c181-b548-4e0c-ae50-58fd4cb6e31a" />

  #### 푸터
<img width="1150" alt="스크린샷 2025-04-19 22 16 30" src="https://github.com/user-attachments/assets/9e496558-c5e5-4546-a992-91be6914d73c" />

</details>



<br><br>

### <p id="5-5">5-5. 📌 테스트 결과 보고서 </p>

테스트 결과에 대한 자세한 내용과 시연 영상은 아래 노션 링크에서 확인하실 수 있습니다.  

[[🔗테스트 결과 보고서 Link]](https://ohgiraffers.notion.site/1d6649136c11805c884cd7559d1ab25b?pvs=4)

<br><br>

---

# <p id="6">🛠 6. 기술 스택 </p>

### 언어

![Java](https://img.shields.io/badge/Java-007396?style=plastic&logo=java&logoColor=white)

### 프레임워크

![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=plastic&logo=spring&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=plastic&logo=spring-boot&logoColor=white)
![Spring JPA](https://img.shields.io/badge/JPA-6DB33F?style=plastic&logo=spring&logoColor=white)
![Hibernate](https://img.shields.io/badge/Hibernate-59666C?style=plastic&logo=hibernate&logoColor=white)
![MyBatis](https://img.shields.io/badge/MyBatis-B5E7A0?style=plastic&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=plastic&logo=spring-security&logoColor=white)

### 라이브러리

![JWT](https://img.shields.io/badge/JWT-000000?style=plastic&logo=json-web-tokens&logoColor=white)

### 도구

- 에디터
  
  ![IntelliJ IDEA](https://img.shields.io/badge/IntelliJ-000000?style=plastic&logo=intellij-idea&logoColor=white)
- 빌드
  
  ![Gradle](https://img.shields.io/badge/Gradle-02303A.svg?style=plastic&logo=Gradle&logoColor=white)

### 데이터베이스

![MariaDB](https://img.shields.io/badge/MariaDB-003545?style=plastic&logo=mariadb&logoColor=white)

### 명세

![Postman](https://img.shields.io/badge/Postman-FF6C37?style=plastic&logo=postman&logoColor=white)
![Swagger](https://img.shields.io/badge/-Swagger-%23Clojure?style=plastic&logo=swagger&logoColor=white)

### ETC

### 버전 관리

![Git](https://img.shields.io/badge/git-%23F05033.svg?style=plastic&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=plastic&logo=github&logoColor=white)

### 소통

![Notion](https://img.shields.io/badge/Notion-%23000000.svg?style=plastic&logo=notion&logoColor=white)

<br><br>

---
# 🚀 Team microsoftwo

| <img src="https://github.com/user-attachments/assets/9e5c3e83-7f0d-41ca-816c-8133409537e1" width="200"> | <img src="https://github.com/user-attachments/assets/8f52dde1-3590-4e2f-880d-32098f5d098a" width="200"> | <img src="https://github.com/user-attachments/assets/0b56df7f-c48d-4975-abff-aeb51af8f2da" width="200"> | <img src="https://github.com/user-attachments/assets/f5cbf6cc-ff54-4720-be15-390182415083" width="200"> | <img src="https://github.com/user-attachments/assets/1d2619c6-f467-485e-9d90-14c7c43bc316" width="200"> |
| :-----------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------: |
|                                                 김기종                                                  |                                                 조윤태                                                  |                                                 신민경                                                  |                                                 황수민                                                  |                                                 이예원                                                  |
| [<img src="https://img.shields.io/badge/Github-Link-181717?logo=Github">](https://github.com/rrangeess) |  [<img src="https://img.shields.io/badge/Github-Link-181717?logo=Github">](https://github.com/cxzaqq)   |  [<img src="https://img.shields.io/badge/Github-Link-181717?logo=Github">](https://github.com/mmmv41)   | [<img src="https://img.shields.io/badge/Github-Link-181717?logo=Github">](https://github.com/emily9949) |  [<img src="https://img.shields.io/badge/Github-Link-181717?logo=Github">](https://github.com/oni128)   |

<br><br>

# <p id="7">🫡 7. 동료평가 </p>

<details>
<summary>동료 평가 확인하기</summary>
<div markdown="1">

#### ABOUT [김기종](https://github.com/rrangeess)

|  FROM  | COMMENT                                                                                                                                                                                                                                                                                                              |
| :----: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 조윤태 | 묵묵히 자신의 역할을 수행하며 책임감 있게 맡은 부분을 구현해내는 모습이 인상적이었습니다. 모르는 부분이 있을 때도 혼자 해결하고 넘어가는 것이 아니라, 적극적으로 의견을 공유하며 더 나은 방향을 고민하는 태도가 돋보였습니다. 이러한 자세는 좋은 개발자가 갖춰야 할 중요한 자질이며, 팀원들에게도 귀감이 되었습니다. |
| 신민경 | 프로젝트를 진행하면서 끈기 있게 끝까지 해내는 모습을 보며 정말 인상 깊었습니다. 새로운 아이디어가 필요할 때마다 적극적으로 의견을 내주었고, 특히 진행 중 예상치 못한 상황이 생겼을 때도 빠르게 해결책을 고민하며 방향을 제시해 준 덕분에 프로젝트가 더 탄탄해질 수 있었습니다. 또한, 팀원들의 의견을 잘 듣고 피드백을 주고받으며 함께 성장하려는 모습이 인상적이었어요. 덕분에 더 나은 결과물을 만들어낼 수 있었습니다. 무엇보다 발표 직전까지도 최선을 다해 마무리 작업을 챙기는 모습이 정말 멋졌습니다.|
| 황수민 | 먼 거리에도 불구하고 대면 회의에 적극적으로 참여하려는 노력에 감탄했습니다. 체력적으로 힘들었을 텐데도 밝은 태도로 분위기를 이끌어주신 덕분에 팀원들 모두 끝까지 집중할 수 있었습니다. 특히, 발표 직전까지도 더 나은 발표를 위해 고민하고 구성해주신 덕분에, 더욱 짜임새 있는 발표 자료를 완성할 수 있었습니다. 또한, 팀원들 간의 이해도가 다를 때 기종님께서 개념을 명확하게 정리해주신 덕분에 모호한 부분을 확실히 짚고 넘어갈 수 있었습니다. 개발 과정에서도 맡은 역할을 철저히 수행해주셔서 프로젝트에 큰 도움이 되었습니다! |
| 이예원 | 맡은 업무의 다양한 기능을 묵묵히 끝까지 책임감 있게 수행하는 모습이 인상 깊었습니다. 그 덕분에  완벽한 테스트코드가 나온 것 같아요 ! 하기 싫은 일이나 어려운 일이 생겼을 때 먼저 나서서 시도해보려는 적극적인 태도도 팀에 큰 도움이 되었고 회의 중간중간 핵심 내용을 정리해줌으로써 팀원들의 이해를 돕는 모습도 굉장히 도움이 되었던 것 같아요 무엇보다 집이 가장 먼 상황에서도 매번 직접 만나 회의에 참여해주시고, 늦게까지 남아 함께 하는 모습에 정말 감사했어요. 그런 책임감 있는 태도 덕분에 팀워크가 더 단단해질 수 있었던 것 같아요 / |

#### ABOUT [조윤태](https://github.com/cxzaqq)

|  FROM  | COMMENT                                                                                                                                                                                                                                                                                                          |
| :----: | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 김기종 | 저희 팀에 없어서는 안 될 브레인으로서 프로젝트 설계, 전체 로직 구현 등 모조리 언급 할 수 없을 정도로 보이는 곳, 안 보이는 곳에서 열심히 임해주고 잘해주셨습니다. 심지어 프로젝트 마감이 급박한 상황에서 발표까지 맡게 되셨는데 이 역할도 훌륭히 수행해 주셔서 이번 프로젝트 내내 감사했다고 말씀드리고 싶습니다. |
| 신민경 | 우리 팀의 비공식 조장님(선장님) 덕분에 어려운 순간들을 잘 극복할 수 있었습니다. DB 설계부터 개발까지 항상 깊이 고민하고 이유를 찾아가며 프로젝트에 임하시는 모습을 보며 정말 많이 배울 수 있었습니다. 특히, 백엔드 개발이 낯선 팀원들을 위해 아는 부분은 아낌없이 공유해 주시고, 막히는 부분이 있을 때마다 해결책을 제시해 주신 덕분에 개발 과정이 훨씬 수월해진 것 같아요. 또한, MSA 설계 과정에서 팀원들이 어려움을 겪고 있을 때 윤태님의 활약 덕분에 프로젝트를 잘 마무리할 수 있었습니다 감사합니다 ! |                                                                 
| 황수민 | 팀의 실질적인 리더 역할을 해주셨다고 생각합니다. 프로젝트 도중 난관에 봉착했을 때도 침착하게 해결 방안을 모색하며 더 나은 방향으로 이끌어주셨습니다. 기술적인 이해도가 뛰어나 많은 도움을 받을 수 있었고, 팀원들의 질문에도 함께 고민하며 적극적으로 문제 해결을 하려고 노력해주셨습니다. 문제가 생겼을 때 바로바로 해결방안을 도출해주신 윤태님 덕분에 프로젝트 기간 동안 팀원들도 함꼐 기술적 성장을 이루어낼 수 있었던 것 같습니다. 많은 일을 맡으셨음에도 불구하고 힘든 내색 없이 끝까지 책임감 있게 임하셨으며, 겸손한 태도를 유지하는 모습이 인상적이었습니다. 특히, 강한 책임감으로 발표까지 완성도 높게 마무리하신 점은 정말 박수쳐드리고 싶습니다! |
| 이예원 | 우리 팀의 선장님. 선장님과 함께라면 언제나 든든합니다. 특히 시간이 촉박한 상황에서도 조급해하지 않고, 차분하게 문제를 해결해나가는 태도가 인상 깊었어요. 그런 태도 덕분에 팀원들도 믿고 의지할 수 있었고, 팀 전체가 흔들림 없이 나아갈 수 있었습니다. 궁금한 점이나 질문이 생기면 바쁘신 와중에도 먼저 도와주셔서 정말 감사했고 오류가 발생했을 때 로그를 활용해 빠르게 원인을 파악하고 해결해나가는 과정을 알려주셔서 많은 것을 배울 수 있었습니다. 모르는 개념에 대해 여러 번 질문을 드려도 늘 한결같은 태도로 친절히 설명해주시고 이해할 때까지 함께 고민해주는 선장님 덕분에 더 많은 성장을 할 수 있었던 것 같습니다. 항상 감사한 마음뿐입니다 / |

#### ABOUT [신민경](https://github.com/mmmv41)

|  FROM  | COMMENT                                                                                                                                                                                                                                                                                                          |
| :----: | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 김기종 | 프로젝트 기간 동안 아이디어 수립 과정에서 적극적으로 자신의 의견을 피력하고, 다양한 아이디어를 제공해주는 모습이 인상 깊었습니다.또한 프로젝트 구현 과정에서 로그인, 회원가입 도메인을 담당하셨는데, 어려운 내용이었음에도 불구하고 성공적으로 구현해내는게 대단하다고 생각했고 감사했습니다.                    |
| 조윤태 | 가장 어려운 부분 중 하나였던 Spring Security를 적용하면서, 프로젝트의 보안성을 한층 높였습니다. 여기에 더해 Redis까지 활용하며 성능 개선에도 기여하는 등, 프로젝트를 더욱 완성도 높은 형태로 발전시키는 데 주요한 역할을 했습니다. 어려운 문제를 해결해 나가는 과정에서 팀원들에게도 긍정적인 영향을 주었습니다. |
| 황수민 | 처음 시도해보는 로그인 구현을 맡게 되면서 짧은 시간 안에 기능을 완성해야 한다는 부담이 있었을 텐데도, 시간을 쪼개가며 로그인 기능을 완벽히 구현해내신 점이 정말 인상적이었습니다. 특히, Redis를 활용한 로그인 기능을 완성함으로써 프로젝트의 완성도를 한층 높여주셨습니다. 기술적인 구현뿐만 아니라 기획 단계에서도 적극적으로 아이디어를 제시해 주셨고, 문서화 작업까지 꼼꼼하게 챙겨주셔서 정말 만능 개발자라고 느꼈습니다! 또한, 팀 분위기를 한층 밝게 만들어주셔서 덕분에 화기애애한 분위기 속에서 프로젝트를 진행할 수 있었습니다. 민경님 덕분에 팀원들의 단합력도 더욱 높아졌습니다! 프로젝트 기간 동안 많은 의지가 되었습니다 // |
| 이예원 | 이번 프로젝트에서 가장 어려운 기능 중 하나였던 회원가입 및 로그인 기능을 자진해서 맡아, 완벽하게 구현한 점이 정말 인상 깊었습니다. 단순히 동작하는 수준이 아니라, 커스텀 예외 처리까지 깔끔하게 정리하며 짧은 개발 기간 안에 높은 완성도로 마무리해주어 팀 전체의 개발 흐름이 훨씬 안정적이었던 것 같아요. 무엇보다도 지속적으로 더 나은 구조와 코드를 고민하고 개선하려는 태도가 매우 인상적이었습니다. 복잡한 요구사항 속에서도 흔들리지 않고 차근차근 문제를 해결해나가는 모습을 보며, 수행능력과 책임감 등 배울점을 많이 느꼈던 것 같아요. 덕분에 이번 프로젝트에서 의지하면서 진행했던 것 같아요/|

#### ABOUT [황수민](https://github.com/emily9949)

|  FROM  | COMMENT                                                                                                                                                                                                                                                                                                                                                              |
| :----: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 김기종 | 팀원들 간에 의견이 서로 엇갈리거나 다양하게 나오는 때에도 남의 말에 경청하고 소통하는 모습에서 배울 점이 많다고 느꼈습니다. 또한 프로젝트 내내 항상 열심히 임하는 모습이 인상 깊었습니다. 프로젝트 마감이 얼마남지 않은 상황에서 신체적으로 안 좋은 게 느껴졌음에도 불구하고 내색하지 않고 끝까지 최선을 다 해주셔서 감사했습니다.                                   |
| 조윤태 | 모르는 부분이 생기면 주저하지 않고 학습하며 해결하려는 적극적인 자세가 정말 인상적이었습니다. 특히, 게이트웨이 필터링을 구현하는 과정에서 기존 강의를 다시 찾아보며 끈질기게 해결책을 모색하는 모습이 돋보였습니다. 피곤한 상황에서도 힘든 기색 없이 끝까지 집중력을 유지하며 맡은 역할을 수행해 준 덕분에, 팀 전체가 더욱 적극적으로 프로젝트에 임할 수 있었습니다. |
| 신민경 | 맡은 역할을 끝까지 최선을 다해 해내는 모습이 인상적이었던 팀원이었습니다. 프로젝트가 진행될수록 시간이 지체되고 예상치 못한 오류가 발생하면서 집중력을 잃기 쉬운 상황에서도, 밤을 새워서라도 자신의 맡은 부분을 끝까지 책임지는 모습이 정말 멋졌습니다. 또한, 누구도 캐치하지 못했던 실수나 오류를 예리하게 발견하고 빠르게 수정할 수 있도록 도와준 덕분에 프로젝트를 원활하게 진행할 수 있었습니다. 무엇보다, 프로젝트 마무리 단계에서 발표 자료를 완벽하게 준비해주시고, 최종 점검까지 세심하게 챙겨준 덕분에 완성도를 높일 수 있었습니다 !  |                                                                              
| 이예원 | 모르는 부분이 생길 때마다 함께 고민해주고 해결 방안을 같이 찾아주는 태도가 정말 인상 깊었습니다. 덕분에 막히는 순간에도 혼자 고민하지 않아도 되어 큰 힘이 되었고, 자연스럽게 팀의 협업 분위기에도 긍정적인 영향을 준 것 같아요. GitHub 사용에 익숙하지 않아 질문을 많이 했는데 항상 친절하게 알려주고, 특히 PR 코멘트에 대해 고민할 때마다 섬세한 피드백을 통해 많은 도움을 받을 수 있었고 세심하게 짚어주는 그 과정 덕분에 저도 더 나은 방식으로 코드 리뷰를 바라보게 되었던 것 같아요. 그리고 어려운 상황 속에서도 끝까지 문제를 해결하려는 끈기 있는 자세가 인상 깊었습니다. 그러한 모습 덕분에 자극받아 더 열심히 할 수 있었어요/ |

#### ABOUT [이예원](https://github.com/oni128)

|  FROM  | COMMENT                                                                                                                                                                                                                                                                                                                                       |
| :----: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 김기종 | 육체적으로나 정신적으로나 지칠 법한 상황에도 항상 밝은 얼굴로 프로젝트에 임해주시는 모습이 인상깊었습니다. 덕분에 프로젝트 동안 큰 트러블 없이 원활히 굴러갈 수 있었다고 생각합니다. 또한 기술적인 측면에서도 도메인 기능 구현, 테스트 코드 작성들을 척척 해내시는 모습을 보고 대단하다고 느꼈고 감사했습니다.                                |
| 조윤태 | 모르는 부분이 있어도 쉽게 포기하지 않고 해결책을 찾아가며 기능을 구현하는 모습을 보며 저 역시 긍정적인 자극을 받을 수 있었습니다. 프로젝트의 완성도를 높이는 데 꾸준히 기여했을 뿐만 아니라, 좋은 아이디어를 제안해 프로젝트 주제를 정하는 과정에서도 중요한 역할을 했습니다. 덕분에 더욱 재미있고 의미 있는 프로젝트를 진행할 수 있었습니다. |
| 신민경 | 의지력과 끈기가 누구보다 뛰어났던 팀원이었습니다. 백엔드 개발이 익숙하지 않아 초반에는 걱정도 많았지만, 그런 우려가 무색할 정도로 끝까지 노력하며 결국 완벽한 결과물을 만들어냈습니다. 특히, 모르는 부분이 생길 때마다 호기심을 가지고 깊이 파고들며 이해하려는 모습이 인상적이었고, 끝내 자신의 것으로 만들어내는 과정에서 많은 걸 배울 수 있었습니다. 또한, 팀원들이 지쳐 있을 때마다 밝은 분위기를 만들어주어 팀워크를 한층 더 끌어올려 준 점도 큰 힘이 되었습니다. 그리고 프로젝트 마무리 단계에서 세심하게 점검하며 놓친 부분을 짚어주어, 마지막까지 완성도를 높이는 데 큰 역할을 해주셨습니다 ! |
| 황수민 | 예원님은 프로젝트 기간 동안 놀라운 의지력과 노력을 보여주셨습니다. 맡은 기능을 다 구현할 수 있을지 걱정하셨지만, 그런 걱정이 무색할 정도로 가장 먼저 기능을 완성해내는 모습을 보며 강한 의지와 집요한 문제 해결력이 돋보인다고 느꼈습니다! 힘든 상황에서도 웃음을 잃지 않고 팀원들에게 긍정적인 에너지를 전해주신 덕분에 즐겁게 프로젝트에 임할 수 있었습니다. 특히, 발표 전날까지 MSA 아키텍처를 구상하고 만들어주신 덕분에 좋은 평가를 받을 수 있었습니다. 묵묵히 해야 할 일을 찾아 수행해주신 덕분에 팀원들의 부담도 한층 덜어질 수 있었어요. 예원님 덕분에 긍정적인 힘을 많이 얻었습니다 감사합니다! |

</details>
