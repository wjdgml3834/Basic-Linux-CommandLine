## 📌 Relative Paths

> 절대적 경로는 항상 루트 디렉토리(/)에서 시작하는 반면, 상대적 경로는 현재의 위치를 기준으로 합니다.

절대적 경로와 상대적 경로의 주요 차이점은 시작점이 다르다는 것입니다.

<br>

**1️⃣ 상대적 경로 (Relative Paths)**

> 현재 작업 디렉토리에 기반한 경로입니다.

예를 들어서 `Desktop` 폴더안에 `dogs`라는 폴더가 있고 그 안에 `cat`이라는 폴더가 있다고 가정해 봅시다.

만약에 `Desktop`을 폴더를 기준으로 `cat`으로 이동이 가능할까요?

불가능합니다. `Desktop`에는 `cat`이라는 폴더가 없기 때문이죠.

```bash
kim@kimubuntu:~/Desktop$ cd cat
bash: cd: cat: No such file or directory
```

그렇다면 `cat` 폴더로 바로 이동을 하려면 어떻게 해야할까요?

하단의 명령어처럼 진행하면 됩니다.

```bash
kim@kimubuntu:~/Desktop$ cd dogs/cat
kim@kimubuntu:~/Desktop/dogs/cat$
```

<br>

**2️⃣ 절대적 경로 (Absolute Paths)**

> 파일 시스템의 루트 디렉토리에서 시작하는 전체 경로를 나타냅니다.

예시는 아래와 같습니다.

```bash
// cat 폴더에서 절대적 경로를 이용하여 바로 Desktop폴더로 이동했습니다.
kim@kimubuntu:~/Desktop/dogs/cat$ cd /home/kim/Desktop
```

이렇게 절대적 경로를 이용하면 어디에 있던지 작동한다는 장점이 있습니다.
