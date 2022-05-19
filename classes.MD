# Classes

```
class Dog{
    val color = "black"
    
    fun sound(){
        println("woof.......")
    }
}

fun main(){
    val dog:Dog = Dog()
    println(dog.color)
    dog.sound()
}

```
**Dirrectly Accessing the class
```
	Dog().sound()
    println(Dog().color) 
```

##Constructor

**Primary Constructor
```
class Test{
  init{
      println("Priyanka is the Best")
  }
}

fun main(){
	Test()
}

```

**Paramiterized Constructor
```
 class Test(private val name:String){
 init{
     println(name)
 }
}

fun main(){
	Test("Priyanka")
}

```

**Secondary Constructor
```
class Test{
 constructor(){
     println("Priyanka")
 }
}

fun main(){
	Test()
}

```

**Secondary Paramiterized Constuctor
```
class Test{
    private lateinit var name:String
 constructor(name1:String){
     name = name1
 }
 fun printName(){
     println(name)
 }
}

fun main(){
	val test = Test("Priyanka")
    test.printName()
}

```

**Primary and Secondary Constructor together
```
class Test(private val fName:String){
    constructor(FName:String,lName:String):this(FName){
        println("my Name is $FName $lName")
         
    }
}

fun main(){
    Test("Priyanka","Bhoir")
} 

