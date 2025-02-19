# network

## 커리큘럼
### 교재
[컴퓨터 네트워킹: 하향식 접근 (제8판)](http://www.yes24.com/Product/Goods/112228953)

### 강의
https://www.youtube.com/playlist?list=PLoCMsyE1cvdWKsLVyf6cPwCLDIZnOj0NS

### 실습
https://cs144.github.io/

## 📂 디렉터리 구조
```
/ ── network/
    ├── book/              # 책/강의 정리
    ├── exercises/         # 실습 코드 및 정리
    ├── resources/         # 참고 자료 및 링크
    ├── README.md          # 저장소 개요
```
## 실행 방법
#### 1️⃣ 원본 저장소 Fork

각자 원본 저장소를 Fork하여 자신의 GitHub 계정에 저장소를 만든다.

Fork된 개인 저장소에서 book/{본인이름}, exercises/{본인이름} 브랜치를 생성하고 작업을 진행한다.

```
# 예시: 자신의 실습 브랜치에서 작업 시작
git checkout -b exercises/myname
```

##### 2️⃣ 작업 후 개인 Fork 저장소에 반영
```
git add .
git commit -m "[Exercise] TCP 연결 실습 추가"
git push origin exercises/myname
```

#### 3️⃣ 원본 저장소에 PR(Pull Request) 제출

#### 4️⃣ Fork 저장소를 원본 저장소와 Sync하지 않음

원본 저장소의 변경 사항을 내 Fork 저장소로 가져오지 않는다.

즉, git fetch upstream을 실행하더라도 git merge upstream/main을 하지 않으면 된다.

## 🌱 브랜치 전략
```
main: 최종 정리본 (수동 병합)
excercises/{본인이름}
book/{본인이름}
main에 병합시 브랜치 삭제
```

## ✏️ 커밋 메시지 규칙
```
[Book] 책 / 강의 요약 작성

[Exercise] 실습 코드 작성

[Assignment] 과제 수행

[Fix] 오류 수정

[Docs] 문서 정리

[Refactor] 코드 리팩토링
```

예시
- [Lecture] 1.1 컴퓨터 네트워크와 인터넷
- [Exercise] TCP 연결 실습 추가
- [Fix] 패킷 캡처 코드 오류 수정


## PR (Pull Request) 규칙
PR 제목: [작업 유형] 작업 내용

PR 설명:
- 작업 내용 요약
- 변경 사항
- 추가 학습이 필요한 내용


