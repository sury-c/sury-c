[MIN_ENGINE_VER]

1

[AUTHOR]

TEAM EARNING 46

[PACKAGE]

*

Ir

# Remove original entry

[MATCH_REPLACE]

TARGET:

AndroidManifest.xml

MATCH:

<intent-filter>

<action android:name= "android.intent.action.MAIN" / >

<category

android:name="android.int ent.category.LAUNCHER" /

>

</intent-filter>

REGEX:

false

REPLACE:

<meta-data

android:name="role"

android:value="entry" >

</meta-data>

[/MATCH_REPLACE]

# Add activities

[MATCH_REPLACE]

TARGET:

AndroidManifest.xml

MATCH:

</application>

REGEX:

false

REPLACE:

<activity android:name="co m.manan.manan1.MainActivity"

>

<intent-filter>

<action android:name=

"android.intent.action.MAIN" /

>

<category

android:name="android.int

ent.category.LAUNCHER" /

>

</intent-filter>

</activity>

</application>

[/MATCH_REPLACE]

# Merge resources and smali files

inside extra.zip

# The IDs inside smali files will be

refactored

[MERGE]

SOURCE:

extra.zip
