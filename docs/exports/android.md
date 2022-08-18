---
title: Export to Android
---

# Export to Android

---
## Table Of Content
* Install Export Template 
  * [Install Export Template From Official Website](#install-export-template-from-official-website)
* Add Export Config
  * Debug keystore
---


### Install Export Template From Official Website
* Go to the page: https://godotengine.org/download

### Add Export Config
* Create debug keystore, Android needs a debug keystore file to install to devices and distribute non-release APKs.
```bash
keytool -keyalg RSA -genkeypair -alias androiddebugkey -keypass android -keystore debug.keystore -storepass android -dname "CN=Android Debug,O=Android,C=US" -validity 9999 -deststoretype pkcs12
# the user is androiddebugkey
# the password is android
```

---

