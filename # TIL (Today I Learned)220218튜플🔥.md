# TIL (Today I Learned)π₯
2022-02-18

# νν

ν κ°μ§ νμμ μμ΄νλ§ μ μ₯ν  μ μλ λ°°μ΄μ΄λ λμλλ¦¬μλ λ¬λ¦¬ 

νλμ ννμ μ¬λ¬ κ°μ§ νμμ μμ΄νμ μ μ₯ν  μ μμ§λ§

λ°°μ΄μ΄λ μ§ν©κ³Ό λ¬λ¦¬ μκ΄νΈ()λ₯Ό μ¬μ©νμ¬ μ μνλ€.

```swift
var tuple = ("zero", 3, 2, "three")
```

```swift
tuple.0 // zero
tuple.1 // 1
tuple.2 // 2
tuple.3 // three
```


ννμμ ννμ κ°μ μ κ·Όν  μλ μλ€.

### ννμ νν

```swift
var tuple = ("zero", 3, 2, "three")
var otherTuple = ((tuple), 4, 5)
```

```swift
otherTuple.0 // ("zero", 1, 2, "three")
otherTuple.0.0 // zero
otherTuple.0.1 // 1
otherTuple.1 // 4
otherTuple.2 // 5
```
### μ΄λ¦ λΆνκΈ°
```swift
var namedTuple = (age: 50, place: ["cafe, home"]) // (age: 50, place: ["cafe, home"])
// namedTuple = ("lol", ["playground", "school"])  (X)
// age κ°μ΄ Int κ°μ΄μμΌλ―λ‘ String νμμΌλ‘ λ³κ²½μ΄ λΆκ°λ₯νλ€
namedTuple.age // 50
namedTuple.place // ["cafe, home"]
```
- μ΄λ¦μ λΆμ¬μ μ΄λ¦μΌλ‘ κ°μ μ κ·Όν  μ μλ€.

- μ μΈνκ³  λλ©΄ κ°μ νμ κ°μΌλ‘ λ§ λ°κΏ μ μλ€.

- κ°μ μΆκ°λ μ­μ λ ν  μ μλ€.


#### μ°Έμ‘°

https://zeddios.tistory.com/238

https://docs.swift.org/swift-book/ReferenceManual/Types.html