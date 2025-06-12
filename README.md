# 📝 To-Do List 웹 애플리케이션

## 📌 프로젝트 소개

이 프로젝트는 간단한 **To-Do List 웹 애플리케이션**으로, HTML/CSS/JavaScript를 사용해 제작되었습니다. 사용자는 할 일을 추가, 수정, 삭제, 완료 체크 등의 기능을 사용할 수 있으며, Git을 적극적으로 활용하여 **브랜치 전략, 커밋 이력 관리, cherry-pick 등 Git 기능**을 실습하기 위한 학습 목적의 프로젝트입니다.

## 🔧 주요 기능

### 1. 할 일 추가

* 텍스트 입력 후 Enter를 누르면 리스트에 항목이 추가됨.

### 2. 할 일 완료 체크

* 체크박스를 클릭하면 해당 항목이 회색 처리되고 텍스트에 취소선이 생김.
* 완료 여부는 리로딩 시에도 유지됨 (`localStorage` 사용).

### 3. 할 일 수정

* 텍스트를 클릭하면 수정 모드로 전환되어 입력창에서 내용 수정 가능.
* Enter 또는 blur 이벤트 시 저장됨.

### 4. 할 일 삭제

* 항목 옆의 빨간 x 버튼을 누르면 해당 항목이 삭제됨.

## 💡 Git 전략 및 사용 내용

### 📂 브랜치 구성

* `main` : 배포용 메인 브랜치
* `feature/edit-mode` : 수정 기능 개발 브랜치
* `feature/checkbox-persist` : 체크박스 상태 영속성 추가 브랜치

### 🔀 사용된 Git 기능

* **기능별 브랜치 분리**: 각 기능은 독립된 브랜치에서 개발
* **cherry-pick**: `feature/edit-mode`에서 개발된 수정 기능을 다른 브랜치에 부분 반영함
* **merge**: 모든 기능이 완료된 후 `main` 브랜치로 병합
* **commit log 관리**: 명확한 메시지로 각 기능 단위별 커밋 기록 작성

### 예시 커밋 메시지

```
feat: add checkbox complete toggle with persistence
fix: edit mode reverted to display mode on blur
refactor: unify todo item structure
```

## 💻 실행 방법

### 1. 프로젝트 클론

```bash
git clone https://github.com/사용자명/저장소명.git
cd 저장소명
```

### 2. 실행

* VS Code에서 `index.html` 파일을 브라우저로 열면 실행됨
* 또는 `Live Server` 확장 프로그램을 사용해 실행 가능

---

## 🙋‍♂️ 프로젝트 목적 및 활용

본 프로젝트는 Git을 실전처럼 체험하고자 하는 **학습 중심의 실습 프로젝트**입니다. 다양한 브랜치 전략 및 커밋 기록을 남기며 협업 및 버전 관리를 훈련할 수 있습니다.

---

## 📎 기타 정보

* 개발자: Jaewoong Lee
* 주요 기술: HTML, CSS, JavaScript, Git/GitHub
* 저장소 링크: [https://github.com/사용자명/저장소명](https://github.com/사용자명/저장소명)
