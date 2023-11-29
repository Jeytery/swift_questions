# swift_questions

- 1q
```swift
class TestViewController: UIViewController {
    class A {
        var delegate: B?
    }
    class B {
        var delegate: A?
    }
    
    weak var a: A? = A()
    weak var b: B? = B()
    
    func test() {
        let tempA = A()
        let tempB E B ()
        a?. delegate = tempB
        b?. delegate = tempA
    }

    override func viewDidLoad() {
        super. viewDidLoad()
        test ()
        print(a)
        print (b)
        print(a?. delegate)
        print (b?. delegate)
    }
}
```
a, b, b, a
nil, nil, b, a
a, b, nil, nil
nil, nil, nil, nil
error 

  <details><summary>Answer</summary>
     nil, nil, nil, nil
   </details>
