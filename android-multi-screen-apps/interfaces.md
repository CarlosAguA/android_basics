# Interfaces

---

In order to understand an interface, you need to remember what a class is. A class contains the **state** and **methods** which are fully implemented.

### Example concrete class

The following code shows the **Book** class. The states are **author** and **title**.The implemented methods are  `getAuthor()` and `getTitle().`

```
public class Book {
    private String author ;
    private String title ;

    public Book (String title , String author){
        this.author = author ;
        this.title = title ;
    }

    public String getAuthor(){
        return author ;
    }

    public String getTitle(){
        return title ;
    }
```

## What´s an interface ?

In Java, Interfaces are equivalent to protocols. They basically represent an agreed-upon behavior to facilitate interaction between unrelated objects. In summary, an interface is normally a group of methods with empty bodies.

The interface `onClickListener()`has one abstract method called `onClick()`,which provide developers the power to customize its behavior.

```
button.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View view) {
                // Do something
            }
        });
```

## What´s an abstract class?

In Java, abstract class is a class which has been declared ‘abstract’. By declaring ‘abstract’ we ensure that the class can’t be instantiated.

## What´s an abstract method?

An abstract method is a method which doesn’t have any implementation.

```
           @Override
            public void onClick(View view) {
                // Do something
            }
```

## What´s a method´s signature?

The method's name, return value and the parameter types.

### Sources

[Difference between interface and abstract class](http://www.onsandroid.com/2011/12/difference-between-interface-and.html)

[Method´s signature](http://stackoverflow.com/questions/16149285/does-a-methods-signature-in-java-include-its-return-type)

[The onClickListener interface](https://developer.android.com/reference/android/view/View.OnClickListener.html)





