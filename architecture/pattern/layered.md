## 한국어

Q1. 레이어드 아키텍처란?

- 계층별로 책임을 나누어, 각 계층이 상하 관계를 가지며 동작하는 아키텍쳐

Q2. 계층 구조

1. 인터페이스 계층 (Presentation Layer)
    - UI 처리, API 요청/응답 처리를 담당한다. (Controller)
2. 애플리케이션 계층 (Application Layer)
    - 도메인 로직을 호출하는 서비스 계층 (Service)
3. 도메인 계층 (Domain Layer)
    - 핵심 비즈니스 규칙과 로직을 담당한다. (Entity, Domain Service)
4. 인프라 계층 (Infrastructure Layer)
    - DB, 외부 API 등 구현 세부사항 처리 (Repository 구현체)

Q3. 레이어드 아키텍처의 장점은?

- 단순한 구조로 빠른 개발이 가능하다.
- 각 계층의 역할이 명확하여, 기본적인 분리와 유지보수가 가능하다.

Q4. 레이어드 아키텍처의 단점은?

- 도메인이 서비스나 DB에 의존하기 쉽다.
- 하위 계층 변경이 상위 계층에 영향을 미친다.
- DB 설계에 대한 의존성이 커, 유연한 변경이 어렵다.
- 도메인만 따로 분리해서 테스트하기가 어렵다.

요약

- 단순하고 빠르게 개발할 수 있다는 장점이 있지만, 도메인의 독립성이 약하여 규모가 커지면 유지보수가 힘들어질 수 있다는 단점이 있다.

---

## 日本語

Q1. レイヤードアーキテクチャとは？

- レイヤーごとに責任を分担し、それぞれが上下関係を持って動作するアーキテクチャです。

Q2. レイヤー構造

1. プレゼンテーションレイヤー
    - UI処理、APIのリクエスト・レスポンスの処理を担当します。(Controller)
2. アプリケーションレイヤー
    - ドメインロジックを呼び出すサービスレイヤーです。(Service)
3. ドメインレイヤー
    - 主要なビジネスルールやロジックを担当します。(Entity, Domain Service)
4. インフラレイヤー
    - DB, 外部APIなど実装の詳細部分を処理します。(Repositoryの実装クラス)

Q3. レイヤードアーキテクチャの長所は？

- シンプルな構造で、早い開発ができます。
- 各レイヤーの役割が明確で、基本的な分離や保守がしやすいです。

Q4. レイヤードアーキテクチャの短所は？

- ドメインがサービスやDBに依存しやすくなります。
- 下位レイヤーの変更が上位レイヤーに影響を与えます。
- DBの設計への依存度が高く、柔軟な変更が難しいです。
- ドメイン単体分離してテストすることが難しいです。

要約

- シンプルで迅速な開発ができる長所がありますが、ドメインの独立性が弱くて規模が大きくなると保守が難しくなる短所があります。