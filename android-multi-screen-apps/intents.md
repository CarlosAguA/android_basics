# Intents

## What types of intents exist?

There are two types of intents. Explicit and implicit.

## What is an intent?

An intent is a messaging object you can use to request an action from another app component.

## What is an app component?

They are the essential builiding blocks of an Android app. Each component is an entry point through which the system or a user can enter your app.

There are four different types of app components:

* Activities.
* Services.
* Broadcast receivers.
* Content providers.

## What is an explicit intent?

An explicit intent allows you to **start a component** in your own app, because you know the class name of **the activity or service** you want to start.

## What is an implicit intent?

An implicit intent allows you to **start an activity** in another app by **describing a simple action** you would like to perform in an intent object. It does not name a specific component. This is specific for an **implicit** intent. Some examples are:

* Open a website in your app.
* Create alarm
* Capture a picture and return it.
* Make a call. 

## What´s inside an intent?

You can imagine the intent, which we already stated it is a messaging object, as a ball. When we launch it it may contain different things depending on if it´s explicit or implicit. 

![](/assets/intents.jpg\)

### Code example of explicit intent.

```
Intent intent = new Intent(CatalogActivity.this, DetailsActivity.class);
                intent.putExtra("fab_button", message);
                startActivity(intent);
```

### Code example of implicit intent.

```
  Intent intent = new Intent(Intent.ACTION_DIAL);
                intent.setData(Uri.parse("tel:" + phoneToCall));
                startActivity(intent);
```

### Sources

[App comonents](https://developer.android.com/guide/components/fundamentals.html#Components)

[Intents and intent filters](https://developer.android.com/guide/components/intents-filters.html)

[Common intents](https://developer.android.com/guide/components/intents-common.html#Music)

