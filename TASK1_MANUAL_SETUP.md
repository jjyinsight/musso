# Task 1: AI 툴 환경 세팅 - 수동 진행 가이드

## 📋 체크리스트

### 1️⃣ Leonardo.ai 세팅
- [ ] https://leonardo.ai 접속
- [ ] 계정 생성 (Google 또는 Email)
- [ ] 로그인 완료
- [ ] 무료 크레딧 확인 (일일 150 토큰)
- [ ] 이미지 생성 테스트:
  - 프롬프트: `desert landscape, cinematic, 8k`
  - 생성 완료 후 이미지 다운로드
  - 저장 위치: `output/test/leonardo_test.png`

### 2️⃣ Kling AI 또는 Pika Labs 세팅
**Kling AI 우선 시도:**
- [ ] https://klingai.com 접속
- [ ] 계정 생성 (Google 또는 Email)
- [ ] 로그인 완료
- [ ] 무료 크레딧 확인
- [ ] 영상 생성 테스트:
  - 프롬프트: `camera slowly zooms in desert`
  - 생성 완료 후 영상 다운로드
  - 저장 위치: `output/test/video_test.mp4`

**Kling AI 실패 시 Pika Labs:**
- [ ] https://pika.art 접속
- [ ] 계정 생성 및 로그인
- [ ] 무료 크레딧 확인
- [ ] 위와 동일한 프롬프트로 영상 생성
- [ ] 저장 위치: `output/test/video_test.mp4`

### 3️⃣ CapCut 설치
- [ ] https://www.capcut.com 접속
- [ ] PC 버전 다운로드 및 설치
  - 또는 모바일 버전 (App Store/Play Store)
- [ ] 설치 완료 후 실행 확인

---

## 📁 파일 저장 위치

```
output/
├── test/
│   ├── leonardo_test.png      ← Leonardo.ai 테스트 이미지
│   └── video_test.mp4         ← Kling/Pika 테스트 영상
```

---

## ✅ 무쏘맨 누끼 이미지 해상도 (이미 확인됨)

모든 이미지가 1536x2752 해상도로 1024x1024 이상 권장 사항 충족:
- 무쏘맨_기다림.png
- 무쏘맨_월척.png
- 무쏘맨_전시장.png
- 무쏘맨_중고차인증.png
- 무쏘맨_햄버거.png

**업스케일링 불필요** - 바로 사용 가능합니다.

---

## 🔍 검증 명령어

완료 후 다음 명령어로 파일 확인:

```bash
# Leonardo.ai 테스트 이미지 확인
ls -la output/test/leonardo_test.png

# Kling/Pika 테스트 영상 확인
ls -la output/test/video_test.mp4

# CapCut 설치 확인 (Mac)
which capcut || ls /Applications/CapCut*

# CapCut 설치 확인 (Windows)
where capcut
```

---

## 📝 완료 후 기록

모든 작업 완료 후 다음 정보를 기록하세요:
1. Leonardo.ai 무료 크레딧 잔량
2. Kling AI 또는 Pika Labs 선택 이유
3. 각 도구의 무료 크레딧 잔량

이 정보는 `.sisyphus/notepads/mussoman-ai-video/decisions.md`에 기록됩니다.

