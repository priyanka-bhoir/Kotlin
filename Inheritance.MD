#Inheritance

##Single Inheritance

open ----> public
```
//single
open class Parent{
    fun parentProperty(){
        println("Priyanka's Property..")
    }
}
class Child : Parent(){
    fun childProperty(){
        println("Child's Property..")
    }
}

fun main(){
    val ch = Child()
    ch.childProperty()
    ch.parentProperty()
    
}
```

##Multilevel Inheritance

```
//multilevel Inheritance
open class Parent{
    fun parentProperty(){
        println("Priyanka")
    }
}

open class Child : Parent(){
    fun childProperty()
    {
        println("Child Property...")
    }
}

class GrandSon : Child(){
    fun grandChild(){
        println("Grandson Property..")
    }
}

fun main(){
    val grandSon = GrandSon()
    grandSon.grandChild()
    grandSon.parentProperty()
    grandSon.childProperty()
}

```
----------output-----------
```
Grandson Property..
Priyanka
Child Property...

```

##Hierarchical Inheritance
```
open class PArent{
    fun ParentProperty(){
        println("getting Property")
    }
}

class Son : PArent(){
    fun son(){
        println("son's Property")
    }
}

class Daughter : PArent(){
    fun daughter(){
        println("daughter's Propety")
    }
}

fun main(){
    val son = Son()
    val daughter = Daughter()
    
    son.ParentProperty()
    daughter.ParentProperty()
}

```
------------------output------------
```
getting Property
getting Property

```

##Hybrid Inheritance 
```
open class PArent{
    fun ParentProperty(){
        println("getting Property")
    }
}

class Son : PArent(){
    fun son(){
        println("son's Property")
    }
}

open class Daughter : PArent(){
    fun daughter(){
        println("daughter's Propety")
    }
}

class Single : Daughter(){
 	fun single(){
        println("getting daughter's property")
    }   
}

fun main(){
//     val son = Son()
//     val daughter = Daughter()
    val single = Single()
    
//     son.ParentProperty()
//     daughter.ParentProperty()
//     
    single.daughter()
    single.single()
    single.ParentProperty()
    
}

```
------------output----------------
```
daughter's Propety
getting daughter's property
getting Property

```