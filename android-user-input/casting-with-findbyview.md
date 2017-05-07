## Casting

Inflation process of the activity.

Find the objects and store them as variables in the activity.

Finding the views in the view hierarchy.

Create variables that reference the specific views in the v. hierarchy.

Making the connection between the variable and the textView. The key is the view ID´sWhen to assign views. When the views will be used in the java code.  findViewById\(\) method belongs to AppCompatActivity class.

The method go and traverse through the view hierarchy and look for the view with the specified ID.

```
View summaryTextView = findViewById(R.id.text_view);
```

This will return a view as an object and it will be stored in the variable.

