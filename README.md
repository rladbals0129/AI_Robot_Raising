# SahurRaising — 포트폴리오용 코드 스냅샷

Unity 기반 모바일 게임 **SahurRaising** 프로젝트의 **C# 게임 로직·에디터 도구**만 공개한 저장소입니다.  
이미지·모델·오디오·에셋 스토어 리소스 등은 **저작권** 때문에 포함하지 않으며, **빌드 가능한 전체 프로젝트가 아닙니다.**

## 포함 범위

| 경로 | 설명 |
|------|------|
| `SahurRaising/Assets/02. Scripts/` | 게임플레이, UI, 코어(서비스/이벤트), 데이터 테이블 정의 등 런타임 스크립트 |
| `SahurRaising/Assets/Editor/` | CSV/테이블 빌드, Addressables 설정, 스폰 패턴 에디터 등 **프로젝트 전용** 에디터 확장 |

서드파티 플러그인 소스(예: UniTask, BreakInfinity), 패키지 데모 스크립트, 에셋 팩 동봉 스크립트는 **제외**했습니다.

## 기술 스택 (참고)

- Unity 6 (`6000.0.60f1` 기준 개발)
- **UniTask** — 비동기
- **Addressables** — 리소스
- **Unity Localization**
- **DOTween**, **TextMeshPro**
- 큰 수: **BreakInfinity** (`BigDouble`)

아키텍처 요약: `ServiceLocator`, `EventBus`, `GameManager` 진입, UI는 `UI_Base` / `UIManager` 패턴.

## 사용 시 유의

- 이 레포만 클론해도 Unity에서 프로젝트가 열리지 않거나 참조가 깨질 수 있습니다. **코드 구조·구현 참고용**으로 보시면 됩니다.
- 실제 개발은 전체 프로젝트(에셋·설정·씬 포함)를 로컬에서 관리하는 것을 권장합니다.

