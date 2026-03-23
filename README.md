# 🦅 SIPE 비상(飛上) 랩: 독수리들의 프로덕트 엔지니어링

> 단순한 기능 구현(How)을 넘어, 사용자의 문제(Why)와 비즈니스 가치(What)를 조망하는 **프로덕트 엔지니어**로의 비상을 실험합니다.

## 📌 미션 소개

AI가 코드를 대신 짜주는 시대, 개발자의 가치는 어디에 있을까요?

이 미션은 기술(How)에 매몰되지 않고, 사용자의 문제(Why)와 비즈니스(What)를 고민하는 프로덕트 엔지니어로 성장하는 것을 목표로 합니다. 매주 실제 서비스를 해부하면서, 역산적 사고(Why → What → KPI → How)를 훈련합니다.

### 이런 걸 해볼 거예요

매주 하나의 실제 서비스/기능을 아래 프레임으로 깊이 파고듭니다:

- **Why**: 이 기능은 왜 존재하는가? 어떤 사용자 문제를 풀고 있는가?
- **What**: 성공을 어떻게 측정하는가? 핵심 KPI는 무엇인가?
- **How**: 왜 이 기술 스택/아키텍처를 선택했을까? 트레이드오프는?
- **What's Next**: 내가 이 제품의 Product Engineer라면 다음에 뭘 바꿀 것인가?

## 👥 참여자

| 이름 | GitHub | 직군 |
|------|--------|------|
| 배지훈 | [@G-hoon](https://github.com/G-hoon) | FE |
| 김소진 | [@sojin2](https://github.com/sojin2) | BE |
| 김수진 | [@SujinKim1127](https://github.com/SujinKim1127) | FE |
| 김지섭 | [@kimjisub](https://github.com/kimjisub) | Full-stack |
| 문상헌 | [@sanghunmoon](https://github.com/sanghunmoon) | BE |
| 문혜리 | [@haileymoon](https://github.com/haileymoon) | BE |
| 박준수 | [@GaBaljaintheroom](https://github.com/GaBaljaintheroom) | Full-stack |
| 장세은 | [@isprogrammingfun](https://github.com/isprogrammingfun) | DevOps |
| 한유진 | [@yujindonut](https://github.com/yujindonut) | DevOps |
| 홍은비 | [@do-not-do-that](https://github.com/do-not-do-that) | BE |

> 참여자 소개와 기대사항은 [members/](./members/) 폴더를 확인해주세요.

## 📅 주차별 계획

| 주차 | 주제 | 산출물 |
|------|------|--------|
| 1주차 | 킥오프 — 서로 알기 + 방향 설정 | [members/{username}.md](./members/README.md) |
| 2주차 | 사용자 플로우 역추적 | 사용자 여정 분석 문서 |
| 3주차 | 공개 데이터로 프로덕트 읽기 | 프로덕트 분석 리포트 |
| 4주차 | 개선 제안 — PRD 작성 | PRD 1편 |
| 5주차 | 도메인 깊게 파기 — 경쟁 분석 | 경쟁 분석 문서 |
| 6주차 | 최종 발표 | 프로덕트 분석 포트폴리오 |

> 주차별 상세 내용은 각 `week-N/README.md`를 확인해주세요.
> 주차별 계획은 참여자들과 OT에서 조율하여 확정할 예정입니다.

## 🔧 참여 방법

### 1. Clone

```bash
git clone https://github.com/sipe-team/5-1_sipe_product_engineering_lab.git
cd 5-1_sipe_product_engineering_lab
```

### 2. 브랜치 생성 + 산출물 작성

```bash
# 예: members 자기소개 작성
git checkout -b members/{your-github-username}

# members/ 폴더에 본인 파일 생성
# 예: members/treejy.md

# 예: 주차별 산출물 작성
git checkout -b week-2/{your-github-username}

# 해당 주차 폴더에 본인 파일 생성
# 예: week-2/treejy.md
```

### 3. PR 제출

```bash
git add .
git commit -m "members: treejy 자기소개"
git push origin members/{your-github-username}
# GitHub에서 main 브랜치로 PR 생성
```

## 📝 PR 컨벤션

- **PR 제목**: `[members] {github-username}` 또는 `[week-2] {github-username}`
- **브랜치명**: `members/{github-username}` 또는 `week-2/{github-username}`
- **base 브랜치**: `main`

## 🤝 리뷰 규칙

1. 서로의 산출물에 코멘트를 남깁니다 — 질문, 다른 관점, 공감 모두 환영
2. "왜 그렇게 판단했는지"에 집중합니다
3. 정답이 없는 만큼, 다양한 시각을 존중합니다

## 📚 참고 자료

> 자세한 참고 자료는 [references/](./references/) 폴더를 확인해주세요.

**한국어**
- [당근 블로그 — "프로덕트에 진심인 엔지니어는 어떻게 일할까?" 1편](https://about.daangn.com/blog/archive/%EB%8B%B9%EA%B7%BC-%EA%B0%9C%EB%B0%9C%EC%9E%90-%EB%AA%A9%EC%A0%81%EC%A1%B0%EC%A7%81-%ED%94%84%EB%A1%9C%EB%8D%95%ED%8A%B8-%EC%97%94%EC%A7%80%EB%8B%88%EC%96%B4/)
- [당근 블로그 — "프로덕트에 진심인 엔지니어는 어떻게 일할까?" 2편](https://about.daangn.com/blog/archive/%EB%8B%B9%EA%B7%BC-%EA%B0%9C%EB%B0%9C%EC%9E%90-%ED%94%84%EB%A1%9C%EB%8D%95%ED%8A%B8-%EC%97%94%EC%A7%80%EB%8B%88%EC%96%B4-%ED%8C%80%EB%B9%8C%EB%94%A9-%ED%9A%8C%EA%B3%A0/)
- [요즘IT — "개발자는 왜 이제 프로덕트 엔지니어가 되어야 할까?"](https://yozm.wishket.com/magazine/detail/3418/)
- [요즘IT — "AI시대에 필요한 개발자, Product Engineer"](https://yozm.wishket.com/magazine/detail/2485/)
- [GeekNews — "프로덕트 엔지니어(The Product Engineer)"](https://news.hada.io/topic?id=22833)
- [역산적 사고 — 아마존의 Working Backward](https://flex.team/blog/2024/08/22/amazon-working-backward/)

**영어**
- [Sherif Mansour — "Product Engineers" (Atlassian, 2019)](https://medium.com/atlassian-product-management-blog/product-engineers-51af415bd1d4)
- [Daniel Bentes — "The AI Product Engineer" (2026)](https://medium.com/@danielbentes/the-ai-product-engineer-0f02d7f08590)
- [PostHog — "Finding a job as a product engineer"](https://posthog.com/newsletter/finding-a-job-product-engineer)
