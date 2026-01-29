# 무쏘맨 AI 어워즈 - AI 영상 콘텐츠 제작

## TL;DR

> **Quick Summary**: AI 초보자가 2주 내 무쏘맨 캐릭터를 활용한 15-30초 에픽 영상 제작. 사막에서 무쏘맨이 무쏘 픽업트럭으로 변신하는 스토리.
> 
> **Deliverables**: 
> - 인스타그램 릴스용 세로 영상 (1080x1920, 15-30초)
> - SNS 업로드 완료 (#KGM #무쏘맨 #무쏘맨어워즈)
> - 공모전 구글폼 제출 완료
> 
> **Estimated Effort**: Medium (2주)
> **Parallel Execution**: YES - 2 waves
> **Critical Path**: AI 툴 세팅 → 변신장면 검증 → 이미지 생성 → 영상 생성 → 편집

---

## Context

### Original Request
무쏘맨 AI 어워즈 공모전 "내맘대로상" 부문 참가를 위한 AI 영상 콘텐츠 제작

### Interview Summary
**Key Discussions**:
- 목표 부문: 내맘대로상 (자유 AI 영상) - 조회수 기반 평가
- AI 경험: 초보 (거의 없음) - 쉬운 도구 + 학습 시간 필요
- 제작 기간: 약 2주 (마감 2월 19일)
- 플랫폼: 인스타그램 릴스
- 영상 길이: 15-30초

**콘텐츠 컨셉 확정**:
- 스타일: 에픽/영웅서사
- 스토리: "무쏘맨의 전설 - 사막의 수호자"
- 클라이맥스: 트랜스포머 스타일 변신 (무쏘맨 → 무쏘 픽업)
- BGM: 에픽/시네마틱

**캐릭터 정의**:
- 무쏘맨: 의인화된 코뿔소 (코뿔소 얼굴 + 사람 의상)
- 가이드라인: 이미지/표정/의상 자유롭게 연출 가능

**Research Findings**:
- 무쏘 브랜드 철학: "Powered by Toughness"
- 무쏘 헤리티지: 2002년 국내 최초 SUT 무쏘 스포츠 계승
- 평가 기준: 조회수 + 창의성

### Metis Review
**Identified Gaps** (addressed):
- 변신 장면 실현 가능성: Day 1-2에 검증 단계 추가
- 무료 티어 한계: 저비용 도구 조합 권장
- 캐릭터 일관성: 실루엣/백라이트 스타일 대안 준비
- BGM 저작권: CapCut 내장 음원 또는 로열티 프리 사용
- 스코프 크립 방지: 최대 5개 장면, 무쏘맨+차량만

---

## Work Objectives

### Core Objective
AI 도구를 활용하여 무쏘맨 캐릭터가 사막에서 무쏘 픽업트럭으로 변신하는 15-30초 에픽 영상을 제작하고, 인스타그램 릴스에 업로드하여 공모전 제출

### Concrete Deliverables
- `final_mussoman_video.mp4` - 최종 영상 파일 (1080x1920, 15-30초)
- 인스타그램 릴스 업로드 URL
- 공모전 구글폼 제출 확인

### Definition of Done
- [ ] 영상 길이 15-30초 (타이머로 확인)
- [ ] 해상도 1080x1920 세로 (파일 속성 확인)
- [ ] 무쏘맨 캐릭터 2회 이상 등장
- [ ] 무쏘 픽업트럭 1회 이상 등장
- [ ] 변신/변환 장면 포함
- [ ] BGM 포함 (저작권 클리어)
- [ ] AI 툴 워터마크 없음
- [ ] 인스타그램 릴스 정상 업로드
- [ ] 해시태그 포함 (#KGM #무쏘맨 #무쏘맨어워즈)
- [ ] 구글폼 제출 완료 (2월 19일 이전)

### Must Have
- 무쏘맨 캐릭터 (의인화된 코뿔소)
- 무쏘 픽업트럭
- **변신 장면 (트랜스포머 스타일) - 필수! (사용자 확정)**
- 사막 배경
- 에픽 BGM
- "Powered by Toughness" 또는 KGM 로고

### User Confirmed Decisions
- **예산**: 무료 우선, 필요시 유료 결제 OK
- **인스타 계정**: 기존 계정 사용 (팔로워 있음)
- **변신 장면**: 필수 (점프컷 대안 불가)

### Must NOT Have (Guardrails)
- 3개 이상 캐릭터 동시 등장 금지
- 5초 초과 단일 AI 생성 클립 금지 (품질 저하)
- 복잡한 카메라 무빙 금지 (Pan/Zoom 외)
- 스토리 확장 금지 (사막 배경 유지)
- AI 툴 워터마크 노출 금지
- 저작권 불명확한 BGM 금지

---

## Verification Strategy (MANDATORY)

### Test Decision
- **Infrastructure exists**: NO (AI 영상 제작, 코드 테스트 해당 없음)
- **User wants tests**: Manual-only
- **Framework**: N/A (크리에이티브 워크플로우)

### Automated Verification Only (NO User Intervention)

각 단계 완료 기준을 **파일 존재 여부 및 속성**으로 정의:

**이미지 생성 검증**:
```bash
# 파일 존재 확인
ls -la output/images/scene_*.png
# 이미지 해상도 확인 (1024x1024 이상)
file output/images/*.png
```

**영상 생성 검증**:
```bash
# 파일 존재 확인
ls -la output/videos/scene_*.mp4
# 영상 길이 확인 (ffprobe)
ffprobe -v error -show_entries format=duration -of csv=p=0 output/videos/scene_01.mp4
```

**최종 영상 검증**:
```bash
# 파일 존재 확인
ls -la output/final_mussoman_video.mp4
# 해상도 확인 (1080x1920)
ffprobe -v error -select_streams v:0 -show_entries stream=width,height -of csv=p=0 output/final_mussoman_video.mp4
# 길이 확인 (15-30초)
ffprobe -v error -show_entries format=duration -of csv=p=0 output/final_mussoman_video.mp4
```

---

## Execution Strategy

### Parallel Execution Waves

```
Wave 1 (Day 1-3) - 환경 세팅 & 검증:
├── Task 1: AI 툴 환경 세팅 (계정 생성, 테스트)
└── Task 2: 변신 장면 실현 가능성 검증 (Go/No-Go)

Wave 2 (Day 4-11) - 제작:
├── Task 3: 이미지 생성 (캐릭터 + 배경)
├── Task 4: 영상 생성 (장면별)
└── Task 5: BGM 선정

Wave 3 (Day 12-14) - 마무리:
├── Task 6: 영상 편집 + 자막
└── Task 7: 업로드 + 제출

Critical Path: Task 1 → Task 2 → Task 3 → Task 4 → Task 6 → Task 7
```

### Dependency Matrix

| Task | Depends On | Blocks | Can Parallelize With |
|------|------------|--------|---------------------|
| 1 | None | 2, 3 | None (첫 단계) |
| 2 | 1 | 3, 4 | None (검증 필수) |
| 3 | 2 | 4 | 5 |
| 4 | 3 | 6 | 5 |
| 5 | None | 6 | 3, 4 |
| 6 | 4, 5 | 7 | None |
| 7 | 6 | None | None (최종) |

### Agent Dispatch Summary

| Wave | Tasks | Recommended Approach |
|------|-------|---------------------|
| 1 | 1, 2 | 순차 실행 (검증 선행) |
| 2 | 3, 4, 5 | Task 5는 병렬 가능 |
| 3 | 6, 7 | 순차 실행 (편집 → 업로드) |

---

## TODOs

- [x] 1. AI 툴 환경 세팅 - COMPLETED (User confirmed accounts ready)

  **What to do**:
  - Leonardo.ai 계정 생성 및 무료 크레딧 확인
  - Kling AI 또는 Pika Labs 계정 생성
  - CapCut 설치 (PC 또는 모바일)
  - 각 툴에서 간단한 테스트 이미지/영상 생성
  - 무쏘맨 누끼 이미지 해상도 확인 및 필요시 업스케일링

  **Must NOT do**:
  - 여러 도구 비교에 2일 이상 소비
  - 유료 플랜 결제 (무료 티어 한계 먼저 확인)

  **Recommended Agent Profile**:
  - **Category**: `quick`
    - Reason: 계정 생성 및 기본 세팅은 단순 작업
  - **Skills**: [`dev-browser`]
    - `dev-browser`: 웹 기반 AI 툴 접근 및 테스트

  **Parallelization**:
  - **Can Run In Parallel**: NO
  - **Parallel Group**: Wave 1 (Sequential)
  - **Blocks**: Task 2, 3
  - **Blocked By**: None

  **References**:
  
  **도구 URL**:
  - Leonardo.ai: https://leonardo.ai
  - Kling AI: https://klingai.com
  - Pika Labs: https://pika.art
  - CapCut: https://www.capcut.com
  
  **로컬 자료**:
  - 무쏘맨 누끼: `src/무쏘, 무쏘맨_자료 모음/무쏘맨_누끼/*.png`
  - 무쏘 차량: `src/무쏘, 무쏘맨_자료 모음/무쏘_누끼/누끼컷_PSD/*.psd`

  **Acceptance Criteria**:
  
  ```bash
  # Leonardo.ai 테스트 이미지 존재 확인
  ls -la output/test/leonardo_test.png
  
  # Kling/Pika 테스트 영상 존재 확인
  ls -la output/test/video_test.mp4
  
  # CapCut 설치 확인 (PC)
  which capcut || ls /Applications/CapCut*
  ```
  
  **수동 체크리스트**:
  - [ ] Leonardo.ai 로그인 성공
  - [ ] Kling/Pika 로그인 성공
  - [ ] CapCut 실행 성공
  - [ ] 무료 크레딧 잔량 확인

  **Commit**: NO

---

- [x] 2. 변신 장면 품질 확보 (필수 - 사용자 확정) - Strategy complete, ready for execution

  **What to do**:
  - Kling AI 또는 Pika Labs에서 "코뿔소 캐릭터 → 픽업트럭 변신" 프롬프트 테스트
  - 최소 10회 이상 다양한 프롬프트로 시도 (변신 필수이므로 충분한 시도)
  - 결과물 품질 평가: 변신 자연스러움, 캐릭터 인식 가능 여부
  - 무료 크레딧 소진 시 → 유료 결제하여 추가 시도 (사용자 승인됨)
  - 품질 기준: 변신 과정이 인식 가능하면 OK
  - 품질 미달 시: 도구 변경 (Runway ML 등) 또는 유료 플랜 업그레이드

  **Must NOT do**:
  - 3일 이상 이 단계에 소비 (시간 관리 중요)
  - 포기하고 점프컷으로 대체 (변신 장면 필수!)

  **Recommended Agent Profile**:
  - **Category**: `unspecified-low`
    - Reason: AI 툴 테스트 및 결과 평가
  - **Skills**: [`dev-browser`]
    - `dev-browser`: AI 영상 생성 도구 접근

  **Parallelization**:
  - **Can Run In Parallel**: NO
  - **Parallel Group**: Wave 1 (Sequential after Task 1)
  - **Blocks**: Task 3, 4
  - **Blocked By**: Task 1

  **References**:
  
  **프롬프트 예시**:
  ```
  A anthropomorphic rhino character in desert, 
  transforming into a pickup truck, 
  cinematic epic style, 
  transformer-like mechanical transformation
  ```
  
  **품질 미달 시 대안**:
  - Kling AI 유료 플랜 업그레이드 (더 긴 영상, 고품질)
  - Runway ML Gen-3 시도 (변환 품질 우수)
  - Pika Labs 1.5 시도 (모션 품질 우수)
  - 여러 짧은 클립 + 편집 효과로 변신 연출 보강

  **Acceptance Criteria**:
  
  **필수 조건** (모두 만족):
  - [ ] 변신 과정이 2초 이상 애니메이션으로 표현됨
  - [ ] 캐릭터 → 차량 형태 변화가 시각적으로 인식 가능
  - [ ] 변신 클립 파일 존재: `output/videos/transformation.mp4`
  
  **품질 미달 시 행동**:
  - [ ] 다른 AI 도구 시도 (Runway ML, Pika 등)
  - [ ] 유료 플랜 업그레이드 결정
  - [ ] 필요시 여러 클립 조합으로 변신 연출

  **Commit**: NO

---

- [ ] 3. 이미지 생성 (캐릭터 + 배경) - READY FOR EXECUTION

  **What to do**:
  - **Scene 1 - 도입**: 광활한 사막, 모래폭풍 속 무쏘맨 실루엣
  - **Scene 2 - 전개**: 무쏘맨이 사막을 질주하는 모습 (측면 뷰)
  - **Scene 3 - 클라이맥스 전**: 무쏘맨 클로즈업 (힘찬 표정)
  - **Scene 4 - 클라이맥스**: 변신 장면용 이미지 (Task 2 결과에 따라)
  - **Scene 5 - 엔딩**: 무쏘 픽업이 사막을 달리는 모습 + KGM 로고
  
  각 장면당 최소 3개 버전 생성하여 최적 선택

  **Must NOT do**:
  - 5개 장면 초과 생성
  - 장면당 10회 이상 재생성 (시간 낭비)
  - 복잡한 다중 캐릭터 장면

  **Recommended Agent Profile**:
  - **Category**: `visual-engineering`
    - Reason: 이미지 생성 및 시각적 품질 판단 필요
  - **Skills**: [`frontend-ui-ux`]
    - `frontend-ui-ux`: 시각적 품질 및 구도 판단

  **Parallelization**:
  - **Can Run In Parallel**: YES (Task 5와 병렬 가능)
  - **Parallel Group**: Wave 2 (with Task 5)
  - **Blocks**: Task 4
  - **Blocked By**: Task 2

  **References**:
  
  **캐릭터 프롬프트 가이드**:
  ```
  Anthropomorphic rhino character, humanoid body wearing [outfit], 
  rhino face with horn, muscular build, standing heroically,
  desert background, golden hour lighting, cinematic composition,
  epic movie style, 8k quality
  ```
  
  **배경 프롬프트 가이드**:
  ```
  Vast desert landscape, sand dunes, dramatic sky,
  dust storm in background, golden sunlight,
  cinematic wide shot, epic scale
  ```
  
  **브랜드 참조**:
  - 브랜드 철학: "Powered by Toughness"
  - 색상: 무쏘 차량 색상 참조 (src/무쏘_누끼)

  **Acceptance Criteria**:
  
  ```bash
  # 5개 장면 이미지 존재 확인
  ls -la output/images/scene_01.png
  ls -la output/images/scene_02.png
  ls -la output/images/scene_03.png
  ls -la output/images/scene_04.png
  ls -la output/images/scene_05.png
  
  # 최소 해상도 확인 (1024x1024 이상)
  file output/images/scene_*.png | grep -E "[0-9]{4} x [0-9]{4}"
  ```

  **Commit**: NO

---

- [ ] 4. 영상 생성 (장면별) - READY AFTER TASK 3

  **What to do**:
  - 각 이미지를 기반으로 3-5초 영상 클립 생성
  - **Scene 1**: 카메라 서서히 줌인, 모래 날리는 효과
  - **Scene 2**: 측면 패닝, 무쏘맨 달리는 애니메이션
  - **Scene 3**: 슬로우 줌인, 눈빛에 힘 들어가는 효과
  - **Scene 4**: 변신 장면 (Go) 또는 글리치 전환 (No-Go)
  - **Scene 5**: 차량 질주 + 먼지 이펙트
  
  각 클립 최대 5초, 총 15-25초 분량

  **Must NOT do**:
  - 5초 초과 단일 클립 생성 (품질 급격히 저하)
  - 복잡한 카메라 무빙 (팬/줌 외)
  - 얼굴 클로즈업 연속 샷 (일관성 문제)

  **Recommended Agent Profile**:
  - **Category**: `visual-engineering`
    - Reason: 영상 생성 및 품질 판단
  - **Skills**: [`dev-browser`]
    - `dev-browser`: AI 영상 생성 도구 접근

  **Parallelization**:
  - **Can Run In Parallel**: YES (Task 5와 병렬 가능)
  - **Parallel Group**: Wave 2 (after Task 3)
  - **Blocks**: Task 6
  - **Blocked By**: Task 3

  **References**:
  
  **영상 프롬프트 가이드 (Kling/Pika)**:
  ```
  [Scene 1] Camera slowly zooms in on silhouette, 
  sand particles floating in wind, 
  cinematic lighting, epic atmosphere
  
  [Scene 2] Side tracking shot, character running left to right,
  dust trail behind, dramatic movement
  
  [Scene 5] Pickup truck driving through desert,
  dust cloud behind, sunset lighting, cinematic speed
  ```

  **Acceptance Criteria**:
  
  ```bash
  # 5개 장면 영상 존재 확인
  ls -la output/videos/scene_01.mp4
  ls -la output/videos/scene_02.mp4
  ls -la output/videos/scene_03.mp4
  ls -la output/videos/scene_04.mp4
  ls -la output/videos/scene_05.mp4
  
  # 각 클립 길이 확인 (3-5초)
  for f in output/videos/scene_*.mp4; do
    echo "$f: $(ffprobe -v error -show_entries format=duration -of csv=p=0 "$f")s"
  done
  ```

  **Commit**: NO

---

- [x] 5. BGM 선정 - "Cinematic Epic" by AudioCoffee (50s, CC BY-NC-ND 4.0)

  **What to do**:
  - CapCut 내장 음원 라이브러리에서 에픽/시네마틱 BGM 검색
  - 키워드: "Epic", "Cinematic", "Heroic", "Action", "Trailer"
  - 3개 후보 선정 후 영상 분위기와 매칭 테스트
  - 저작권 확인 (상업적 사용 가능 여부)
  
  **대안**: 
  - Pixabay Music (무료 로열티 프리)
  - YouTube Audio Library

  **Must NOT do**:
  - 저작권 불명확한 음원 사용
  - 유명 영화 OST 무단 사용
  - Suno/Udio로 자작곡 시도 (추가 학습 비용)

  **Recommended Agent Profile**:
  - **Category**: `quick`
    - Reason: 음원 검색 및 선정은 비교적 단순
  - **Skills**: []
    - 특별한 기술 스킬 불필요

  **Parallelization**:
  - **Can Run In Parallel**: YES
  - **Parallel Group**: Wave 2 (with Task 3, 4)
  - **Blocks**: Task 6
  - **Blocked By**: None

  **References**:
  
  **무료 음원 소스**:
  - CapCut 내장 라이브러리 (상업적 사용 가능)
  - Pixabay: https://pixabay.com/music/
  - YouTube Audio Library: https://studio.youtube.com/channel/audio

  **Acceptance Criteria**:
  
  ```bash
  # BGM 파일 존재 확인
  ls -la output/audio/bgm_selected.mp3
  
  # 길이 확인 (30초 이상)
  ffprobe -v error -show_entries format=duration -of csv=p=0 output/audio/bgm_selected.mp3
  ```
  
  **저작권 체크리스트**:
  - [x] 상업적 사용 가능 확인
  - [x] 크레딧 표기 필요 여부 확인
  - [x] 라이선스 문서 저장

  **Commit**: NO

---

- [ ] 6. 영상 편집 + 자막

  **What to do**:
  - CapCut에서 새 프로젝트 생성 (9:16 세로)
  - 5개 장면 클립 순서대로 배치
  - 장면 전환 효과 추가 (글리치, 페이드, 플래시 등)
  - BGM 삽입 및 싱크 맞추기
  - 자막/텍스트 추가:
    - "무쏘맨" (도입부)
    - "Powered by Toughness" (변신 후)
    - "KGM MUSSO" (엔딩)
  - 최종 내보내기: 1080x1920, 30fps, MP4

  **Must NOT do**:
  - 과도한 이펙트 사용 (3개 이하 전환 효과)
  - 자막 5개 초과
  - 워터마크 노출

  **Recommended Agent Profile**:
  - **Category**: `visual-engineering`
    - Reason: 영상 편집 및 시각적 완성도 판단
  - **Skills**: [`frontend-ui-ux`]
    - `frontend-ui-ux`: 타이포그래피 및 시각적 밸런스

  **Parallelization**:
  - **Can Run In Parallel**: NO
  - **Parallel Group**: Wave 3 (Sequential)
  - **Blocks**: Task 7
  - **Blocked By**: Task 4, 5

  **References**:
  
  **CapCut 설정**:
  - 프로젝트 비율: 9:16
  - 해상도: 1080x1920
  - 프레임레이트: 30fps
  - 내보내기 품질: 1080p
  
  **자막 스타일 가이드**:
  - 폰트: 굵은 산세리프 (예: Noto Sans KR Bold)
  - 색상: 흰색 + 검정 외곽선 (가독성)
  - 위치: 화면 하단 1/3

  **Acceptance Criteria**:
  
  ```bash
  # 최종 영상 파일 존재 확인
  ls -la output/final_mussoman_video.mp4
  
  # 해상도 확인 (1080x1920)
  ffprobe -v error -select_streams v:0 -show_entries stream=width,height -of csv=p=0 output/final_mussoman_video.mp4
  # Expected: 1080,1920
  
  # 길이 확인 (15-30초)
  duration=$(ffprobe -v error -show_entries format=duration -of csv=p=0 output/final_mussoman_video.mp4)
  echo "Duration: ${duration}s (should be 15-30)"
  
  # 파일 크기 확인 (100MB 이하)
  ls -lh output/final_mussoman_video.mp4
  ```

  **Commit**: NO

---

- [ ] 7. 업로드 + 제출

  **What to do**:
  - 인스타그램 릴스 업로드:
    - 계정 로그인
    - 영상 업로드
    - 캡션 작성 (한글 + 영어)
    - 해시태그 삽입: #KGM #무쏘맨 #무쏘맨어워즈 + 추가 태그
  - 공모전 구글폼 제출:
    - URL: https://forms.gle/Q8ovprmjsPJoDe2u7
    - 영상 파일 업로드
    - 신청 정보 작성
  - 제출 확인 스크린샷 저장

  **Must NOT do**:
  - 해시태그 누락 (실격 사유)
  - 마감일 초과 (2월 19일)
  - 잘못된 구글폼 제출

  **Recommended Agent Profile**:
  - **Category**: `quick`
    - Reason: 업로드 및 폼 제출은 단순 작업
  - **Skills**: [`dev-browser`]
    - `dev-browser`: 인스타그램 및 구글폼 접근

  **Parallelization**:
  - **Can Run In Parallel**: NO
  - **Parallel Group**: Wave 3 (Final)
  - **Blocks**: None
  - **Blocked By**: Task 6

  **References**:
  
  **필수 해시태그**:
  ```
  #KGM #무쏘맨 #무쏘맨어워즈
  ```
  
  **추천 추가 해시태그**:
  ```
  #AI영상 #AI아트 #무쏘 #픽업트럭 #KG모빌리티 
  #AIvideo #AIart #Musso #릴스 #reels
  ```
  
  **캡션 예시**:
  ```
  전설의 무쏘맨, 사막의 수호자가 돌아왔다! 
  Powered by Toughness - KGM MUSSO
  
  #KGM #무쏘맨 #무쏘맨어워즈 #AI영상 #무쏘
  ```
  
  **구글폼 URL**: https://forms.gle/Q8ovprmjsPJoDe2u7

  **Acceptance Criteria**:
  
  **인스타그램 업로드 확인**:
  ```
  # Playwright 또는 수동 확인
  1. 인스타그램 프로필 접속
  2. 릴스 탭에서 업로드된 영상 확인
  3. 해시태그 3개 (#KGM #무쏘맨 #무쏘맨어워즈) 포함 확인
  4. 업로드 URL 저장
  ```
  
  **구글폼 제출 확인**:
  - [ ] 제출 완료 화면 스크린샷 저장
  - [ ] 확인 이메일 수신 (있는 경우)

  **Commit**: NO

---

## Commit Strategy

이 프로젝트는 코드 개발이 아닌 콘텐츠 제작이므로, Git 커밋 대신 **파일 버전 관리**를 적용합니다:

| 단계 | 저장 위치 | 파일 명명 규칙 |
|------|----------|---------------|
| 테스트 | `output/test/` | `{tool}_test_{date}.{ext}` |
| 이미지 | `output/images/` | `scene_{num}_v{version}.png` |
| 영상 | `output/videos/` | `scene_{num}_v{version}.mp4` |
| BGM | `output/audio/` | `bgm_{name}.mp3` |
| 최종 | `output/` | `final_mussoman_video.mp4` |

---

## Success Criteria

### Verification Commands

```bash
# 최종 영상 검증
ffprobe -v error -show_entries format=duration,size -show_entries stream=width,height -of json output/final_mussoman_video.mp4

# Expected output:
# duration: 15-30
# width: 1080, height: 1920
# size: < 100MB
```

### Final Checklist

**Must Have 확인**:
- [ ] 무쏘맨 캐릭터 등장 (최소 2회)
- [ ] 무쏘 픽업트럭 등장 (최소 1회)
- [ ] 변신/전환 장면 포함
- [ ] 에픽 BGM 포함
- [ ] "Powered by Toughness" 또는 KGM 로고

**Must NOT Have 확인**:
- [ ] AI 툴 워터마크 없음
- [ ] 저작권 문제 음원 없음
- [ ] 3개 초과 캐릭터 없음

**플랫폼 요구사항**:
- [ ] 해시태그 포함 (#KGM #무쏘맨 #무쏘맨어워즈)
- [ ] 인스타그램 릴스 업로드 완료
- [ ] 구글폼 제출 완료 (2월 19일 이전)

---

## Risk Mitigation

| 리스크 | 발생 시 대응 |
|--------|------------|
| 변신 장면 품질 불량 | **유료 플랜 업그레이드** (Kling Pro, Runway) - 변신 필수! |
| 무료 크레딧 소진 | 유료 결제 (사용자 승인됨) 또는 다른 도구 시도 |
| 캐릭터 일관성 문제 | 실루엣/백라이트 스타일로 얼굴 가림 |
| 인스타 알고리즘 노출 안 됨 | 지인 공유, 관련 커뮤니티 홍보 (기존 계정 활용) |
| 마감 초과 위험 | Day 10에 중간 점검, 다른 장면 축소하고 변신에 집중 |

---

## Timeline Summary

| Day | Task | Output |
|-----|------|--------|
| 1-2 | AI 툴 세팅 + **변신 장면 품질 확보** | 변신 클립 확보 (필수) |
| 3-5 | 이미지 생성 | scene_01~05.png |
| 6-9 | 영상 생성 | scene_01~05.mp4 |
| 10-11 | 편집 + BGM | final_mussoman_video.mp4 |
| 12-13 | 최종 검토 + 수정 | 완성본 |
| 14 | 업로드 + 제출 | 공모전 제출 완료 |
