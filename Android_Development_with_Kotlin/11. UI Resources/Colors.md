# <div align="center">Color Resources</div>

In our android apps there are certain colours that go with our designs and app purpose. 
Every app generally has a colour palleete. 
Like WhatsApp uses it's teak green and white colour. 

So, basicaly while creating the application the developer will have to use the same shade again and again at many places.

>android:background="#D1E8E4"  
```
Writing the #RRGGBB value for the particular color is tedious
```

**Instead of manually writing the hexadecimal values, we can create a color.xml file in our res directory.**

![navigation](https://user-images.githubusercontent.com/72865709/137015432-8978dbf4-9e0f-46fa-99b3-b7c532bda64b.jpg)

**res/values/colors.xml**
In here we can easily list different colors used in the app.


```
<?xml version="1.0" encoding="utf-8"?>
<resources>
    <color name="black">#000000</color>
    <color name="ColorDefaultNote">#606570</color>
    <color name="ColorBlueNote">#4e33ff</color>
    <color name="ColorYellowNote">#ffd633</color>
    <color name="ColorWhiteNote">#ffffff</color>
</resources>
```

Once you have declared your colors in the res directory you can easily use them inside your .xml file or your .kt file.

**Inside the .xml files**

```
android:textColor="@color/black"
```

**Inside the .kt file**

```
val color: Int = resources.getColor(R.color.ColorDefaultNote);
```
