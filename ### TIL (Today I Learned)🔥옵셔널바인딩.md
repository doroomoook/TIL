### TIL (Today I Learned)π₯

2022-02-21


# μ΅μλ λ°μΈλ©
<br>

μ‘°κ±΄λ¬Έμ μ΄μ©ν΄ (let)μμ λλ (var)λ³μμ μ΅μλκ°μ λμνλ λ°©μμΈλ°

κ·Έ κ²°κ³Όμ μ°Έ κ±°μ§ κ°μ λ°λΌ nil κ°μΈμ§ μλμ§ κ΅¬λΆν μμλ€.

```swift
var optionalNumber1: Int? = 12
var optionalNumber2: Int? = nil

print(optionalNumber1) // Optional(12)
print(optionalNumber2) // nil
```
<br>

## if let

```swift
func optionalIf(_ optionalNumber: Int?) {
    if let number = optionalNumber {
        print("\(number) λ°ν")
    } else {
        print("κ° λ°ν μ€ν¨")
    }
}

optionalIf(optionalNumber1)  //12 λ°ν
optionalIf(optionalNumber2)  //κ° λ°ν μ€ν¨
```
optianalNumber λ₯Ό number μ λμνμ¬ 

λμμ΄ κ°λ₯νλ©΄ μ°Έ. λ°λΌμ ifμ‘°κ±΄μλ§λ κ°μ΄ λμ€κ³ 

λμν μμμΌλ©΄ else λ¬Έμ΄ μ€νλλ€.

<br>

## guard let
```swift
func optionalGuard(_ optionalNumber: Int?) {
    guard let number = optionalNumber else {
        print("κ° λ°ν μ€ν¨")
        return
    }
    print("\(number) λ°ν")
}

optionalGuard(optionalNumber1) //12 λ°ν
optionalGuard(optionalNumber2) //κ° λ°ν μ€ν¨
```

guard let μ μ‘°κ±΄μ λ§μ‘±νλ©΄ λμ΄κ°κ³ 

λ§μ‘±νμ§λͺ»νλ©΄ else λ¬Έμ΄ μ€νλλ€. 