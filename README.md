# WORK SAFE NOTE — jun2026

WORK SAFE NOTE 개인_5의 새 GitHub 배포 저장소야. 기존 `test` 저장소는 수정하지 않아.

- 현재 작업본: **v1.0.5** (`versionCode 6`)
- Android package: `com.safetyladder.app`
- TBM 등록: https://safe-app.skons.net/services
- 앱 업데이트: `jun2026` 공개 Release에서 최신 `WORK_SAFE_NOTE.apk` 확인 → 사용자 승인 후 설치

## 현재 상태
- 이 저장소는 초기화 중이며, 전체 Android 소스와 APK는 **아직 배포되지 않았어.**
- 위치 주소 표시 오류 수정본은 별도 HTML/Android Studio ZIP으로 제공돼.
- **공개 저장소에는 서명키, 비밀번호, 내부 전용 API 인증값을 업로드하면 안 돼.** 인증값이 포함된 앱 리소스는 별도 검토와 제거가 필요해.
- 첫 릴리스 전 동일 서명키 설정, 빌드 검증, Release APK 첨부가 필요해.

## 빌드 및 업데이트
Android Studio 프로젝트를 저장소 루트에 올린 뒤, GitHub Actions의 서명 비밀값 `WSN_KEYSTORE_BASE64`, `WSN_STORE_PASSWORD`, `WSN_KEY_ALIAS`, `WSN_KEY_PASSWORD`를 설정해야 해. `v1.0.5` 태그를 배포하면 자동 빌드를 시도할 수 있어.

> 앱이 안내하는 업데이트는 자동 다운로드/설치가 아니며 Android의 설치 승인이 필요해. 이전 3.x 버전은 서명키와 versionCode가 달라 덮어쓰기할 수 없을 수 있어.
