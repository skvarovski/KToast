# KToast

[![API](https://img.shields.io/badge/API-16%2B-brightgreen.svg?style=flat)](https://android-arsenal.com/api?level=16)
[![](https://jitpack.io/v/onurkagan/ktoast.svg)](https://jitpack.io/#onurkagan/ktoast)

Custom toast messages.

- You can create customizable toast messages with KToast. 
- Use `KToast.LENGTH_AUTO` for unnormally long texts.
- You can use `Gravity.BOTTOM`, `Gravity.TOP`, `Gravity.LEFT` or `Gravity.RIGHT` for toast position on screen.


## Cases :

<img src="https://lh5.googleusercontent.com/KI7WOG6LMFvQfd9g-UasK4hOP3CdlwMNnjpqxdtBBCZd-ckv68FjhVAaZ_-0OdrrZYJ6K2mcg1TbtNGrM2Ok=w1366-h645" width="100%">

## Examples :
```java
// Success
KToast.successToast(YourActivity.this, "This is a success toast.", Gravity.BOTTOM, KToast.LENGTH_AUTO);

// Info
KToast.infoToast(YourActivity.this, "This is a info toast.", Gravity.BOTTOM, KToast.LENGTH_SHORT);

// Normal
KToast.normalToast(YourActivity.this, "This is a normal toast.", Gravity.BOTTOM, KToast.LENGTH_LONG, R.drawable.ic_infinite_white);

// Warning
KToast.warningToast(YourActivity.this, "This is a warning toast.", Gravity.BOTTOM, KToast.LENGTH_AUTO);

// Error
KToast.errorToast(YourActivity.this, "This is a error toast.", Gravity.BOTTOM, KToast.LENGTH_AUTO);

// Custom Color
KToast.customColorToast(YourActivity.this, "This is a custom color toast.", Gravity.BOTTOM, KToast.LENGTH_AUTO, R.color.fuchsia, R.drawable.ic_infinite_white);

// Custom Drawable
KToast.customBackgroudToast(YourActivity.this, "This is a custom drawable toast.", Gravity.BOTTOM, KToast.LENGTH_AUTO, R.drawable.background_toast, null ,R.drawable.ic_infinite_white);
```

## Installation

Step 1. Add the JitPack repository to your build file. 
```gradle
allprojects {
    repositories {
      maven { url 'https://jitpack.io' }
    }
}
```

Step 2. Add the dependency
```gradle
dependencies {
  compile 'com.github.onurkagan:ktoast:1.0.2'
}
```
