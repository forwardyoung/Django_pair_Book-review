# 📖 Django_Book Review
![image](https://user-images.githubusercontent.com/99783474/199030424-b19938a6-15f2-4635-bcde-49a0a2fc8cc1.png)



## ✔ 목표
페어 프로그래밍을 통한 영화 리뷰 커뮤니티 서비스를 개발합니다. 아래 조건을 만족해야 합니다.

- **CRUD** 구현(구현 방법 제한 없음)
- **Staticfiles** 활용 정적 파일(이미지, CSS, JS) 다루기
- Django **Auth** 활용 회원 관리(회원 가입 / 회원 조회 / 로그인 / 로그아웃)
- Media 활용 동적 파일 다루기
- 모델간 **1 : N / M : N 관계** 매핑

## ✔ 요구 사항

### 📚 모델 Model (모델 이름 : User, 모델 이름 : Review, 모델 이름 : Comment)


### 📚 **폼 Form** 

> `회원가입`, `로그인`, `기능 view`, `리뷰 reviews`, `데이터 생성`, `데이터 수정`, `데이터 삭제`

> 리뷰 `좋아요 / 좋아요 취소`, `댓글 comments`, `댓글 생성`, `댓글 삭제`

> 회원 관리 accounts `회원 가입`, `회원 목록 조회`, `회원 정보 조회`, `로그인`, `로그아웃`, `팔로우`


### 📚 화면 Template

> `메인 페이지`, `목록 페이지`, `리뷰 정보 페이지`, `리뷰 작성 페이지`, `리뷰 수정 페이지`

> `회원 가입 페이지`, `회원 조회 페이지(프로필 페이지)`, `로그인 페이지`, `팔로우 버튼`


---

### 💡 주의할점
#### ❌ 에러 발생 문구 : NoReverseMatch at /'accounts' is not a registered namespace

pjt 폴더의 urls.py에서 path를 

```python
path('accounts/', include('allauth.urls')),
```

로 설정하였더니 에러가 발생
```python 
path("accounts/", include("accounts.urls")),
```
로 수정하여 해결

---

### ✔ 다크 모드 기능 구현

![2022-10-31 23;32;43](https://user-images.githubusercontent.com/99783474/199033212-1bfd5d36-0c77-40a7-921d-1506f352bf4d.gif)

---

### ✔메인 페이지 










