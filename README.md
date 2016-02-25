# JavaScript
This is AppBeat public repository for useful JavaScript libraries that we develop for our [AppBeat project](https://appbeat.io) project (web application and framework for easy uptime and performance monitoring).

AppBeat.Email.js and AppBeat.Email.min.js implements easy to use method AppBeat.Email.isDisposable which can be used to check if email address is disposable (also known as burner or temporary email address).

Library does not depend on any external library. If you find out about new disposable domains you can add them or you can contact us.

Usage examples:

```js
AppBeat.Email.isDisposable('something@sharklasers.com'); //returns true
AppBeat.Email.isDisposable('something@mailinator.com'); //returns true
AppBeat.Email.isDisposable('   something@mailinator.com   '); //returns true
AppBeat.Email.isDisposable('@mailinator.com'); //returns true
AppBeat.Email.isDisposable('mailinator.com'); //returns true
AppBeat.Email.isDisposable('unknown-domain.some-domain'); //returns false
AppBeat.Email.isDisposable('something@unknown-domain.some-domain'); //returns false
AppBeat.Email.isDisposable('something@gmail.com'); //returns false (whitelisted)
AppBeat.Email.isDisposable('something@outlook.com'); //returns false (whitelisted)
```
