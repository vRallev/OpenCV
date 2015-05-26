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
    compile 'org.opencv:opencv-android:2.4.8'
}
```

Compiling the library
---------------------

You can also clone the library and add it your local maven repository.
 
 1. Clone the repository.
 2. In the root project folder (`opencv-library`) run `gradle uploadArchives`.
 3. Add the same dependency as above:

```groovy
repositories {
    mavenLocal()
}

dependencies {
    compile 'org.opencv:opencv-android:2.4.8'
}
``` 

License
-------

	By downloading, copying, installing or using the software you agree to this license.
	If you do not agree to this license, do not download, install,
	copy or use the software.


	                          License Agreement
	               For Open Source Computer Vision Library
	                       (3-clause BSD License)

	Copyright (C) 2000-2015, Intel Corporation, all rights reserved.
	Copyright (C) 2009-2011, Willow Garage Inc., all rights reserved.
	Copyright (C) 2009-2015, NVIDIA Corporation, all rights reserved.
	Copyright (C) 2010-2013, Advanced Micro Devices, Inc., all rights reserved.
	Copyright (C) 2015, OpenCV Foundation, all rights reserved.
	Copyright (C) 2015, Itseez Inc., all rights reserved.
	Third party copyrights are property of their respective owners.

	Redistribution and use in source and binary forms, with or without modification,
	are permitted provided that the following conditions are met:

	  * Redistributions of source code must retain the above copyright notice,
	    this list of conditions and the following disclaimer.

	  * Redistributions in binary form must reproduce the above copyright notice,
	    this list of conditions and the following disclaimer in the documentation
	    and/or other materials provided with the distribution.

	  * Neither the names of the copyright holders nor the names of the contributors
	    may be used to endorse or promote products derived from this software
	    without specific prior written permission.

	This software is provided by the copyright holders and contributors "as is" and
	any express or implied warranties, including, but not limited to, the implied
	warranties of merchantability and fitness for a particular purpose are disclaimed.
	In no event shall copyright holders or contributors be liable for any direct,
	indirect, incidental, special, exemplary, or consequential damages
	(including, but not limited to, procurement of substitute goods or services;
	loss of use, data, or profits; or business interruption) however caused
	and on any theory of liability, whether in contract, strict liability,
	or tort (including negligence or otherwise) arising in any way out of
	the use of this software, even if advised of the possibility of such damage.