# Ex.No:1 To create a HelloWorld Activity using all lifecycles methods to display messages.


## AIM:

To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:
```
/*
Program to print the text “Hello World”.
Developed by:Kausalya G
Registeration Number :212221040076
*/
```
## activity_main.xml:

```
activity_main.xml:

<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
xmlns:android="http://schemas.android.com/apk/res/android"
 xmlns:app="http://schemas.android.com/apk/res-auto"
 xmlns:tools="http://schemas.android.com/tools"
 android:layout_width="match_parent"
 android:layout_height="match_parent"
 tools:context=".MainActivty">
 <TextView
 android:layout_width="wrap_content"
 android:layout_height="wrap_content"
 android:text="Hello World!"
 app:layout_constraintBottom_toBottomOf="parent"
 app:layout_constraintEnd_toEndOf="parent"
 app:layout_constraintStart_toStartOf="parent"
 app:layout_constraintTop_toTopOf="parent" />
</androidx.constraintlayout.widget.ConstraintLayout>
```

## MainActivity.java:
```
MainActivity.java:
package com.example.life;
import android.content.Context;
import android.content.Intent;
import android.support.annotation.Nullable;
import android.support.v7.app.AppCompatActivity;
import android.os.Bundle;
import android.widget.Toast;
public class MainActivity extends AppCompatActivity {
 @Override
 protected void onCreate(Bundle savedInstanceState) {
 
 super.onCreate(savedInstanceState);
 setContentView(R.layout.activity_main);
 Toast.makeText(this, "onCreate Called",
Toast.LENGTH_SHORT).show();
 }
 
 @Override
  protected void onRestart() {
       Toast.makeText(this, "onRestart Called",
Toast.LENGTH_SHORT).show();
 super.onRestart();
 }
 
 @Override
 protected void onStart() {
 Toast.makeText(this, "onStart Called",
Toast.LENGTH_SHORT).show();
 super.onStart();
 }
 
 @Override
 protected void onResume() {
       Toast.makeText(this, "onResume Called",
Toast.LENGTH_SHORT).show();
 super.onResume();
 }
 
 @Override
 protected void onPause() {
 Toast.makeText(this, "onPause Called",
Toast.LENGTH_SHORT).show();
 super.onPause();
 }
 
 @Override
 protected void onStop() {
       Toast.makeText(this, "onStop Called",
Toast.LENGTH_SHORT).show();
 super.onStop();
 }
 
 @Override
 protected void onDestroy() {
       Toast.makeText(this, "onDestroy Called",
Toast.LENGTH_SHORT).show();
 super.onDestroy();
 }}
```

## OUTPUT
![Screenshot (37)](https://github.com/gkausalya232/LifeCycle/assets/133086820/293ac961-204a-4e99-8333-1a952fdc922c)
![Screenshot (38)](https://github.com/gkausalya232/LifeCycle/assets/133086820/3aebf15f-3b4f-4de8-b6a5-9a65472dfd7e)
![Screenshot (39)](https://github.com/gkausalya232/LifeCycle/assets/133086820/b4c521e3-58a3-40e6-830b-9b86e24d9fda)
![Screenshot (40)](https://github.com/gkausalya232/LifeCycle/assets/133086820/219655df-3e66-4d5e-b959-a85817599a22)
![Screenshot (41)](https://github.com/gkausalya232/LifeCycle/assets/133086820/623e09f9-9080-44f0-80b5-195da80f67ca)
![Screenshot (42)](https://github.com/gkausalya232/LifeCycle/assets/133086820/4d050f50-be25-4d9f-a0c2-68ba47b57824)
![Screenshot (43)](https://github.com/gkausalya232/LifeCycle/assets/133086820/e67a295f-9d3d-4b62-b906-52d37fa2ac7c)



## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
