# TIL (Today I Learned)π₯
2022-02-11

# λ°μ΄ν° νμ
λͺ¨λ  λ°μ΄ν°νμ μ΄λ¦μ μ²« κΈμκ° λλ¬Έμλ‘ μμνλ λλ¬Έμ μΉ΄λ©μΌμ΄μ€λ₯Ό μ¬μ©νλ€

## λΆλ¦¬μΈ(Bool)
```swift
var someBool: Bool = true
// true λλ false κ°λ§ κ°μ μ μλ€.
```
## μ μ(Int)
```swift
var someInt: Int = 1000
// μ μκ°λ§ κ°λ₯

var someUInt: UInt = 100
// 0κ³Ό μμ μ μκ°λ§ κ°λ₯   -> -λΆνΈ λΆκ°

someInt = someUInt       // (x) νμμ΄ λ¬λΌμ μ€λ₯ λ°μ 
someInt = Int(someUInt)  // (o) 
```
## μ€μ(Float,Double)
```swift
var someFloat: Float = 3.123
//32λΉνΈμ λΆλμμ νν

var someDouble: Double = 123133.2123
//64λΉνΈμ λΆλμμ νν
```
## λ¬Έμ(Character)
```swift
var someCharacter: Character = "A"
someCharacter = "β‘"
someCharacter = "γ"
// νκΈμλ§ κ°λ₯ 
```

## λ¬Έμμ΄(String)
```swift
var someString: String = "hello"
//λ¬Έμμ΄ 
someString.append(" world!")
someString = someString + " world!!" 
//λ¬Έμμ΄ μ΄μ΄λΆμ΄κΈ°

print(someString) //hello world! world!!

print(someString.isEmpty) //false
//λΉ λ¬Έμμ΄μΈμ§ μ°Έ κ±°μ§ νλ³κ°λ₯

print(someString.count) //20
//λ¬Έμμ μ μΈκΈ°


print(someString.hasPrefix("hell")) // true
// λ¬Έμμ΄μ΄ () λ‘ μμ νλμ§ Bool κ°μΌλ‘ νμΈ  

print(someString.hasSuffix("!!"))  //true
// λ¬Έμμ΄μ΄ () λ‘ λλλμ§ Bool κ°μΌλ‘ νμΈ

print(someString.uppercased())  
// λλ¬Έμ λ³ν. HELLO WORLD! WORLD!!

print(someString.lowercased()) 
// μλ¬Έμ λ³ν. hello world! world!!