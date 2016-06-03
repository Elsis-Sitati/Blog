---
layout: post
title: How to move to a different activity in android 
---

An activity is what you see on your android screen.Activities can be compared to web pages in web
programming ie about page,contacts page etc.In the same way clicking to a button or link directs you to a 
different page,clicking a button in android can direct you to a different activity.I am going to take you through
the process of writing code that will enable you to move to a different activity in android.

### Step 1
Attach  an on Click Listener to a button 

    <Button
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Login"
        android:layout_gravity="center_vertical|center_horizontal"
        android:onClick="goToNextActivity"

        />
Android studio will prompt you to create an OnClick Event Handler.Choose this option and specify what class you want that event handler to be generated. You will get a method like the one below on that activity class

    public void goToNextActivity(View view) {
       
    }
The last step is to define an intent inside that method.

    public void goToNextActivity(View view) {
        Intent intent =new Intent(getApplicationContext(),Images.class);
        startActivity(intent);
    }
    
This piece of code basically says "move from this class and go to the Images class"

And we are done.You can now move to a different Activity once you click your button.
