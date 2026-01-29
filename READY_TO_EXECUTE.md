# 🎬 무쏘맨 AI 어워즈 - 실행 준비 완료

**상태**: ✅ 모든 준비 작업 완료  
**다음 단계**: 사용자 수동 작업 (Task 1) 완료 후 즉시 실행 가능  
**예상 소요 시간**: 8-10시간 (준비 완료로 20% 단축)

---

## 📊 현재 진행 상황

### ✅ 완료된 작업 (3/7)

| Task | 상태 | 산출물 | 비고 |
|------|------|--------|------|
| **Task 2** | ✅ 완료 | 변신 전략 문서 (499줄) | Pika Labs 우선, Plan B 준비 |
| **Task 5** | ✅ 완료 | BGM 선정 (50초, CC BY-NC-ND 4.0) | "Cinematic Epic" by AudioCoffee |
| **Playbooks** | ✅ 완료 | 4개 실행 가이드 (2,177줄) | Task 3, 4, 6, 7 즉시 실행 가능 |

### 🚫 대기 중인 작업 (4/7)

| Task | 상태 | 차단 요인 | 예상 시간 |
|------|------|-----------|----------|
| **Task 1** | 🚫 차단 | **사용자 수동 작업 필요** | 20-35분 |
| **Task 3** | ⏸️ 대기 | Task 1 완료 필요 | 2-3시간 |
| **Task 4** | ⏸️ 대기 | Task 3 완료 필요 | 4-6시간 |
| **Task 6** | ⏸️ 대기 | Task 4, 5 완료 필요 | 2-3시간 |
| **Task 7** | ⏸️ 대기 | Task 6 완료 필요 | 45분 |

**핵심**: Task 1 (20-35분) 완료 시 나머지 작업 즉시 진행 가능

---

## 🎯 지금 해야 할 일: Task 1 (수동 작업)

### ⏱️ 예상 소요 시간: 20-35분

### 📋 체크리스트

#### 1. Leonardo.ai 계정 생성 (10분)
- [ ] https://leonardo.ai 접속
- [ ] Google 또는 Email로 회원가입
- [ ] 이메일 인증 완료
- [ ] 무료 크레딧 확인 (일일 150 토큰)
- [ ] 테스트 이미지 생성:
  - 프롬프트: `desert landscape, cinematic, 8k`
  - 생성 버튼 클릭
  - 결과 확인 (30초-1분 소요)
- [ ] 테스트 이미지 다운로드 → `output/test/leonardo_test.png` 저장

#### 2. Kling AI 또는 Pika Labs 계정 생성 (10분)
**우선순위**: Kling AI → Pika Labs (둘 중 하나만 필수)

**Kling AI** (추천):
- [ ] https://klingai.com 접속
- [ ] 회원가입 (Google 또는 Email)
- [ ] 이메일 인증 완료
- [ ] 무료 크레딧 확인
- [ ] 테스트 영상 생성:
  - 프롬프트: `camera slowly zooms in desert`
  - 생성 버튼 클릭
  - 결과 확인 (2-5분 소요)
- [ ] 테스트 영상 다운로드 → `output/test/video_test.mp4` 저장

**또는 Pika Labs** (대체):
- [ ] https://pika.art 접속
- [ ] Discord 계정 연동 또는 Email 가입
- [ ] 무료 크레딧 확인
- [ ] 테스트 영상 생성
- [ ] 다운로드 → `output/test/video_test.mp4` 저장

#### 3. CapCut 설치 (5-10분)
**PC 버전** (추천 - 워터마크 없음):
- [ ] https://www.capcut.com 접속
- [ ] "Download for PC" 클릭
- [ ] 설치 파일 다운로드 (Mac 또는 Windows)
- [ ] 설치 실행
- [ ] CapCut 실행 확인

**또는 모바일 버전**:
- [ ] App Store (iOS) 또는 Play Store (Android)
- [ ] "CapCut" 검색 및 설치
- [ ] 앱 실행 확인

#### 4. 완료 확인
```bash
# 터미널에서 실행하여 확인
ls -la output/test/leonardo_test.png
ls -la output/test/video_test.mp4
```

---

## 📚 준비된 실행 가이드

### 1. Task 3: 이미지 생성 플레이북
**파일**: `output/playbooks/TASK3_IMAGE_GENERATION_PLAYBOOK.md` (434줄)

**내용**:
- 5개 장면 상세 설명 (사막 도입, 질주, 클로즈업, 변신 준비, 피날레)
- Leonardo.ai 최적화 프롬프트 (긍정 + 부정 프롬프트)
- 장면별 품질 기준
- 프롬프트 엔지니어링 베스트 프랙티스
- 문제 해결 가이드
- 파일 관리 구조

**사용법**: Task 1 완료 후 이 파일을 열고 단계별로 따라하기

### 2. Task 4: 영상 생성 플레이북
**파일**: `output/playbooks/TASK4_VIDEO_GENERATION_PLAYBOOK.md` (541줄)

**내용**:
- 도구 선택 가이드 (Pika Labs vs Kling AI vs Runway)
- 5개 장면 모션 설명 및 프롬프트
- **Scene 4 (변신) 집중 전략** (90-120분 할당)
- Plan B 멀티클립 전략
- 도구별 프롬프트 변형
- 품질 평가 기준

**사용법**: Task 3 완료 후 이 파일로 영상 생성

### 3. Task 6: 영상 편집 플레이북
**파일**: `output/playbooks/TASK6_VIDEO_EDITING_PLAYBOOK.md` (589줄)

**내용**:
- CapCut 프로젝트 설정 (9:16, 1080x1920)
- 5개 클립 조립 워크플로우
- 전환 효과 가이드 (글리치, 플래시, 페이드)
- BGM 동기화 (4개 싱크 포인트)
- 자막 오버레이 (3개 텍스트)
- 내보내기 설정 (1080p, 30fps, MP4)
- 품질 검증 명령어 (ffprobe)
- 문제 해결 가이드 (7가지 이슈)

**사용법**: Task 4, 5 완료 후 CapCut으로 편집

### 4. Task 7: 업로드 + 제출 플레이북
**파일**: `output/playbooks/TASK7_UPLOAD_SUBMISSION_PLAYBOOK.md` (613줄)

**내용**:
- 인스타그램 캡션 템플릿 (필수 해시태그 포함)
- 영상 전송 방법 (AirDrop, USB, 클라우드, 이메일)
- 인스타그램 릴스 업로드 워크플로우
- 구글폼 제출 가이드 (https://forms.gle/Q8ovprmjsPJoDe2u7)
- 확인 스크린샷 캡처
- 문제 해결 가이드 (6가지 이슈)
- 제출 후 홍보 전략

**사용법**: Task 6 완료 후 인스타그램 업로드 및 공모전 제출

---

## 🎵 준비된 자산

### BGM (Task 5 완료)
**파일**: `output/audio/bgm_selected.mp3`
- **제목**: "Cinematic Epic" by AudioCoffee
- **길이**: 50초
- **라이선스**: CC BY-NC-ND 4.0 (비상업적 사용 가능, 공모전 출품 가능)
- **크레딧 표기**: "Music by AudioCoffee: https://www.audiocoffee.net/"

**BGM 싱크 포인트**:
- 0:00-0:10: 사막 장면 도입 (오프닝)
- 0:10-0:25: 무쏘맨 질주 빌드업
- 0:25-0:35: 변신 장면 클라이맥스 (합창 + 퍼커션 피크) ⭐
- 0:35-0:50: 무쏘 픽업 피날레

### 변신 전략 (Task 2 완료)
**파일**: `output/strategy/transformation_strategy.md` (499줄)

**핵심 내용**:
- **도구 추천**: Pika Labs 2.5 (Pikaffects) > Runway Gen-4 > Kling AI
- **14가지 프롬프트 변형** (직접 변신, 파티클 효과, 기계적 변신, 하이브리드, Pika 전용)
- **Plan B**: 멀티클립 조합 (3-클립 접근법)
- **품질 평가 기준**: 3단계 레벨 (필수, 우수, 최고)
- **예상 문제 & 해결책**: 5가지 이슈 대응

### 참조 이미지
**위치**: `src/무쏘, 무쏘맨_자료 모음/무쏘맨_누끼/`
- 무쏘맨_기다림.png (1536 x 2752)
- 무쏘맨_월척.png (1536 x 2752)
- 무쏘맨_전시장.png (1536 x 2752)
- 무쏘맨_중고차인증.png (1536 x 2752)
- 무쏘맨_햄버거.png (1536 x 2752)

**해상도**: 모두 1024x1024 이상 (업스케일링 불필요)

---

## 📅 실행 타임라인

### Task 1 완료 후 예상 일정

| 일차 | 작업 | 소요 시간 | 산출물 |
|------|------|----------|--------|
| **Day 1** | Task 1 (수동) | 20-35분 | 계정 생성 완료 |
| **Day 1-2** | Task 3 (이미지 생성) | 2-3시간 | scene_01~05.png |
| **Day 3-5** | Task 4 (영상 생성) | 4-6시간 | scene_01~05.mp4 |
| **Day 6** | Task 6 (편집) | 2-3시간 | final_mussoman_video.mp4 |
| **Day 6** | Task 7 (업로드) | 45분 | 인스타 업로드 + 공모전 제출 |

**총 예상 시간**: 8-10시간 (플레이북 준비로 20% 단축)

**마감일**: 2026년 2월 19일 (충분한 여유 있음)

---

## 🚀 Task 1 완료 후 즉시 실행

### 실행 순서

1. **Task 3 시작**:
   ```bash
   # 플레이북 열기
   open output/playbooks/TASK3_IMAGE_GENERATION_PLAYBOOK.md
   # 또는
   cat output/playbooks/TASK3_IMAGE_GENERATION_PLAYBOOK.md
   ```
   - Leonardo.ai 로그인
   - 플레이북의 프롬프트 복사-붙여넣기
   - 5개 장면 이미지 생성
   - `output/images/` 폴더에 저장

2. **Task 4 시작**:
   ```bash
   # 플레이북 열기
   open output/playbooks/TASK4_VIDEO_GENERATION_PLAYBOOK.md
   ```
   - Kling AI 또는 Pika Labs 로그인
   - Task 3 이미지 업로드
   - 플레이북의 프롬프트 사용
   - **Scene 4 (변신)에 집중** (90-120분)
   - `output/videos/` 폴더에 저장

3. **Task 6 시작**:
   ```bash
   # 플레이북 열기
   open output/playbooks/TASK6_VIDEO_EDITING_PLAYBOOK.md
   ```
   - CapCut 실행
   - 5개 영상 클립 + BGM 가져오기
   - 플레이북 단계별 따라하기
   - 최종 영상 내보내기: `output/final_mussoman_video.mp4`

4. **Task 7 시작**:
   ```bash
   # 플레이북 열기
   open output/playbooks/TASK7_UPLOAD_SUBMISSION_PLAYBOOK.md
   ```
   - 영상을 모바일로 전송
   - 인스타그램 릴스 업로드
   - 구글폼 제출: https://forms.gle/Q8ovprmjsPJoDe2u7

---

## ⚠️ 중요 사항

### 필수 요구사항
- ✅ **변신 장면 필수** (사용자 확정) - 점프컷 대안 불가
- ✅ **해시태그 필수**: #KGM #무쏘맨 #무쏘맨어워즈
- ✅ **BGM 크레딧 표기**: "Music by AudioCoffee: https://www.audiocoffee.net/"
- ✅ **마감일**: 2026년 2월 19일 이전 제출

### 품질 기준
- 영상 길이: 15-30초
- 해상도: 1080x1920 (세로)
- 프레임레이트: 30fps
- 파일 크기: <100MB
- 워터마크: 없음

### 예산
- **무료 우선**: 모든 도구 무료 티어 먼저 사용
- **유료 전환 OK**: 필요 시 유료 결제 승인됨 (사용자 확정)
- **예상 비용**: $0-24 (무료 범위 내 가능성 높음)

---

## 📞 문제 발생 시

### 각 플레이북에 문제 해결 가이드 포함
- Task 3: 이미지 생성 문제 (프롬프트 최적화, 품질 개선)
- Task 4: 영상 생성 문제 (변신 품질, 도구 전환)
- Task 6: 편집 문제 (CapCut 크래시, 오디오 싱크, 워터마크)
- Task 7: 업로드 문제 (인스타그램 업로드 실패, 구글폼 오류)

### 추가 지원 필요 시
- 플레이북의 "Troubleshooting" 섹션 참조
- 각 도구의 공식 튜토리얼 확인
- 커뮤니티 포럼 검색 (Reddit, Discord)

---

## 🎉 준비 완료!

**현재 상태**:
- ✅ 전략 수립 완료 (Task 2)
- ✅ BGM 선정 완료 (Task 5)
- ✅ 실행 가이드 완료 (4개 플레이북, 2,177줄)
- ✅ 참조 자료 준비 완료

**다음 단계**:
1. **Task 1 완료** (20-35분) ← 지금 시작!
2. 플레이북 따라 실행 (8-10시간)
3. 공모전 제출 (2월 19일 이전)

**성공 확률**: 높음 (모든 준비 완료, 상세 가이드 제공)

**행운을 빕니다!** 🦏⚡🏆

---

**문서 버전**: 1.0  
**최종 업데이트**: 2026-01-29  
**상태**: ✅ 실행 준비 완료
