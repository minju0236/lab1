# 자재관리 CRUD 구조

## 전체 흐름

**Express서버**에서 모든 요청 처리

MySQL DB와 연결하여 데이터 관리

HTML 템플릿에 데이터를 넣어 화면 출력

## 기능별 구성
## 1. 자재 목록 조회 (/material/list)

DB에서 전체 자재 조회

테이블 형태로 리스트 출력

조회 / 수정 / 삭제 기능 연결

## 2. 자재 등록 (/material/write)

입력 폼 제공

POST 요청으로 DB에 데이터 저장

저장 후 리스트로 이동

## 3. 자재 상세 조회 (/material/detail/:id)

특정 자재 정보 조회

상세 데이터 화면 출력

## 4. 자재 수정 (/material/edit/:id)

기존 데이터 불러오기

수정 후 DB 업데이트

상세 페이지로 이동

## 5. 자재 삭제 (/material/delete/:id)

해당 자재 DB에서 삭제

삭제 후 리스트로 이동

## 6. 예외 처리 (message 페이지)

DB 오류 / 데이터 없음 처리

사용자에게 메시지 페이지 제공

## 템플릿 역할

**material-list.html** → 리스트 화면

**material-write.html** → 등록 화면

**material-detail.html** → 상세 화면

**material-edit.html** → 수정 화면

**material-message.html** → 에러/알림
