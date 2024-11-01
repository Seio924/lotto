# javascript-lotto-precourse

# 💰 로또 발매기 기능 구현 목록

## 사용자 입력

- [x] 로또 구입 금액을 입력 받는다.

  - ❌ 예외 처리
    - [x] 1,000원으로 나누어 떨어지지 않는 경우 예외 처리한다. [ '[ERROR] 구입 금액은 1,000원으로 나누어 떨어져야 합니다.' ]
    - [x] 입력하지 않은 경우 예외 처리한다. [ '[ERROR] 구입 금액을 입력해야 합니다.' ]
    - [x] 숫자가 아닐 경우 예외 처리한다. [ '[ERROR] 구입 금액은 숫자여야 합니다.' ]

- [x] 당첨 번호를 입력 받는다. (번호는 쉼표(,)를 기준으로 구분한다.)

  - ❌ 예외 처리
    - [x] 입력한 당첨 번호에 중복이 있을 경우 예외 처리한다. [ '[ERROR] 중복된 당첨 번호가 있습니다.' ]
    - [x] 입력한 당첨 번호가 1~45가 아닌 경우 예외 처리한다. [ '[ERROR] 당첨 번호는 1~45 사이여야 합니다.' ]
    - [x] 입력하지 않은 경우 예외 처리한다. [ '[ERROR] 당첨 번호를 입력해야 합니다.' ]
    - [x] 숫자가 아닐 경우 예외 처리한다. [ '[ERROR] 당첨 번호는 숫자여야 합니다.' ]
    - [x] 입력한 당첨 번호가 6개가 아닌 경우 예외 처리한다. [ '[ERROR] 당첨 번호는 반드시 6개여야 합니다.' ]

- [x] 보너스 번호를 입력 받는다.
  - ❌ 예외 처리
    - [x] 입력한 보너스 번호가 중복일 경우 예외 처리한다. [ '[ERROR] 보너스 번호는 당첨 번호와 중복될 수 없습니다.' ]
    - [x] 입력한 보너스 번호가 1~45 범위를 벗어날 경우 예외 처리한다. [ '[ERROR] 보너스 번호는 1~45 사이여야 합니다.' ]
    - [x] 입력하지 않은 경우 예외 처리한다. [ '[ERROR] 보너스 번호를 입력해야 합니다.' ]
    - [x] 숫자가 아닐 경우 예외 처리한다. [ '[ERROR] 보너스 번호는 숫자여야 합니다.' ]
    - [x] 입력한 보너스 번호가 1개가 아닌 경우 예외 처리한다. [ '[ERROR] 보너스 번호는 반드시 1개여야 합니다.' ]

## 로또 발매기

- [x] 1~45 사이의 중복되지 않는 6개의 숫자를 뽑는다.
- [x] 구입 금액에 해당하는 만큼 로또를 발행한다.

## 결과 계산

- [x] 당첨 내역을 계산한다.
- [ ] 총 수익률을 계산한다.

## 결과 출력

- [ ] 발행한 로또의 번호 생성 결과를 출력한다.
- [ ] 당첨 통계를 출력한다.
- [ ] 총 수익률을 출력한다.

# 💰 로또 발매기 실행 결과

```
구입금액을 입력해 주세요.
8000

8개를 구매했습니다.
[8, 21, 23, 41, 42, 43]
[3, 5, 11, 16, 32, 38]
[7, 11, 16, 35, 36, 44]
[1, 8, 11, 31, 41, 42]
[13, 14, 16, 38, 42, 45]
[7, 11, 30, 40, 42, 43]
[2, 13, 22, 32, 38, 45]
[1, 3, 5, 14, 22, 45]

당첨 번호를 입력해 주세요.
1,2,3,4,5,6

보너스 번호를 입력해 주세요.
7

당첨 통계
---
3개 일치 (5,000원) - 1개
4개 일치 (50,000원) - 0개
5개 일치 (1,500,000원) - 0개
5개 일치, 보너스 볼 일치 (30,000,000원) - 0개
6개 일치 (2,000,000,000원) - 0개
총 수익률은 62.5%입니다.
```
