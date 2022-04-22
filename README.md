# hardlink
## 발상
- 하드링크를 이용해 같은 코드를 여기저기 놔두는 방식으로 개발하면 어떨까

- 비즈니스 로직에 따라 관련 있는 파일들을 하나의 디렉토리에 몰아넣는다.
- 중복된 파일이 분명히 생길텐데 이 경우 하드 링크로 연결한다.

- 연관성을 찾기 위해 파일을 찾아다닐 필요 없이 하나의 디렉터리 안에서 모든 개발을 진행한다.

## 예상되는 문제점
- cycle이 생길 수 있다.
  - 원본 파일은 하나의 디렉터리에 모아두고 하드링크만 가지고 코딩을 진행하면 어떨까?

- import가 제대로 안 될 수 있다.
  - 빌드 시 바벨처럼 적절히 수정하는 코드를 작성한다.

- 코드가 무거워진다.
  - 배포 시 적절히 수정한다.
  - 사실 코드가 몇 배 불어난다고 성능에 큰 이슈가 생길 것 같진 않다.
