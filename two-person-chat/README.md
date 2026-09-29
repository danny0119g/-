# 둘만의 채팅 (GitHub Pages + Firebase)

## 1. Firebase 프로젝트 만들기
1. https://console.firebase.google.com 에서 프로젝트 생성 (Analytics는 꺼도 됩니다)
2. 프로젝트 설정 → 내 앱 → **웹(</>)** 앱 추가 → 표시되는 `firebaseConfig` 값을 복사
3. `index.html` 상단의 `firebaseConfig` 4개 값(apiKey, authDomain, projectId, appId)을 교체

## 2. Firebase 기능 켜기
- **Authentication → 로그인 방법 → 익명** 사용 설정
- **Firestore Database → 데이터베이스 만들기** (프로덕션 모드, 가까운 리전 예: asia-northeast3 서울)
- **Firestore → 규칙** 탭에 `firestore.rules` 내용을 붙여넣고 **게시**
- **Authentication → 설정 → 승인된 도메인**에 `아이디.github.io` 추가

## 3. GitHub Pages 켜기
저장소 → Settings → Pages → Branch: `main` / root → Save
접속 주소: `https://아이디.github.io/저장소명/`

## 4. 사용법
페이지를 열면 방 링크(`#room=...`)가 자동 생성됩니다. 상단 **초대 링크** 버튼으로 복사해서 상대방에게 보내세요.
링크를 아는 사람만 같은 방에 들어올 수 있으니 다른 사람에게 공유하지 마세요.
