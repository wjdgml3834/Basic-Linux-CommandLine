## 📌Command Structure (명령어 구조)

```bash
command -options arguments
```

### ✅ option:

> 명령어를 실행할 때 같이 줄 수 있는 다양한 옵션들을 나타냅니다.

항상 옵션을 줄때는 '-'를 앞에 붙입니다.

```bash
ncal -h // 달력의 하이라이트를 끕니다.
ncal -j // 1월1일부터 센 날짜 수가 나옵니다. 율리우스식입니다.
ncal -M // 월요일이 먼저 달력에 등장하게 합니다.
ncal -3 // 이전 달, 현재 달, 그리고 다음 달이 출력됩니다.
sort -r colors.txt // 반대로 정렬할 때 사용합니다.
```

### ✅ arguments

> 명령어에 값을 넘겨줍니다. (passing a value to the command.)

```bash
cal october 1996 // 공백문자로 구분하는 두 개의 인자 october와 1996을 넘겼다.
```

```bash
sort colors.txt
```
