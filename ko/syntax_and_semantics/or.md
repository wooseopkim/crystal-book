# ||

`||`(논리합, OR)는 좌항을 먼저 평가합니다. 그 값이 *참*이라면, 우항을 평가하여 그 값을 가집니다. 그렇지 않다면 좌항의 값을 가집니다. 그 타입은 양쪽 항의 타입의 결합입니다.

`||`를 `if`의 문법적 설탕으로 볼 수 있습니다.

```crystal
some_exp1 || some_exp2

# 다음과 동일
tmp = some_exp1
if tmp
  tmp
else
  some_exp2
end
```