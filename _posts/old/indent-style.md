---
layout  : wiki
title   : 중괄호 인덴트 스타일
summary : K&R style, Allman style
date    : 2017-03-08 23:00:00 +0900
updated : 2019-01-14 21:41:31 +0900
tag     :
toc     : true
public  : true
parent  : what
latex   : false
---
* TOC
{:toc}

중괄호 인덴테이션 방식에도 이름이 있을 거라는 생각은 했었지만 실제로 찾아본 건 오늘이 처음이다.

# K&R style

K 는 Kernighan을 말하고, R은 Ritche를 뜻한다.

즉 [The C Programming Language](https://en.wikipedia.org/wiki/The_C_Programming_Language)에서 사용된 스타일이다.

```c
while (x == y) {
    something();
    somethingelse();
}
```

중괄호 시작부분을 오른쪽에 두는 K&R 스타일이라 보면 되겠다고 생각했지만 꼭 그렇지만은 않은 모양이다.

```c
int main(int argc, char *argv[])
{
    ...
    while (x == y) {
        something();
        somethingelse();

        if (some_error)
            do_correct();
        else
            continue_as_usual();
    }

    finalthing();
    ...
}
```

# Allman style

```c
while (x == y)
{
    something();
    somethingelse();
}
```

# Links

* [Indent_style](https://en.wikipedia.org/wiki/Indent_style)을 참고하였다.

