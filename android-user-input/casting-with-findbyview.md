## Casting

In order to understand casting, you have to be familiar with the Inflation process of the activity. When you create an activity, there is always an xml file in paralel. This xml file has a hierarchy with different widgets or views that need to be inflated on the activity.

To do so, the `OnCreate()` method takes place as well as the `setContentView()` within it. What this last method does is finding the views in the view hierarchy in order to inflate them.

When the views are going to be used or referenced in the activity the same process take place but with the help of other method called `findViewById()`. 

## When to use findViewById or assing views?

When the views will be used in the java code or activity and you can store them as variables within it.

## How to use findViewById ?

Creating variables that reference the specific views in the view hierarchy. For example,  making the connection between the variable and the textView \(This will return a view as an object and it will be stored in the variable\).

```
View summaryTextView = findViewById(R.id.text_view);
```

The ID is  **R.id.text\_view **so the  method goes and traverse through the view hierarchy and look for the view with the specified ID.

The method belongs to **AppCompatActivit**y class.

The left side is where you store it \(data type and name of the variable\) , and the left side is the return type of using the findViewById.



