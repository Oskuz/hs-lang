# hs-lang
hs is small (toy) system language.
Example code:
```
module main {
    import "io", "math"
    let main = (){   #fibonacci
                     [1 ..8] |> (n:i32){ 
                                    if n <= 1 { ret 1}
                                    else {ret rec(n-1) + rec(n-2)}
                                    } | println;
                 }

#struct
type vector = {i:i j:i},
    impl{ 
        let lenght = (self){ math.sqr math.pow self.i 2 + math.pow self.j 2 }
    }
}   
```
