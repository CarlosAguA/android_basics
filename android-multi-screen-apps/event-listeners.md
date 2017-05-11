# Event listeners

---

The user interact with the apps by touching the screen. This corresponds to user input events. You can choose to get notified when certain events occur on a specific view.

The paradigm is called: **listening for a certain event**. Once you know the event has happened, you can program what should happen when an user interacts with a part of the UI.

## What is an input event?

It is a user´s interaction with the application.

## What is an event listener?

An event listener is an interface in the `View` class that contains a single callback method. These methods will be called by the Android framework when the View to which the listener has been registered is triggered by user interaction with the item in the UI.

## What event listeners exist?

There are different kinds of event listeners like:

* Key
* Touch
* Button
* Focus

## What is a callback method?

It´s a method, which is part of an event listener and it is called by the Android framework when the respective action occurs on a view \(within this context\). Normally, you have to fill in or provide code to it, in order to perform an action once is called back.

## How to set up event listeners?

There are three options for implementing a listener:

* Implement the nested interface in your Activity
* Creating a private class
* Define an anonymous class
* Creating the onClickListener for the Button
* Defining the listener in the xml file.

### Implementing an OnClickListener as part of the activity

```
public class ExampleActivity extends Activity implements OnClickListener {
    protected void onCreate(Bundle savedValues) {
        ...
        Button button = (Button)findViewById(R.id.corky);
        button.setOnClickListener(this);
    }

    // Implement the OnClickListener callback
    public void onClick(View v) {
      // do something when the button is clicked
    }
    ...
}
```

### Defining an anonymous class

The key in this implementation is to pass  an instance of your implementation to the respective`View.set...Listener()`

method.

```
// Create an anonymous implementation of OnClickListener
private OnClickListener mCorkyListener = new OnClickListener() {
    public void onClick(View v) {
      // do something when the button is clicked
    }
};

protected void onCreate(Bundle savedValues) {
    ...
    // Capture our button from layout
    Button button = (Button)findViewById(R.id.corky);
    // Register the onClick listener with the implementation above
    button.setOnClickListener(mCorkyListener);
    ...
}
```

### Creating the onClickListener method for a button or view as inner class

```
 protected void onCreate(Bundle icicle) {
    super.onCreate(icicle);
    setContentView(R.layout.content_layout_id);

    final Button button = (Button) findViewById(R.id.button_id);
    button.setOnClickListener(new View.OnClickListener() {
            public void onClick(View v) {

              // Perform action on click   
            }
          });
  }
```

### Creating a private class

The class may be created In a separate file or within the activity file.

```
class MyOnClickListener implements View.OnClickListener {
    @Override           
    public void onClick(View v) {
        // Handle view click here           
    }
}
```

Then, an instance must be created and registered to the view.

```
MyOnClickListener listener = new MyOnClickListener();
myView.setOnClickListener(listener);
```

There exist a possibility to use event handlers which won´t be covered in this work.

### Defining the listener in the xml file

Pending.

### Sources

\[Input events\]\([https://developer.android.com/guide/topics/ui/ui-events.html\#EventListeners\](https://developer.android.com/guide/topics/ui/ui-events.html#EventListeners%29\)

\[Android button onClickListener\]\([http://stackoverflow.com/questions/16636752/android-button-onclicklistener\](http://stackoverflow.com/questions/16636752/android-button-onclicklistener%29\)

Intents and Activities /13.Event Listeners in Android

\[onClickListener implementation\] \(http://stackoverflow.com/questions/11815101/view-onclicklistener-a-function-or-interface\)

