# PHP Cookies

Cookies are small pieces of data that are stored on the client-side (in the user's browser) and sent to the server with each HTTP request. They are commonly used for storing user preferences, session identifiers, and other information to personalize the user experience. In this chapter, we'll explore how to work with cookies in PHP.

## 1. Setting Cookies
PHP provides a built-in function setcookie() to set cookies in the user's browser. The setcookie() function accepts several parameters, including the cookie name, value, expiration time, path, domain, and security options.

```php
setcookie("username", "John Doe", time() + 3600, "/");
```

### In this example:

* The cookie name is "username".
* The cookie value is "John Doe".
* The expiration time is set to one hour from the current time (time() + 3600).
* The cookie is accessible from the root path ("/") of the domain.

## 2. Retrieving Cookies

You can retrieve cookie values using the $_COOKIE superglobal array. Once a cookie is set, its value will be available in the $_COOKIE array on subsequent page loads.

```php
$username = $_COOKIE["username"];
```

## 3. Deleting Cookies

To delete a cookie, you can use the setcookie() function with an expired expiration time. Setting the expiration time to a past timestamp effectively removes the cookie from the user's browser.

```php
setcookie("username", "", time() - 3600, "/");
```



