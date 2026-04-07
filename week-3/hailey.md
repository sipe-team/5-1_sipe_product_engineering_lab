# 3주차: 공개 데이터로 프로덕트 읽기

## 분석 대상

- **서비스**: Duolingo
- **분석한 기능**: Streak (연속 학습일)
- **서비스 유형**: B2C 앱

---

## 2주차에서 발견한 페인포인트

1. **Streak 소멸 → 재진입 장벽**: 한 번 깨지면 다시 돌아가기 싫어진다
2. **Streak 유지 → 학습 품질 저하**: streak을 지키려고 최소한의 레슨만 하게 된다
3. **Streak Freeze 남용 → 학습 동기 희석**: 안 들어가도 streak이 살아있으니까 오히려 더 안 들어가게 된다

---

## 공개 데이터 분석

- **사용한 소스**: Google Play 리뷰, Medium/블로그 아티클 (실제 장기 사용자 경험담)
- **소스 선정 이유**: 수백 일 streak 보유 후 이탈한 유저들의 1인칭 서술이 페인포인트 검증에 가장 직접적
- **분석한 피드백 수**: 약 30개 이상 (리뷰 + 아티클)

### 내 페인포인트와 겹치는 피드백

**페인포인트 1: Streak 소멸 → 재진입 장벽**

> "streak이 깨지면 streak도 잃고 습관도 동시에 잃는다. 점진적으로 그만두는 게 아니라 한꺼번에 그만두는 구조다" — mysenpai.com

> "두 번 streak을 잃고 나서 그냥 포기했다" — italianlg.com (터키어 교사)

> "350일 마일스톤을 찍고 사진까지 저장했는데 다음날 349일로 되어있고 어제 학습을 빠졌다고 해서 매우 매우 억울했다" — Google Play 한국어 리뷰

→ 이탈이 점진적이 아니라 streak 소멸 시점에 한꺼번에 발생하는 구조.

**페인포인트 2: Streak 유지 → 학습 품질 저하**

> "streak을 지키려고 42초 만에 레슨을 끝내고 나온 적도 있다. streak이 학습을 보장하는 게 아니라 앱 접속만 보장한다" — Android Authority (550일 유저)

> "628일 동안 streak을 지키려고 보석만 소모했다. 언어 학습이 아니라 디지털 축적에 불과했다" — arttu.net

> "1,500일 streak이 있지만 솔직히 요즘은 초반 레슨만 반복한다. 사실상 아무것도 배우지 않는다" — Medium (Eric Ravenscraft)

> "독일어를 배우려고 시작했는데 결국 streak을 유지하려고 이미 배운 레슨만 반복하게 됐다" — sereneluna.net (588일 유저)

→ 장기 유저일수록 "streak 지키기"가 목적이 되고 학습은 수단으로 전락하는 패턴이 반복적으로 등장.

**페인포인트 3: Streak Freeze 남용 → 학습 동기 희석**

> "streak freeze를 너무 많이 줘서 pay-to-win처럼 느껴진다. 몇 달 전에 이미 잃었어야 할 streak이 계속 살아있다" — Android Authority (550일 유저)

> "streak freeze가 문제를 해결하는 게 아니라 이탈을 지연시킬 뿐이다" — Medium (480일 유저)

→ "안 들어가도 streak이 살아있으니까 오히려 더 안 들어가게 됨" — Streak Freeze가 이탈 방지 도구로 설계됐지만 오히려 학습 동기를 희석시키는 역효과.

### 추가로 발견한 페인포인트

- **외적 동기가 내적 동기를 대체**: streak이 길어질수록 "배우고 싶어서"가 아니라 "streak 지키려고" 앱을 여는 구조로 전환됨. 외적 보상이 내적 동기를 밀어내는 crowding-out 효과.
- **streak 소멸 = 학습 포기**: streak이 곧 학습 습관과 동일시되기 때문에, streak 소멸 시 학습 자체를 포기하는 경우가 많음. 숫자가 리셋되는 순간 "처음부터 다시"라는 심리적 부담이 생김.

### 피드백 트렌드

- 2021~2025년까지 동일한 불만이 반복적으로 등장 → 듀오링고가 인지하고 있지만 근본적으로 해결하지 못하고 있는 구조적 문제
- Streak Freeze, Monthly Streak Repair 등 패치를 지속적으로 추가했지만 "근본 문제를 지연시킬 뿐"이라는 평가가 반복됨
- 최근(2024~2025) 피드백에서 Super 유료 전환 압박과 streak 문제가 함께 언급되는 경우가 늘어남

---

## 기업 공개 정보

### 기술 블로그

- **"How Streaks keep Duolingo learners committed"** ([링크](https://blog.duolingo.com/how-streaks-keep-duolingo-learners-committed-to-their-language-goals/))
  - Streak Wager A/B 테스트에서 Day-7 retention +14% 달성
  - Weekend Amulet 도입 → streak 소멸률 5% 감소, 1주일 후 재방문율 4% 증가
  - → 회사가 streak 소멸로 인한 이탈을 실제 KPI 문제로 인식하고 있다는 직접적 근거

- **"Improving the streak: Forming habits one lesson at a time"** ([링크](https://blog.duolingo.com/improving-the-streak/))
  - streak과 daily goal을 분리하는 구조 변경 → Day 14 retention +3.3%, 7일+ streak 유저 비율 +10.5%
  - "intense 목표를 설정한 유저 중 40%가 매일 사용해도 streak이 없었다" → 구조적 문제를 발견하고 패치한 사례
  - → 회사가 streak 설계를 지속적으로 개선 중이라는 신호

- **"The Duolingo Streak Uses Habit Research"** ([링크](https://blog.duolingo.com/how-duolingo-streak-builds-habit/))
  - **"streak을 잃으면 오히려 demotivating할 수 있다"고 공식 블로그에서 직접 인정**
  - → 페인포인트 1("한 번 깨지면 돌아가기 싫다")을 회사도 인지하고 있음을 확인

### 채용 공고 / PM 인터뷰

- Duolingo Retention Team PM인 Jackson Shuttleworth가 공개 인터뷰에서 직접 언급:
  - "streak이 너무 쉽게 접근 가능하면 가치가 없어진다. 동시에 streak을 잃으면 retention이 급격히 떨어진다" — 딜레마를 회사 내부에서도 인식
  - streak 최적화를 위해 **600회 이상의 A/B 테스트** 진행
  - → 이 딜레마를 해결하려는 엔지니어링 투자가 지속되고 있다는 신호

### 앱 업데이트 기록 (streak 관련)

- Streak Freeze 도입 → 이탈 방지 시도
- Weekend Amulet 도입 → 주말 streak 소멸 완화
- Monthly Streak Repair (Super 전용) → 유료 전환 유도와 이탈 방지 결합
- Streak Wager 도입 → 7일 달성 보상으로 초기 이탈 방지
- → 패치가 반복된다는 것 자체가 "streak 소멸 → 이탈" 문제가 해결되지 않았다는 신호

---

## 종합 판단

> 이 기능은 **부분적 성공 / 구조적 딜레마 상태**이다.
>
> **근거:**
> 1. Streak은 단기 retention에는 강력하게 작동한다. Duolingo 내부 데이터에서 7일 streak 유저는 코스 완료 확률이 3.6배 높고, 2024년 DAU 3,700만 명 달성의 핵심 동력
> 2. 그러나 장기 유저에서 일관되게 "학습 품질 저하 → 동기 희석 → 한꺼번에 이탈"하는 패턴이 반복됨
> 3. Streak Freeze는 이탈을 막으려는 시도였지만, 오히려 학습 동기를 희석시키는 역효과를 낳고 있음
>
> **핵심 딜레마:**
> Streak은 Duolingo의 가장 강력한 retention 도구인 동시에, 장기 이탈의 트리거이기도 하다. 단기 DAU를 높이는 설계가 장기 학습 동기를 갉아먹는 구조적 모순.
>
> **한계:**
> - 공개 데이터는 이탈한 유저 중심 — 계속 사용 중인 유저의 목소리가 상대적으로 적어 편향이 있을 수 있음
> - Streak 소멸 후 실제 이탈률 수치는 외부 데이터로 확인 불가

---

## (선택) 내가 PM이라면 다음에 뭘 할 것인가?

Streak의 구조적 딜레마를 해결하려면 "숫자 보호"가 아니라 "학습 동기 재점화"에 집중해야 한다.

- **Streak 소멸 후 재진입 온보딩 설계**: 0으로 리셋되는 대신 "지난 학습 기록"을 시각화해서 "처음부터 다시"라는 심리적 부담을 낮춤. 숫자가 아니라 누적 학습량으로 동기를 부여.
- **Streak Freeze → 학습 목표 기반으로 전환**: 단순 접속이 아니라 "이번 주 목표 달성 여부"로 streak 유지 조건을 바꿈. 42초짜리 레슨으로 streak을 유지하는 구조를 막고 실질 학습과 연동.
- **장기 유저 감지 후 개입**: 반복 레슨 비율이 높아지면 "새로운 챕터 도전" 알림을 보내 학습 깊이를 유도. streak 숫자가 아니라 실제 진도가 retention 지표가 되도록.

---

## 참고 자료

- [Why it might be time to give up my 550+ day Duolingo streak — Android Authority](https://www.androidauthority.com/reasons-give-up-duolingo-streak-3543009/)
- [I Think It's Time to Give Up My Duolingo Streak — Medium (Eric Ravenscraft)](https://debugger.medium.com/i-think-its-time-to-give-up-my-duolingo-streak-81c27ff1be8b)
- [Why I let go of my ~480 day Duolingo streak — Medium (Saunved)](https://saunved.medium.com/why-i-let-go-of-my-480-day-duolingo-streak-a2098b3eff35)
- [Why I Quit Duolingo After a 588 Day Streak — Medium (Diana Craciun)](https://medium.com/babel/why-i-quit-duolingo-after-a-588-day-streak-dd38de2d8d79)
- [10 Reasons I Stopped Using Duolingo in 2025 — arttu.net](https://arttu.net/blog/top-10-reasons-why-i-stopped-grinding-duolingo/)
- [Why People Quit Duolingo — my-senpai.com](https://my-senpai.com/insights/why-people-quit-duolingo.html)
- [Why I'm Quitting Duolingo — sereneluna.net](https://sereneluna.net/2024/06/10/why-im-quitting-duolingo/)
- [듀오링고(Duolingo) Google Play 리뷰](https://play.google.com/store/apps/details?id=com.duolingo&hl=ko)
