# TIL (Today I Learned)π₯
2022-02-15

## Array

- μμλ₯Ό κ°κ³  μ€λ³΅μ΄ κ°λ₯νλ€
- λΉ λ°°μ΄μ λ§λ€λλ λ°λμ νμμ λͺμν΄μΌνλ€
- μμλ₯Ό μΈλ±μ€λΌκ³  νλ©° 0λΆν° μμνλ€


```swift
var animal: Array<String> = Array<String>()
```

### μΆκ° 
```swift
animal.append("tiger")
//["tiger"]
animal.append(contentsOf: ["lion, elephant"])
//["tiger", "lion", "elephant"]
animal.insert("monkey", at: 2)
//["tiger", "lion", "monkey", "elephant"]
animal.insert(contentsOf: ["lion2, elephant2"], at: 2)
//["tiger", "lion", "lion2", "elephant2", "monkey", "elephant"]
```



### κ΅μ²΄
```swift
animal[0...3] = ["dog"]
//["dog", "monkey", "elephant"]
animal.replaceSubrange(1...2, with: ["cat"])
//["dog", "cat"]
```


### μ­μ 
```swift
animal.remove(at: 0)
//["cat"]
animal.removeAll()
//[]
```

```swift
//κ°μ νλ³ κ°λ₯
animal.count == 0 
//true λλ false κ°μΌλ‘ νλ³ κ°λ₯ 

animal.isEmpty // λΉμ΄μλμ§ true false
```