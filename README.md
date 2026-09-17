# OSS Student Management
학생 수강 정보 관리 페이지

---

## Service Topic

수강한 학생의 정보 및 세부 정보 관리

---

## Data Fields

> 학번
> 이름
> 학부
> 학기
> 이메일
> 전화번호

---

## List Page

- 학번
- 이름
- 학부
- 학기

각 버튼을 통해 상세 추가 html로 이동 가능

---

## Validation

`add.html`과 `edit.html`의 Form에서는 입력 데이터의 형식에 맞는 HTML Form Element를 사용하였습니다.
> 학부는 `select`를 이용하여 목록에서 선택하도록 구성
> 학기는 숫자만 입력할 수 있도록 `input type="number"` 사용
> 이메일은 이메일 형식을 확인할 수 있도록 `input type="email"` 사용
> 전화번호는 전화번호 입력에 적합한 `input type="tel"` 사용

---

## Responsive Web Design

- `viewport`를 설정하여 모바일 기기의 화면 너비에 맞도록 구성
- Bootstrap의 `container`를 사용하여 화면 크기에 따라 콘텐츠 영역을 조절
- `table-responsive`를 사용하여 작은 화면에서도 학생 목록 Table을 확인할 수 있도록 구성
- Bootstrap Grid의 `row`, `col-*`을 활용하여 화면 크기에 따라 콘텐츠 크기를 조절
- `col-12`, `col-md-8`, `col-lg-6` 등을 이용하여 Form이 Desktop과 Mobile에서 적절한 폭을 가지도록 구성
- Flexbox를 이용하여 Header와 Button의 위치가 화면 크기에 맞게 유지되도록 구성
- Desktop과 Mobile Device Mode에서 각 페이지의 레이아웃을 확인

---

## Bootstrap

페이지 제작에 Bootstrap 5.3을 사용하였습니다.

주요 Bootstrap Component 및 Class는 다음과 같습니다.

- `container`
- `row`
- `col-*`
- `d-flex`
- `justify-content-between`
- `align-items-center`
- `table`
- `table-striped`
- `table-hover`
- `table-responsive`
- `form-label`
- `form-control`
- `form-select`
- `btn`
- `btn-dark`
- `btn-outline-dark`
- `card`
- `bg-dark`
- `text-white`
- `text-body-secondary`
- `py-*`, `mb-*`, `mt-*`
- `gap-*`


---

## Problem & Solution

- Mobile 환경에서 버튼의 글자가 줄바꿈되는 문제

> 화면의 폭이 작아지면서 Header의 `[학생 추가]` 버튼의 글자가 두 줄로 표시되는 문제가 발생하였습니다.

> Bootstrap의 Flexbox와 `text-nowrap`, `flex-shrink-0` 이용
> 버튼의 크기가 지나치게 줄어들지 않도록 구성

## Reflection

`text-nowrap`, `flex-shrink-0` 이용하여 버튼의 크기가 지나치게 작아짐을 예방 가능