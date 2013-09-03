OpenCV Java project for Android
===============================

The OpenCV library for Android as Gradle project.

All credit goes to http://opencv.org/ I've took their library and exported it as `.aar` library. Now you can easily use OpenCV in a Gradle / Android Studio project.

Usage Maven Repo
----------------

I've uploaded the `.aar` in my maven repository. You only need to add following lines to your `build.gradle` to add the dependency:
```groovy
repositories {
    maven {
        url 'https://raw.github.com/vRallev/mvn-repo/master/'
    }
}

dependencies {
    compile 'org.opencv:opencv-android:2.4.6'
}
```

Compiling the library
---------------------

You can also clone the library and add it your local maven repository.
 
 1. Clone the repository.
 2. In the root project folder (`OpenCV`) run `gradle uploadArchives`.
 3. Add the same dependency as above:

```groovy
repositories {
    mavenLocal()
}

dependencies {
    compile 'org.opencv:opencv-android:2.4.6'
}
``` 