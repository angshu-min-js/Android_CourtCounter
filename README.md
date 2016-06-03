Court Counter App
===================================

Keeps track of basketball scores for two teams. Used in the Udacity Android for Beginners course.

Pre-requisites
--------------

- Android SDK v22
- Android Build Tools v22.0.1
- Android Support Repository v22.1.1

Getting Started
---------------

This sample uses the Gradle build system. To build this project, use the
"gradlew build" command or use "Import Project" in Android Studio.

Support
-------

- Google+ Community: https://plus.google.com/communities/105153134372062985968
- Stack Overflow: http://stackoverflow.com/questions/tagged/android

Patches are encouraged, and may be submitted by forking this project and
submitting a pull request through GitHub. Please see CONTRIBUTING.md for more details.

License
-------

Copyright 2015 The Android Open Source Project, Inc.

Licensed to the Apache Software Foundation (ASF) under one or more contributor
license agreements.  See the NOTICE file distributed with this work for
additional information regarding copyright ownership.  The ASF licenses this
file to you under the Apache License, Version 2.0 (the "License"); you may not
use this file except in compliance with the License.  You may obtain a copy of
the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  See the
License for the specific language governing permissions and limitations under
the License.

-------------------------------------------------------------------------------
##Views: 
- Indiviual views (rectange) make up the layout of the android screen. Basic building block of the App.
- Types: Text View, Image View, Button

###xml view:

```
<TextView
	android:text="Welcome!"
	android:background="@android:color/darker_gray"
	android:layout_width="150dp" #"wrap_content" for wrapping
	android:layout_height="75dp" 
	android:textSize="45sp"		/> #sp for font or use 					 #android:textAppearance="?android:textAppearanceSmall"
	 #android:textColor=""
```					   

- Density Independent Pixel (dp): 48dp recommended
- Google.com/design/spec/style/typography
- developer.android.com

### Layouts:

- viewgroups
	- Relative Layout, Linear Layout

```
<LinearLayout
	android:orientation="vertical"
	android:layout_width="wrap_content"
	android:layout_height="wrap_content">

	<TextView
		android:text="Guest List"
		android:layout_width="wrap_content" #"match_parent"
		android:layout_height="wrap_content"  />

	<TextView
		android:text="Angshuman"
		android:layout_width="wrap_content"
		android:layout_height="wrap_content"  />
</LinearLayout>
```

####android:layout_height="0 dp" #android:layout_weight="1"

- Relative Layout

```
<RelativeLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_alignParentRight="true"
        android:layout_alignParentTop="true"
        android:textAppearance="?android:textAppearanceLarge"
        android:text="Happy" />

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_alignParentBottom="true"
        android:layout_alignParentLeft="true"
        android:textAppearance="?android:textAppearanceLarge"
        android:text="Birthday" />

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:textAppearance="?android:textAppearanceLarge"
        android:text="To You" />

</RelativeLayout>
```
###android:id="@+id/<name>"

