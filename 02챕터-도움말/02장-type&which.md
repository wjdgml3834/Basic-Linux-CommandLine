## 📌 type & which command

#### ✅ type

> `type`은 명령어의 종류를 확인할 수 있습니다.

즉 명령어가 어디에, 어떻게 정의되어있는지 보여줍니다.

지정한 명령어가 쉘에 내장된 명령어인가? 또는 앨리아스(alias)명령어인가? 또는 함수(function)인가? 그리고 디스크상에 파일로 존재하는 외부명령어인가를 확인하는 방법으로 type명령어를 사용합니다.

`type`이라는 명령어를 실행해봅시다.

```bash
type passwd

passwd is /usr/bin/passwd // 바이너리이고 파일로 존재하는 실행 가능한 스크립트입니다.
```

```bash
type cd // change directory의 약자입니다.

cd is a shell builtin // 쉘에 내장된 명령어입니다.
```

#### ✅ which

> 명령어가 어디에 위치해있는지를 보여줍니다.

단, 별칭 혹은 내장된 쉘 명령어의 경우에 사용할 수 없습니다.

```bash
which passwd

/usr/bin/passwd
```
