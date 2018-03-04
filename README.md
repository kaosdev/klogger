# KLogger
Expressive, simple yet powerful kotlin logger for Android


## Example usage
```kotlin
fun test() {
    this d "That's cool"
    //on Any variable
    MainActivity.Example.pizza i "I want to eat you"

    MainActivity.Example i {
        pizza d {
            "type: $type good? $good"
        }
        pizza
    }

    i {
        MainActivity.Example.doSomething() //doSomething and Log the result
    }
    // or
    i {"Pizza"} //where Pizza can be Any? variable

    //with custom tags
    "myTag" e "pizza is too good"
    "myTag" i {
        MainActivity.Example.eatPizza() //or "eatPizza" like before
    }

    //also d, e, w ,v and wtf

    //Try also this
    MainActivity.Example tryLog {
        eatPizzaWithException() //doSomething and then log any Exception
    }

    logTime {
        (1..100).sumBy { it + 1 }
    }
}
```

## Using klogger

### Gradle
```groovy
allprojects {
    repositories {
        maven { url 'https://jitpack.io' }
    }
}
//...
dependencies {
    compile 'com.github.kaosdev:klogger:0.1.2'
}
```
