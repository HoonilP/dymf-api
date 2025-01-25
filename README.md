# Customer
<details>
<summary>span<p>$\bf{\large{\color{#6580DD}POST}}$ /customer</p></summary>
    - 고객 정보 등록
    - /customer
    - Header: -
    - Request:
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
    - Response: -
</details>
<details>
<summary><span style="color:red">DELETE</span> /customer</summary>
	고객 정보 삭제
	<details>
	<summary>Header</summary>
	</details>
	<details>
	<summary>Request</summary>
		*id(int): id
	</details>
	<details>
	<summary>Response</summary>
	</details>
</details>
<details>
<summary><span style="color:orange">PUT</span> /customer/id</summary>
	고객 정보 수정
	<details>
	<summary>Header</summary>
	</details>
	<details>
	<summary>Request</summary>
		name(string): 이름
		nrc_no(string): 주민번호
		date_of_birth(string): 생년월일
		gender(enum): 성별
		phone_number(string): 전화번호
		email(string): 이메일
		loan_type(enum): 대출 구분
		cp_number(enum): 관리 코드
		home_address(string): 집 주소
		home_postal_code(string): 집 우편번호
		office_address(string): 사무실 주소
		office_postal_code(string): 사무실 우편번호
		details([string]): 추가 정보
		image(???): 사진
	</details>
	<details>
	<summary>Response</summary>
	</details>
</details>
