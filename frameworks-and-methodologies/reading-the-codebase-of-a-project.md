# Reading a codebase

When you import a project you can start exploring it

1. Check the **java folder** \(where the logic of the app is\)
2. Check the **resource folder** \(where everything related to the appearance of the app is\).Resources can include xml files, images and other media files.
3. Open the **layout folder** and explore it. 
4. Open the **mipmap folder** which contains the icon of the app.
5. Images of the app go on the **drawable folder**.
6. The **values folder **contains: dimensions.colors, strings ,styles: the theme of the app is defined here.

| Java Folder | Layout Folder | Drawable Folder | Values Folder |
| :---: | :---: | :---: | :---: |
| ![](/assets/logic.png) | ![](/assets/layout.png) | ![](/assets/drawable.png) | ![](/assets/values.png) |

## Drawing the diagram of an app

After checking the folders you can start creating the visual diagram of the different parts of the app.

![](/assets/Codebase_reading.png)

According to the video of the lesson 1 : Activities and intents: Quiz: import an existing project, having a mental map in our head will help us figure out what parts of the app you would need to modify to make new features work properly.

### Summary
If the changes are related to the **logic** and how the app responds, you should go to the **java folder**.

If the cahnges are related to the **view and design** of the app, you should go to the **resources folder**.
