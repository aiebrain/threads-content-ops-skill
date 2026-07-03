# Threads 콘텐츠 운영 스킬

Threads 콘텐츠를 단순히 많이 쓰는 방식이 아니라, **사람 승인 → 발행 → 실제 게시 확인 → 댓글/DM 분석 → 다음 글 조절**까지 반복 가능한 운영 루프로 관리하기 위한 공개용 Hermes Skill입니다.

이 저장소는 자동 스팸 발행이나 무작위 대량 게시 도구가 아닙니다. 크리에이터, 교육자, 1인 사업자, 콘텐츠 운영자가 짧은 글 SNS를 작은 운영 시스템처럼 관리할 수 있도록 만든 공개 배포용 워크플로입니다.

## 이브레인 YouTube

이 구조를 만든 이브레인의 AI 커머스/자동화 콘텐츠는 아래 채널에서 볼 수 있습니다.

- YouTube: [AI 커머스 브레인 - 이브레인](https://www.youtube.com/@aiebrain)

## 전체 운영 흐름

```text
리서치 / 계정 성과 확인
→ 후보 글 3개 작성
→ 사람 승인
→ 승인된 글만 발행
→ 실제 게시물 검증
→ 댓글 / DM / 반응 분석
→ 다음 글 조절
→ 운영 기록 저장
```

## 왜 이 구조가 필요한가

많은 콘텐츠 운영은 보통 여기서 끝납니다.

```text
아이디어
→ 글쓰기
→ 발행
→ 끝
```

이 방식은 매번 처음부터 다시 시작하게 만듭니다. 댓글에서 나온 질문이 다음 글로 이어지지 않고, 어떤 글이 실제로 리드나 문의를 만들었는지도 남지 않습니다. 또 발행 전에 사람의 승인 단계가 없으면, 계정 톤과 다른 글이 올라가거나 검증되지 않은 자동 발행이 발생할 수 있습니다.

이 스킬은 Threads 운영을 다음과 같은 피드백 루프로 바꿉니다.

```text
쓰기
→ 승인
→ 발행
→ 확인
→ 학습
→ 다음 글 조절
```

## 이 스킬이 하는 일

이 스킬은 Hermes Agent가 다음 과정을 일관되게 수행하도록 돕습니다.

1. 현재 계정 상황과 이전 반응을 확인합니다.
2. 공개적으로 참고 가능한 벤치마크 글의 구조를 분석합니다.
3. 댓글, DM, 자료 요청, 상담 문의 등 하나의 비즈니스 연결 경로를 정합니다.
4. 서로 다른 각도의 후보 글을 여러 개 작성합니다.
5. 사용자의 명시적 승인을 기다립니다.
6. 승인된 글만 발행합니다.
7. 발행 후 실제 URL과 답글 세그먼트를 확인합니다.
8. 댓글, DM, 반응의 질을 분석합니다.
9. 결과에 따라 다음 글의 훅, CTA, 길이, 주제를 조절합니다.
10. 운영 기록을 남깁니다.

## 핵심 운영 모델

### 1. 리서치와 성과 확인

글을 쓰기 전에 세 가지 관점으로 확인합니다.

| 관점 | 확인할 내용 |
|---|---|
| 외부 벤치마크 | 훅, 대비 구조, CTA, 글 길이, 답글 구성 |
| 내 계정 반응 | 조회수, 유효 댓글, 저장/공유, 반복 질문 |
| 비즈니스 경로 | 댓글, DM, 자료 요청, 상담, 상품/서비스 질문 |

중요한 것은 바이럴 글을 그대로 베끼는 것이 아니라, **작동한 구조만 추출하는 것**입니다.

### 2. 후보 글 작성

한 번에 최종 글 하나만 만들지 않습니다. 서로 다른 목적과 스타일의 후보 글을 여러 개 준비합니다.

각 후보 글에는 다음 항목을 포함합니다.

```text
후보 번호
제목
스타일
목적
비즈니스 연결 경로
예상 성공 신호
참고한 구조
승인 요청 문구
본문
작성자 답글 / 확장 답글
```

사용 가능한 스타일 예시:

- 짧은 인사이트
- 문제 진단
- 실제 업무 예시
- 체크리스트
- 반대 관점
- 대화형 기록
- 댓글 유도형 질문
- 미니 스토리
- Before / After
- 초보자용 미니 레슨

### 3. 사람 승인 게이트

초안 작성은 발행이 아닙니다. 이 스킬의 핵심은 **사람 승인 전 발행 금지**입니다.

승인 예시는 다음과 같습니다.

```text
1번 후보 승인
첫 번째 글 지금 발행
세 개 모두 승인
1번만 발행하고 나머지는 반응 보고 조절
```

운영 규칙:

- 명시적 승인 전에는 발행하지 않습니다.
- 승인된 글만 발행합니다.
- 뒤 글이 앞 글의 반응에 따라 달라지는 경우, 너무 일찍 확정하지 않습니다.

### 4. 발행 구조

여러 개의 답글로 이어지는 Threads 글은 세그먼트로 나눕니다.

예시:

```text
1/3 핵심 문제 또는 인사이트
2/3 예시 또는 설명
3/3 구체적 CTA 또는 질문
```

발행 전에는 검증용 고유 문구를 정리합니다.

```json
{
  "segments": [
    "메인 글 텍스트",
    "작성자 답글 텍스트",
    "CTA 답글 텍스트"
  ],
  "sentinels": [
    "메인 글의 고유 문구",
    "작성자 답글의 고유 문구",
    "CTA 답글의 고유 문구"
  ]
}
```

### 5. 실제 게시 검증

발행 버튼을 눌렀다고 작업이 끝난 것이 아닙니다.

반드시 확인할 항목:

- 새 canonical URL이 생성되었는지
- 프로필 또는 피드에 새 훅이 보이는지
- 기대한 `1/N` 답글 구조가 보이는지
- 필요한 경우 숨겨진 답글을 펼쳐 확인했는지
- 마지막 CTA가 누락되지 않았는지
- 끝부분 세그먼트가 중복되거나 빠지지 않았는지

단순히 URL을 받았거나 버튼을 눌렀다는 사실만으로 완료 처리하지 않습니다.

### 6. 댓글과 DM 분석

반응은 단순 조회수보다 질을 우선합니다.

우선순위는 다음과 같습니다.

```text
적격 연락 / DM / 문제 진술
> 상품 또는 서비스 질문
> 유효 댓글
> 저장 / 공유
> 팔로우
> 조회수
```

유효 댓글은 단순 참여가 아니라 다음 글의 재료입니다.

예시:

```text
댓글 질문
→ 짧은 답변
→ 같은 질문이 반복되면 초보자용 후속 글 작성
```

### 7. 결과 기반 조절

첫 글의 결과에 따라 다음 글을 조절합니다.

| 상황 | 조절 방식 |
|---|---|
| 반응이 강함 | 같은 주제를 확장 |
| 조회수는 있는데 댓글이 없음 | CTA를 더 구체적으로 변경 |
| 답글까지 읽히지 않음 | 핵심 내용을 메인 글로 이동 |
| 기초 질문이 등장 | 초보자용 후속 글 작성 |
| DM 또는 상품 질문 등장 | 관련 자료, 제안, 상담 흐름으로 연결 |

## Hermes에 설치하는 방법

저장소를 클론합니다.

```bash
git clone https://github.com/aiebrain/threads-content-ops-skill.git
```

Hermes skills 디렉터리로 복사합니다.

```bash
mkdir -p ~/.hermes/skills/social-media
cp -R threads-content-ops-skill/skills/social-media/threads-content-ops ~/.hermes/skills/social-media/
```

설치 확인:

```bash
hermes skills list | grep threads-content-ops
```

또는 Hermes 내부에서 직접 불러옵니다.

```text
skill_view(name="threads-content-ops")
```

## 패키지 구성

```text
README.md
LICENSE
skills/social-media/threads-content-ops/SKILL.md
skills/social-media/threads-content-ops/references/public-workflow.md
skills/social-media/threads-content-ops/templates/daily-approval-request.md
skills/social-media/threads-content-ops/templates/publish-log.md
```

## 템플릿

### 일일 승인 요청 템플릿

경로:

```text
skills/social-media/threads-content-ops/templates/daily-approval-request.md
```

후보 글 3개, 선정 기준, 비즈니스 연결 경로, 예상 성공 신호, 승인 선택지를 정리하는 템플릿입니다.

### 발행 기록 템플릿

경로:

```text
skills/social-media/threads-content-ops/templates/publish-log.md
```

승인 여부, 발행 시간, canonical URL, 세그먼트 검증, visible metrics, 유효 댓글, 다음 글 조절 방향을 기록하는 템플릿입니다.

## 공개 배포 기록

```text
Repository: aiebrain/threads-content-ops-skill
URL: https://github.com/aiebrain/threads-content-ops-skill
Visibility: PUBLIC
Default branch: main
Initial public commit: 537d315 Add public Threads content ops skill
README Korean update: 이 커밋 이후 README를 한글 중심으로 업데이트
YouTube: https://www.youtube.com/@aiebrain
```

## 공개 공유 전 안전 체크리스트

이 워크플로를 공유하거나 변형할 때는 다음 항목을 제거하거나 일반화해야 합니다.

- 개인 로컬 경로
- 비공개 채널 ID
- 브라우저 프로필명
- 내부 자동화 endpoint
- 비공개 계정 운영 정보
- API key, token, cookie, password
- 고객, 수강생, 클라이언트 정보
- 아직 공개하지 않은 사업 전략

## 안전 원칙

- 발행 전 사람 승인 게이트를 유지합니다.
- 민감하거나 비공개인 정보는 발행하지 않습니다.
- access token, cookie, API key, password를 로그에 저장하지 않습니다.
- 브라우저 자동화는 본인 계정 또는 정당하게 권한을 받은 계정에서만 사용합니다.
- 발행 후 실제 게시물을 검증합니다.
- 외부 공유 시에는 공개 가능한 예시만 사용합니다.

## 한 줄 요약

```text
Threads 운영은 글을 많이 쓰는 일이 아니라, 반응을 기록하고 다음 글을 조절하는 작은 콘텐츠 운영 시스템입니다.
```

## 라이선스

MIT
