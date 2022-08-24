### 1. HTML 요소가 어떻게 화면에 자리를 차지할지 정해주는 역할

#### 1) none

- 요소가 눈에 보이지 않고, 자리를 차지하지도 않아서 렌더링 parsing 단계에서도 아예 무시됨

#### 2) inline

- 콘텐츠 크기만큼만 자리를 차지하기 때문에, 요소들끼리 한줄로 나란히 배치되어 보임
- width, height 속성을 지정해도 무시됨
- margin, padding 속성은 좌우만 반영되고 상하 간격은 반영되지 않음
- 가운데 정렬 text-align: center
- `span`, `strong`, `a`, `img`

#### 3) block

- 콘텐츠 크기와 상관없이 한 줄을 모두 차지하고 있어 줄바꿈이 일어남
- width, height, marign, padding 모두 정상적으로 작동
- 가운데 정렬 margin: 0 auto
- `div`, `h1`, `p`, `li`, `section`

#### 4) inline-block

- 외부는 inline, 내부적으로는 block요소를 따르는 것
- iline처럼 한 줄에 나란히 배치되지만, block 요소처럼 width, height, marign, padding 모두 정상적으로 적용됨
- `button`, `input`, `select`

---

### 2. 자식 요소를 배치하여 레이아웃 설정

#### 1) flex

- 부모 요소(컨테이너) 아래에서 자식 요소(아이템)들이 한 방향으로 배치
- 다양한 속성을 통해 자식 요소 사이를 일정한 간격으로 줄 수 있고 정렬하기가 매우 편리

#### 2) grid

- 행과 열, 두 가지 방향으로 배치가 가능하기 때문에 어렵고 복잡한 매트릭스 레이아웃 작성에 용이
