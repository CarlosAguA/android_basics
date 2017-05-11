# Interfaces

---

In order to understand an interface, you need to remember what a clas is. A class contains the **state **and **methods** which are fully implemented.

### Example concrete class

The following code shows the **Book** class. The states are** author **and **title**.The implemented methods are  `getAuthor()` and `getTitle().`

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



