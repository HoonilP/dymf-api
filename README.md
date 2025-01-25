# API 명세
## 공통 응답/요청 방식, JSON 정의
1. API 요청 형식은  *‘application/json’*으로 제한합니다. 이때 application 대신에 app으로 줄여서 씁니다.
2. 성공/실패 여부는 HTTP 상태코드를 통해 제공합니다. 상태 코드는 다음과 같습니다.   
    - 200번대 : 성공
    - 300번대 : 리다이렉트
    - 400번대 : 클라이언트 오류(request error)
    - 500번대 : 서버 오류

- JSON 형식
```json
{
	"code" : 
	"message":
	"result" : 
}
```

## Customer
<details>
  <summary><strong>POST /customer</strong></summary>
  
  > 고객 정보 등록  
  - **Header**: None  
  - **Request**:
    - *name(string): 이름
    - *nrc_no(string): 주민번호
    - *date_of_birth(string): 생년월일
    - *gender(enum): 성별
    - *phone_number(string): 전화번호
    - email(string): 이메일
    - *loan_type(enum): 대출 구분
    - *cp_number(enum): 관리 코드
    - *home_address(string): 집 주소
    - *home_postal_code(string): 집 우편번호
    - office_address(string): 사무실 주소
    - office_postal_code(string): 사무실 우편번호
    - details([string]): 추가 정보
    - image(???): 사진  
  - **Response**: None
</details>
<details>
  <summary><strong>DELETE /customer</strong></summary>
  
  > 고객 정보 삭제  
  - **Header**: None  
  - **Request**:
    - *id(int)*: ID  
  - **Response**: None
</details>
<details>
  <summary><strong>GET /customer/id</strong></summary>
  
  > 고객 정보 조회
  - **Header**: None
  - **Request**:
    - id(int): id
  - **Response**:
    - name(string): 이름
    - nrc_no(string): 주민번호
    - date_of_birth(string): 생년월일
    - gender(enum): 성별
    - phone_number(string): 전화번호
    - email(string): 이메일
    - loan_type(enum): 대출 구분
    - cp_number(enum): 관리 코드
    - home_address(string): 집 주소
    - home_postal_code(string): 집 우편번호
    - office_address(string): 사무실 주소
    - office_postal_code(string): 사무실 우편번호
    - details([string]): 추가 정보
    - image(???): 사진
</details>
<details>
  <summary><strong>PUT /customer/id</strong></summary>
  
  > 고객 정보 수정  
  - **Header**: None  
  - **Request**:
    - name(string): 이름
    - nrc_no(string): 주민번호
    - date_of_birth(string): 생년월일
    - gender(enum): 성별
    - phone_number(string): 전화번호
    - email(string): 이메일
    - loan_type(enum): 대출 구분
    - cp_number(enum): 관리 코드
    - home_address(string): 집 주소
    - home_postal_code(string): 집 우편번호
    - office_address(string): 사무실 주소
    - office_postal_code(string): 사무실 우편번호
    - details([string]): 추가 정보
    - image(???): 사진  
  - **Response**: None
</details>

