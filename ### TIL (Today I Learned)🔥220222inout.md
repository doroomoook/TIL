# TIL (Today I Learned)π₯

2022-02-22

<br>

```swift
var number = 100

func add(to number: Int) -> Int {
    number += 1
    return number
}
```

![https://s3.ap-northeast-2.amazonaws.com/media.yagom-academy.kr/resources/usr/61ee3b7c2947bf40f08f32e4/20220223/6216150d536b5e1551d11006.png](https://s3.ap-northeast-2.amazonaws.com/media.yagom-academy.kr/resources/usr/61ee3b7c2947bf40f08f32e4/20220223/6216150d536b5e1551d11006.png)



1μ λνλ ν¨μλ₯Ό λ§λ€μλλ° 

μ΄μ²λΌ μ€λ₯κ° λμλ€.

<br>

```swift
func addOne(to number: Int) -> Int {
    var functionNumber = number
    functionNumber += 1
    return functionNumber
}

print(addOne(to: number))  // 101
print(number)  // 100
```

μ΄λ κ² ν¨μμμ λ³μλ₯Ό μ μΈνλ©΄ λ΅μ λμ€μ§λ§ 

λ€μ `number` λ₯Ό μΆλ ₯νμ λ κ°μ λ³νμ§ μμλ€.

κ·Έλ κ² κ΅¬κΈλ§ν΄λ³Έκ²°κ³Ό

<br>

# inout

```swift
func addTwo(to number: inout Int) -> Int {
    number += 2
    return number
}

print(addTwo(to: &number))  // 102
print(number)  // 102
```

ν¨μ λ§€κ°λ³μ νμμ μΈ μμ ``inout`` μ λΆμ΄κ³ 

ν¨μ νΈμΆ λ ``&`` λ₯Ό λΆμ¬μ£Όλ©΄ 

`number`κ°λ λμΌνκ² λ°λκ² λλ κ²μ μκ² λμλ€.

<br>

#### inout μ΄λ 

**copy-in copy-out** μ μ€μλ§μ΄λ©°

- ν¨μ νΈμΆ  
         β
- λ§€κ°λ³μ μλ¦¬μ λ³μ λ³΅μ¬
         β
- ν¨μ λ΄λΆ κ° μμ 
         β
- λ°νν κ° λ³μμ μ¬ν λΉ

         κ³Όμ μΌλ‘ μ΄λ£¨μ΄μ§λ€.


<br>


### π«
```swift
let letNumber = 100
addTwo(to: &letNumber) //(x)
addTwo(to: &10) //(X)
```

- μμλ λ¦¬ν°λ΄μ `inout` λ§€κ°λ³μμ μΈμκ°μΌλ‘ μ λ¬ν  μ μλ€.

<br>

### μ°Έμ‘°

https://syjdev.tistory.com/21

κΌΌκΌΌν μ¬μμ¨μ swift: λ¬Έλ²νΈ