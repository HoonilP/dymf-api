# Customer

<details>
    <summary><strong>Customer</strong></summary>

<details>
  <summary><strong>POST /customer</strong></summary>
  
  > 고객 정보 등록  
  - **Header**: None  
  - **Request**:
    - *name(string)*: 이름
    - *nrc_no(string)*: 주민번호
    - *date_of_birth(string)*: 생년월일
    - *gender(enum)*: 성별
    - *phone_number(string)*: 전화번호
    - email(string): 이메일
    - *loan_type(enum)*: 대출 구분
    - *cp_number(enum)*: 관리 코드
    - *home_address(string)*: 집 주소
    - *home_postal_code(string)*: 집 우편번호
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

</details>