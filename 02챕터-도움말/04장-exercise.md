## 📌 Getting Help Exercise

#### Q: There is a command called `whoami`. **Before you run it**, read the manual page entry on it. From the manual page entry, can you tell if it needs any options or arguments? What does it do?

```bash
NAME
       whoami - print effective userid

SYNOPSIS
       whoami [OPTION]...

DESCRIPTION
       Print the user name associated with the current effective user ID.  Same as id -un.

       --help display this help and exit

       --version
              output version information and exit
```

`whoami` 명령어는 유저 아이디를 출력하는 명령어이다.

`whoami` 명령어 같은 경우 옵션 두개를 쓸 수있다. `--help` 와 `--version`이 그 두 가지이다.

이 `...`으로 보아 두 가지의 옵션을 동시에 쓸 수 있다.

#### Q: There is another command called `who`. Without turning to Google, figure out what it does! Does it require any arguments or options to run?

```bash
NAME
       who - show who is logged on

SYNOPSIS
       who [OPTION]... [ FILE | ARG1 ARG2 ]

DESCRIPTION
       Print information about users who are currently logged in.

       -a, --all
              same as -b -d --login -p -r -t -T -u

       -b, --boot
              time of last system boot

       -d, --dead
              print dead processes

       -H, --heading
              print line of column headings

       --ips  print  ips  instead  of  hostnames. with --lookup, canonicalizes based on stored IP, if available,
              rather than stored hostname

       -l, --login
              print system login processes

       --lookup
              attempt to canonicalize hostnames via DNS

       -m     only hostname and user associated with stdin

       -p, --process
              print active processes spawned by init

        -q, --count
              all login names and number of users logged on

       -r, --runlevel
              print current runlevel

       -s, --short
              print only name, line, and time (default)

       -t, --time
              print last system clock change

       -T, -w, --mesg
              add user's message status as +, - or ?

       -u, --users
              list users logged in

       --message
              same as -T

       --writable
              same as -T

       --help display this help and exit

       --version
              output version information and exit

       If FILE is not specified, use /var/run/utmp.  /var/log/wtmp as FILE is common.  If ARG1  ARG2  given,  -m
       presumed: 'am i' or 'mom likes' are usual.
```

`who` 명령어는 지금 현재 로그인되어 있는 유저를 출력하는 명령어이다.

#### Q: Use the `who` command to print out the time of the most recent system boot. You'll need to find an option to help you do this!

```bash
who -b
         system boot  2023-08-30 09:07
```

#### Q: Run a command to figure out whether the `echo` command is a a binary, a shell-built in, or an alias.

```bash
type echo

결과: echo is a shell builtin
```

#### Q: Do the same for the `date` command

```bash
type date

결괴: date is hashed (/usr/bin/date) // 찾기의 과정을 줄이기 위해, shell (사용자와 컴퓨터 시스템 간의 인터페이스)은 한 번 찾은 명령어의 위치를 "기억"합니다. 이렇게 기억하는 것을 "hashing"이라고 합니다. date는 외부 명령어입니다. date라는 외부 명령어의 위치(/usr/bin/date)를 쉘이 기억하고 있다는 것을 의미합니다.
```
