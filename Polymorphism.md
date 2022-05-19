##Polymorphism
-----------------------------
```
many forms

```
**overloading
**overriding



**Function Overloading
```
class Test{
    fun disp(){
        println("Priyanka is the best")
    }
    
    fun disp(x:Int)
    {
        print(x)
    }
    fun disp(x:Int , y:Int){
        print(x*y)
    }
}

fun main(){
    val test = Test()
    test.disp()
    test.disp(9)
    test.disp(5,8)
}

```

**Function Overriding
```
open class Parent{
    open fun property(){
        println("Parent's Property")
    }
}

 class Child : Parent(){
    override fun property(){
        println("child's Property..")
    }
}

fun main(){
    val child = Child()
    child.property()
}

```

------------output---------------
```
child's Property..

```

**Super Keyword
```
open class Parent{
    open fun property(){
        println("Parent's Property")
    }
}

 class Child : Parent(){
    override fun property(){
        super.property()
        println("child's Property..")
    }
}

fun main(){
    val child = Child()
    child.property()
}

```

------------output-------------------
```
Parent's Property
child's Property..

```
