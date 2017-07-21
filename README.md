# splash
McNally Developers Android Library for Splash Screen

![screenshot](http://i.imgur.com/OWG9NlF.png)

You can download from maven central.

    dependencies {
      compile 'com.mcnallydev.library:splash:0.0.4'
    }

Add to **AndroidManifest.xml**.

    <activity
      android:name="com.chocoyo.labs.splash.SplashActivity"
      android:configChanges="keyboardHidden|orientation"
      android:theme="@style/AppTheme.NoActionBar.Fullscreen">
        <intent-filter>
            <action android:name="android.intent.action.MAIN" />
            <category android:name="android.intent.category.LAUNCHER" />
        </intent-filter>
    </activity>

Add to **styles.xml**

    <style name="AppTheme.NoActionBar">
        <item name="windowNoTitle">true</item>
        <item name="windowActionBar">false</item>
    </style>

    <style name="AppTheme.NoActionBar.Fullscreen">
        <item name="windowNoTitle">true</item>
        <item name="windowActionBar">false</item>
        <item name="android:windowFullscreen">true</item>
        <item name="android:windowContentOverlay">@null</item>
    </style>

Add to **strings.xml**

    <string name="mcnallydev_library_splash_class_name">com.package.MainActivity</string>

The value on **mcnallydev_library_splash_class_name** is the class name to open after **SplashActivity** close.
