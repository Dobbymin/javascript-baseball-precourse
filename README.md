# 숫자 야구 기능 구현 목록

## 페이지 디자인 구현

- [ ] 기본적인 디자인 구현
- [ ] 각 태그별 적절한 class와 id 작성
- [ ] 처음 게임 시작 시 '결과' 부분 숨기기

## 야구게임 결과

### 1. 정답일때

- [ ] '🎉정답을 맞추셨습니다🎉' 문구 출력
- [ ] 게임 재시작 문구 출력
- [ ] 게임 재시작 버튼 생성

### 2. 정답이 아닐때

- [ ] '❌정답이 아닙니다❌' 문구 출력

### 3. 잘못된 값 입력했을 때

- [ ] `alert()` 으로 **에러메시지** 출력

### 예외 case 종류

1. 문자열 입력
2. 특수문자 입력
3. 소수 입력
4. 중복된 숫자 입력
5. 3개 이상 또는 이하의 숫자 입력
6. 숫자 0 입력

## 기능 구현

### 숫자 입력 받기

1. input창에 숫자 입력
2. 확인 button 클릭 시 input창의 숫자 전달받기
3. try-catch문을 이용하여 예외 case 찾기

- 예외 case에 해당하는 입력 받을경우 에러메시지 출력

### 게임 진행

1. random 함수를 이용해 임의의 상대방의 수 생성
2. 입력받은 수와 상대방의 수를 비교

- 같은 수, 같은자리 = 스트라이크
- 같은 수, 다른자리 = 볼
- 모두 다른 수 = 낫싱

```
e.g.
상대방(컴퓨터)의 수가 425일 때,
- 123을 제시한 경우: 1스트라이크
- 456을 제시한 경우: 1볼 1스트라이크
- 789를 제시한 경우: 낫싱
```

### 게임 결과 출력

1. 정답일때

- 정답 문구 및 게임 재시작 버튼 보여주기

2. 정답이 아닐때

- 틀렸다는 문구 보여주기
