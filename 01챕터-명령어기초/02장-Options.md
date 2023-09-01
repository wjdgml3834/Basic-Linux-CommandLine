## 📌Combining Options (옵션 한꺼번에 쓰기)

옵션을 한 번에 여러개 줄 수도 있습니다.

```bash
ncal -3 -h
```

계속 따로 쓰면 불편하기에 한꺼번에 줄여서 쓸 수도 있습니다.

```bash
ncal -3hjM
```

## 📌Long Form Option (긴 형태 옵션 쓰기)

`--`이것은 쉘에게 긴 옵션임을 알려주는 것입니다.

뒤 따라오는 글자들을 하나의 옵션으로 인식하라는 뜻입니다.

모든 명령어가 지원하는 것은 아니지만, 일부 명령어들이 지원합니다.

이것들이 필요한 이유는 단어 자체가 때로는 설명이 되기 때문에 다른 사람에게 이해를 시킬때 용이합니다.

```bash
date --universal // 각각 -u , -n으로 인식하는 것이 아니라, 한 단어로 인식합니다.
```

```bash
sort --reverse colors.txt

sort -r colors.txt
```

```bash
sort colors.txt --reverse --unique // 2개이상 길게 써주는 옵션을 사용하고 싶다면, 공백을 가져서 구분해줍니다.

sort colors.txt -ru // u는 unique의 약자로 중복없이 정렬합니다.
```

## 📌Options with Parameters (매개변수를 필요로 하는 옵션들)

일부 옵션의 경우에 값을 전달해줘야 하는 경우가 있습니다.

```bash
ncal -A 1 // 현재 달부터 한 달 뒤까지 출력합니다.
```

```bash
ncal -B2 // 현재 달부터 두 달 전까지 출력합니다. B와 숫자 사이에는 공백은 써도 되고 안써도 됩니다.
```

```bash
ncal october 1996 -A1 -B1
```
