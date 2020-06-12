# hacker101

## Stuff I learned

- SQL Injection
- XSS
- Bruteforcing
- Some crypto-attacks
- Basic Android Hacking

### SQL Injection

- Lets you run SQL through unsanitized inputs.
- [sqlmap](http://sqlmap.org/) is a useful tool to get database details, if you have the database creds.
- [Burp Suite](https://portswigger.net/burp) lets you intercept and examine requests closely.

### XSS

- Lets you execute JS on the browser using unsanitized inputs.
- Image XSS was also a neat technique.

### Bruteforcing

- [Burp Suite](https://portswigger.net/burp) does allow bruteforcing, but the community version runs really slow. Hydra is a much faster alternative.

```
hydra -l gg -P ez.txt <server-ip/url> http-post-form "/login:username=^USER^&password=^PASS^:<error text>"
```

- We hit a match when the response returned doesn't contained the specified error text.

### Some crypto attacks

- Padding Oracle Attack

### Basic Android Hacking

#### Setup

- You'd want to set up an emulator to test the app on.
- [Android studio](https://developer.android.com/studio) can be used to perform a lot useful tasks, like creating an emulator, decompiling an apk into dex files, within a GUI interface.
- [apktool](https://ibotpeaches.github.io/Apktool/) can decompile an apk, among other things. Its pretty useful if you're low on RAM, as running both the emulator and Android Studio may cause your computer to hang.
- [dex2jar](https://github.com/pxb1988/dex2jar) converts dex files (retrieved from apk using apktool) to jar files.
- [jd-gui](https://github.com/java-decompiler/jd-gui) can be used to view the jar files as java code.
- [Burp Suite](https://portswigger.net/burp), with some [setup](https://portswigger.net/support/installing-burp-suites-ca-certificate-in-an-android-device), lets you intercept requests.
  