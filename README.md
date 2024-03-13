# Ex.No:2 To create a HelloWorld Activity using all lifecycles methods to display messages.


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
Developed by:Ranjeeth B K
Registeration Number :212222040132
*/
```
# MainActivity.java
```java
package com.example.lifecycle;


import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast toast = Toast.makeText(getApplicationContext(), "onCreate Called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onRestart()
    {

        super.onRestart();
        Toast toast =Toast.makeText(getApplicationContext(),"onReStart Called",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onStart()
    {

        super.onStart();
        Toast toast =Toast.makeText(getApplicationContext(),"onStart Called",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onResume()
    {

        super.onResume();
        Toast toast =Toast.makeText(getApplicationContext(),"onResume Called",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onPause()
    {

        super.onPause();
        Toast toast =Toast.makeText(getApplicationContext(),"onPause Called",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onStop()
    {
        super.onStop();
        Toast toast = Toast.makeText(getApplicationContext(), "onStop Called", Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onDestroy()
    {
        super.onDestroy();
        Toast toast = Toast.makeText(getApplicationContext(), "onDestroy Called", Toast.LENGTH_LONG);
        toast.show();
    }

}
```
# activity_main.java
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="HelloWorld!"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>
```

## OUTPUT
![image](https://github.com/RANJEETH17/lifecyclemethods/assets/120718823/4696a1af-f5c9-439e-a9d0-cf4a493d1a3a)
![image](https://github.com/RANJEETH17/lifecyclemethods/assets/120718823/27a9dcac-82a9-4453-9a7e-43edad2778ef)


![image](https://github.com/RANJEETH17/lifecyclemethods/assets/120718823/7cb84140-db73-4dbd-adbb-54336206f7e9)
![image](https://github.com/RANJEETH17/lifecyclemethods/assets/120718823/33e1965f-5705-4f1d-9925-143c890044f0)
![image](https://github.com/RANJEETH17/lifecyclemethods/assets/120718823/438746a7-02d5-4b05-a9e7-754ca12c8a79)
![image](https://github.com/RANJEETH17/lifecyclemethods/assets/120718823/a279854e-9189-42a1-937d-cb7bad916a2a)
![image](https://github.com/RANJEETH17/lifecyclemethods/assets/120718823/3177f717-4f94-4042-bcaf-3e82782b1051)
![image](https://github.com/RANJEETH17/lifecyclemethods/assets/120718823/53ff377b-aa44-413d-af5b-f1dfa140e84d)











## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
