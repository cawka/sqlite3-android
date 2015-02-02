Sqlite3 for Android NDK
=======================

Usage example

App source:

    ├── AndroidManifest.xml
    ├── java
    │   ├── ...
    │   └── ...
    ├── jni
    │   ├── Android.mk
    │   └── Application.mk
    └── res
        ├── ...
        └── ...

Clone or create submodule:

    git submodule add http://github.com/cawka/sqlite3-android jni/sqlite3

In jni/Android.mk, add

    include $(LOCAL_PATH)/sqlite3/Android.mk

Afterwards, sqlite3 can be added to `LOCAL_STATIC_LIBRARIES` for other
static or shared libraries
