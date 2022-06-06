# IntelliJ 단축키  for Mac

## 기호 의미
|기호| 의미     |
|---|--------|
| ⇧ |  Shift |
| ⌘ |Command|
| ⌥ | Option |
| ⌃ | Control|
| ⏎ |Enter|

## 코드 관련 단축키
| 기능                             | 단축키                              |
|--------------------------------|----------------------------------|
| 클릭한 메소드로 이동                    | ⌘(Command) + 클릭                  |         
| 파라미터 변수 확인                     | ⌘(Command) + P                   |       
| 코드 라인 복사                       | ⌘(Command) + D                   |     
| 해당 메소드 변수화                     | ⌥(Option) + ⌘(Command) + V       | 
| 패키지 import하기                   | ⌥(Option) + ⏎                    |
| import한 패키지 중 사용하지 않는 것 정리     | ⌃(Control) + ⌥(Option) + O       | 
| 한 줄 단위로 코드 이동                  | ⇧(Shift) + ⌥(Option) + ⬆️  or ⬇️ |
| 주석                             | ⌘(Command) + /                   |
| 생성자/Getter/Setter/toString 만들기 | ⌃(Control) + ⏎(Enter)            |
| 해당 코드 라인 마치고 다음 라인으로 이동        | ⇧(Shift) + ⌘(Command) + ⏎(Enter) |
| 메소드 생성 및 수정(코드 라인 위치에서 누를 시)   | ⌥(Option) + ⏎(Enter)             |
|해당 메소드를 사용하는 곳 조회 | ⌥(Option) + F7                   |

## 파일 관련 단축키
|기능| 단축키                       |
|---|---------------------------|
|파일 이름 변경| ⇧(Shift) + F6             |
|파일 찾기| ⇧(Shift) + ⌘(Command) + O |
|이전에 열었던 파일 확인| ⌘(Command) + E            |
| 이전에 열었던 파일 상세 확인| ⇧(Shift) + ⌘(Command) + E |

## Debugging 관련 단축키
| 기능                                                   | 단축키                        |
|------------------------------------------------------|----------------------------|
| 실행                                                   | ⌃(Control) + D             |
| 프로젝트에서 실행한 브레이크 포인트 확인                               | ⇧(Shift) + ⌘(Command) + F8 |
| Resume(다음 Break Point로 이동)                           | ⌥(Option) + ⌘(Command) + R |
| Step Into(메소드 내부로 이동)                                | F7                         |
| Force Step Into(Step Into와 비슷하지만 'Stepping'을 무시하고 진행 | ⇧(Shift) + ⌥(Option) + F7  |
| Step Over(현재 실행 지점에서 다음 줄로 이동)                       | F8                         |
| Step Out(현재 break 된 라인에서 호출한 곳으로 빠져나감)               | ⇧(Shift) + F8              |
| Evalutate Expression(Break 된 상태에서 코드를 실행해서 값 확인 가능)  |⌥(Option) + F8|
| Run to Cursor(명령어 입력 시 커서가 포커스 되어있는 라인으로 이동          | ⌥(Option) + F9             |
| Show Execution Point(현재 실행 포인트로 커서 이동)               | ⌥(Option) + F10            |

> ### 참고1) Stepping이란?
> 디버그의 설정 기능 중 하나로 디버깅 중 건너뛸 수 있는 요소 지정 가능
> Command + Shift + a를 눌러서 Stepping 설정 창에서 지정

> ### 참고2) Evaluate Expression 주의사항
> 실제로 코드를 실행하는 것이기 때문에 사용에 유의해야함