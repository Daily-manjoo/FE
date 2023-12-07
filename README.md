## Overview

## 인싸가 되고싶어? 소셜 미디어 Inssagram

인스타그램 + 블라인드로 직장인들의 소셜 네트워크 웹 어플리케이션

## **Project**

[inssagram](https://github.com/inssagram)

### 🎯 Trouble Shooting

# 검색 input 렌더링 오류

## 🚨이슈

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/44838c05-45d7-4ee9-815f-a006e1f3ec45/b38d0f06-a991-4a1d-a8d5-618db35866a2/Untitled.png)

1. 검색 입력 시 최근 검색 기록과 검색 결과 리스트가 함께 보임

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/44838c05-45d7-4ee9-815f-a006e1f3ec45/970b15d5-3f7c-4580-a789-20adc0fc2653/Untitled.png)

1. 입력 값이 없는데도 검색 결과 리스트가 조회됨.

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/44838c05-45d7-4ee9-815f-a006e1f3ec45/59dce605-f1f4-43f0-82ed-0bc5d8f562e1/Untitled.png)

1. 대화 상대를 선택한 후 SearchInput에 `memberNickname`을 props로 전달했을 때 이전 검색 값이 초기화되지 않는 오류가 발생함.

## 🔍 원인 도출

1. **검색어 입력 시 최근 검색 기록과 결과 리스트 함께 보이는 이슈:**
2. **입력 값이 없는데도 검색 결과 리스트가 조회되는 이슈:**
3. **대화 상대를 선택 후 ‘SearchInput’에 `memberNickname`을 전달할 때 이전 검색 값이 초기화되지 않는 이슈:**

## ⚒️ 해결

1. **`isSelectedAccount`**에 boolean 값을 할당하여 검색 페이지에서 더 명확한 조건에 따라 데이터를 렌더링하도록 하였음.
2. **`searchTerm`** 값이 지워질 때 초기화되도록 코드를 추가함.
3. **`selectedAccount`**에서 배열로 담고 있던 부분의 타입 정의를 **`string`**으로 수정하였고, 입력 값이 지워질 때 **`SearchInput`**에 담긴 값이 초기화되도록 코드를 추가하였음.

[WebSocket 연결시 헤더 설정 오류](https://www.notion.so/WebSocket-70f02357eeeb44479dfdf187508b5ca0?pvs=21)

[Elasticsearch 렌더링 오류](https://www.notion.so/Elasticsearch-2b4f928d99784d32b92b1e764a431138?pvs=21)

[컴포넌트 내 렌더링 오류](https://www.notion.so/d12bec9067434a5a8bcfa6565efe9fd7?pvs=21)

[SSE 연결시 헤더 설정 오류](https://www.notion.so/SSE-8c198ff37ce1481e82da3f97e3dc6a61?pvs=21)

[Redux-toolkit 적용 시 **A non-serializable value error**](https://www.notion.so/Redux-toolkit-A-non-serializable-value-error-459069a3aa354591898801d3592509e5?pvs=21)

[AWS 용량 초과에 따른 Firebase 이용](https://www.notion.so/AWS-Firebase-19a39ff24a3646c2a5420dc5bc2c98a7?pvs=21)

[이미지를 압축하여 로드 속도 개선](https://www.notion.so/42fdcbb304304627ade9aabb943bbea5?pvs=21)

[Next.js pages 폴더 구조 관리](https://www.notion.so/Next-js-pages-f646e4e2362c41e282493341fd25db13?pvs=21)

[이메일 인증 버튼 오버클릭 방지](https://www.notion.so/245b84a7de6a4c8e9c9c0cd38432101e?pvs=21)

[FOUC 개선](https://www.notion.so/FOUC-c6261746326f4df185cef2303d73c9b0?pvs=21)
### 🖥️ Tech Stack

---

### FE

`Next.js + React JS`

`Typescript`

`Redux-toolkit`

`Axios`

`WebSocket`

`SSE`

`FireBase`

`Styled-components`

`Fontawesome`

### BE

`SpringBoot` `SpringSecurity` `SpringDataJPA`

`AWS RDS(MySQL)` `AWS S3`

`JWT` 

 `AWS Certificate Manager` `SSL`

 `WebSoket` `SSE`

### CI / CD

**FE :**  `Github`  `Github Actions` `Vercel`

**BE :**  `Github Actions` `AWS` `EC2` `AWS CodeDeploy`

**Communication**

`Slack` `Gather`
