# amp_a

PRACTICAL 2
Aim : Programming Resources 
Android Resources: (Color, Theme, String, Drawable, Dimension, 
Image) 
A Defining Color Property
B Defining Theme Property
C Defining String Property
D Adding images and dimensions
Steps :
1. Open Android Studio
2. Go to File > New > New Project
3. Select Phone and Tablet > Empty Activity > Next
4. Do the following:
a. Name of the application
b. Language : Java
c. SDK : Pie
5. Click on Finish
6. Android Studio creates the Project with many files
 Android apps contain multiple activities. (Just like how a website has multiple 
web pages!)
 As soon as the name of the application is entered, the package name also 
changes.
 Package contains all the files of that project.
 About res file (resources file)
 main > res
 Drawables : for images
 Values : 3 files default
1. Colors.xml (in hexadecimal)(RGB)
2. Strings.xml
3. Themes
Changes can be made in 
strings.xml. Once change is 
made here, it will be changed everywhere.

Activity.xml → GUI Designing
[ A ] Defining Color Property
1. Create a new project and go to:
Project Name > App > src > main > res > values > colors.xml
2. Defining new color properties in colors.xml


            <?xml version="1.0" encoding="utf-8"?>
            <resources>
             <color name="purple_200">#FFBB86FC</color>
             <color name="purple_500">#FF6200EE</color>
             <color name="purple_700">#FF3700B3</color>
             <color name="teal_200">#FF03DAC5</color>
             <color name="teal_700">#FF018786</color>
             <color name="black">#FF000000</color>
             <color name="white">#FFFFFFFF</color>
             <color name="red">#C64F4F</color>
             <color name="pink">#E1DE44B5</color>
             <color name="blue">#3692EC</color>
             <color name="green">#43BC65</color>
            </resources>
            
            
3. Now go to activity_main.xml and do the following:
a. Drag and drop LinearLayout(Vertical) From Layout tab in Palette 
window
b. Similarly, drag and drop four TextView from Text tab in palette window

c. In the TextView code, call the colors from the colors.xml file as follows 
in activity_main.xml: (line 21)

            <TextView
             android:id="@+id/textView"
             android:layout_width="match_parent"
             android:layout_height="40dp"
             android:text="TextView"
             android:background="@color/red"/>
             
             
4. Now the final Code of activity_main.xml is :


          <?xml version="1.0" encoding="utf-8"?>
          <androidx.constraintlayout.widget.ConstraintLayout 
          xmlns:android="http://schemas.android.com/apk/res/android"
           xmlns:app="http://schemas.android.com/apk/res-auto"
           xmlns:tools="http://schemas.android.com/tools"
           android:layout_width="match_parent"
           android:layout_height="match_parent"
           tools:context=".MainActivity">
           <LinearLayout
           android:layout_width="match_parent"
           android:layout_height="match_parent"
           android:orientation="vertical">
           <TextView
           android:id="@+id/textView"
           android:layout_width="match_parent"
           android:layout_height="40dp"
           android:text="TextView"
           android:background="@color/red"/>
           <TextView
           android:id="@+id/textView2"
           android:layout_width="match_parent"
           android:layout_height="44dp"
           android:text="TextView"
           android:background="@color/pink"/>/>
           <TextView
           android:id="@+id/textView3"
           android:layout_width="match_parent"
           android:layout_height="40dp"
           android:text="TextView"
           android:background="@color/green"/>/>
          <TextView
           android:id="@+id/textView4"
           android:layout_width="match_parent"
           android:layout_height="48dp"
           android:text="TextView"
           android:background="@color/blue"/>/>
           </LinearLayout>
          </androidx.constraintlayout.widget.ConstraintLayout>
          


We are done with Colors…
[ B ] Defining Theme Property
1. Defining new theme properties in themes.xml
2. Create a new project and go to:
Project Name > App > src > main > res > values > themes > themes.xml
3. Add the following codes in themes.xml :

            <resources xmlns:tools=”http://schemas.android.com/tools”>
             <!—Base application theme. 
             <style name=”Theme.Prac2_practise”
            parent=”Theme.MaterialComponents.DayNight.DarkActionBar”>
             <!—Primary brand color. 
             <item name=”colorPrimary”>@color/purple_500</item>
             <item name=”colorPrimaryVariant”>@color/purple_700</item>
             
             
We are done with Colors…
[ B ] Defining Theme Property
1. Defining new theme properties in themes.xml
2. Create a new project and go to:
Project Name > App > src > main > res > values > themes > themes.xml
3. Add the following codes in themes.xml :

            <resources xmlns:tools=”http://schemas.android.com/tools”>
             <!—Base application theme. 
             <style name=”Theme.Prac2_practise”
            parent=”Theme.MaterialComponents.DayNight.DarkActionBar”>
             <!—Primary brand color. 
             <item name=”colorPrimary”>@color/purple_500</item>
             <item name=”colorPrimaryVariant”>@color/purple_700</item>


We are done with the themes…


[ C ] Defining String Property
1. Defining paragraph and header property in strings.xml
2. Create a new project and go to:
Project Name > App > src > main > res > values > strings.xml
strings.xml

          <resources>
           <string name="app_name">Prac2</string>
           <string name="Heading">This is Practical 2 of AMP</string>
           <string name="Description">
           NAME : Anjana Jayan Kizhiyapat\nROLL : A020
           </string>
          </resources>
          
activity_main.xml
→ Change any 2 TextView

            <TextView
             android:id="@+id/textView"
             android:layout_width="match_parent"
             android:layout_height="40dp"
             android:text="@string/Heading"
             android:background="@color/red"/>
            <TextView
             android:id="@+id/textView2"
             android:layout_width="match_parent"
             android:layout_height="44dp"
             android:text="@string/Description"
             android:background="@color/pink"/>


We are done with the strings…
[ D ] Adding images and dimensions
1. Adding Images to Application created
2. For adding a new image files, do the following:
Project Name > App > src > main > res > drawable > Right-click and paste the images that are copied


3. Create a new file called dim.xml in the res > values > New > Values 
Resource File folder
4. Write the following code in dim.xml

            <?xml version="1.0" encoding="utf-8"?>
            <resources>
             <dimen name="textview_height">35dp</dimen>
             <dimen name="textview_width">150dp</dimen>
             <dimen name="font_size">26sp</dimen>
            </resources>
            activity_main.xml
            <?xml version="1.0" encoding="utf-8"?>
            <androidx.constraintlayout.widget.ConstraintLayout 
            xmlns:android="http://schemas.android.com/apk/res/android"
             xmlns:app="http://schemas.android.com/apk/res-auto"
             xmlns:tools="http://schemas.android.com/tools"
             android:layout_width="match_parent"
             android:layout_height="match_parent"
             tools:context=".MainActivity">
             <LinearLayout
             android:layout_width="match_parent"
             android:layout_height="match_parent"
             android:orientation="vertical">
             <TextView
             android:id="@+id/textView"
             android:layout_width="match_parent"
             android:layout_height="40dp"
             android:background="@color/red"
             android:text="@string/Heading"
             tools:ignore="TextContrastCheck" />
             <TextView
             android:id="@+id/textView2"
             android:layout_width="match_parent"
             android:layout_height="44dp"
             android:background="@color/pink"
             android:text="@string/Description"
             tools:ignore="TextContrastCheck" />
             <TextView
             android:id="@+id/textView3"
             android:layout_width="match_parent"
             android:layout_height="40dp"
             android:background="@color/green"
             android:text="TextView"
             tools:ignore="TextContrastCheck" />
             <TextView
             android:id="@+id/textView4"
            android:layout_width="match_parent"
             android:layout_height="48dp"
             android:background="@color/blue"
             android:text="TextView"
             tools:ignore="TextContrastCheck" />
             <ImageView
             android:id="@+id/imageView"
             android:layout_width="match_parent"
             android:layout_height="wrap_content"
             app:srcCompat="@drawable/yh" />
             </LinearLayout>
            </androidx.constraintlayout.widget.ConstraintLayout>


