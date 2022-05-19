#Constructor Overloading
```
you can only overload Secondary Constructor only not the Primary one

```

------------------------------------------------------
```
class Test{
    constructor(){
        println("Priyanka is the best")
    }
    constructor(x:Int){
        println("hello Mr. $x")
    }
}

fun main(){
	Test()    
    Test(6)
}

```

#Constructor OverRidding
```
open class Test(private val x:Int){
    
}
class Child(x:Int) : Test(x){
    init{
        println(x)
    }
}
fun main(){
    Child(12)
}

```
---------output------------------
```
12

```