## 📌 man pages(명령어 구조)

> man pages는 manual pages의 줄임말입니다.

이것은 유닉스 계열 운영체제 대부분에 있는 내장된 문서입니다.

```bash
man ncal
```

```bash
man date
```

메뉴얼에서 `f`를 누르면 페이지가 앞으로 넘어가고 (스페이스바도 마찬가지), `B`를 누르면 뒤로 넘어갑니다.

`/`를 누르고 원하는 검색을 진행할 수 있습니다.

#### ✅ man pages content (메뉴얼 페이지 구성)

메뉴얼 페이지에는 일정한 패턴이 있습니다.

1️⃣ 명령어의 이름과 함께 짧은 설명이 있습니다.

```bash
NAME
     cal, ncal – displays a calendar and the date of Easter
```

2️⃣ 명령어의 시놉시스가 있습니다.

```bash
SYNOPSIS
     ncal [-3hjJpwy] [-A number] [-B number] [-s country_code] [[month] year]
     ncal [-3hJeo] [-A number] [-B number] [year]
     ncal [-CN] [-H yyyy-mm-dd] [-d yyyy-mm]
```

여기서 `[]`은 선택 가능임을 나타냅니다.

예를들어 `-3hjJpwy`에서 각각 `-3` `-h` `-j` 등은 쓸 수 있는 옵션을 한 공간에 묶어넣은 것입니다.

`-A number`는 옵션과 함께 같이 넣어줘야하는 매개변수를 의미합니다.

`[[month] year]`는 그냥 월 혹은 년도를 넣어주면 된다는 뜻입니다. 이는 따로 옵션을 주지 않아도 된다는 뜻입니다.

```bash
SYNOPSIS
       echo [SHORT-OPTION]... [STRING]...
       echo LONG-OPTION
```

`...`의 의미는 1개 혹은 여러개를 넣어도 된다는 뜻입니다.

```bash
SYNOPSIS
       cp [OPTION]... [-T] SOURCE DEST
       cp [OPTION]... SOURCE... DIRECTORY
       cp [OPTION]... -t DIRECTORY SOURCE...
```

`SOURCE DEST`는 무엇을 복사할지, 목적지는 어디인지를 나타냅니다. 이는 선택이 아닙니다.

3️⃣ 명령어에 사용할 수 있는 옵션들에 대한 설명이 있습니다.

```bash
DESCRIPTION
     The cal utility displays a simple calendar in traditional format and ncal
     offers an alternative layout, more options and the date of Easter.  The new
     format is a little cramped but it makes a year fit on a 25x80 terminal.  If
     arguments are not specified, the current month is displayed.

     The options are as follows:

     -h      Turns off highlighting of today.

     -J      Display Julian Calendar, if combined with the -e option, display
             date of Easter according to the Julian Calendar.

     -e      Display date of Easter (for western churches).

     -j      Display Julian days (days one-based, numbered from January 1).
```
