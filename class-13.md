# THE PAST, PRESENT & FUTURE OF LOCAL STORAGE FOR WEB APPLICATIONS

## Diving In
*ersistent local storage is one of the areas where native client applications have held an advantage over web applications. For native applications, the operating system typically provides an abstraction layer for storing and retrieving application-specific data like preferences or runtime state. These values may be stored in the registry, INI files, XML files, or some other place according to platform convention. Historically, web applications have had none of these luxuries. Cookies were invented early in the web’s history, and indeed they can be used for persistent local storage of small amounts of data.*

##A BRIEF HISTORY OF LOCAL STORAGE HACKS BEFORE HTML5
*There was only one browser at first: Internet Explorer. At least, that's what Microsoft wanted the rest of the world to believe. To that aim, Microsoft created a lot of items during the First Great Browser Wars and included them in their browser-to-end-all-browser-wars, Internet Explorer. DHTML Behaviors was one of these things, and userData was one of these behaviors.*

*In a hierarchical XML-based structure, userData allows web pages to hold up to 64 KB of data per domain. (Trusted domains, such as intranet sites, have ten times the storage capacity.) And, hey, 640 KB should plenty for most people.) There is no permissions dialog in Internet Explorer, and there is no way to increase the amount of storage available.*

*the problem that HTML5 set out to solve: to provide a standardized API, implemented natively and consistently in multiple browsers, without having to rely on third-party plugins.*

## Introducing HTML5 Storage
*HTML5 local storage is a component of the Web storage application programming interface. It is a method by which Web pages locally store named key/value pairs inside a client's Web browser.*

## USING HTML5 STORAGE
*HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like `parseInt()` or `parseFloat()` to coerce your retrieved data into the expected JavaScript datatype.*

+ Calling `setItem()` with a named key that already exists will silently overwrite the previous value.
+ alling `getItem()` with a non-existent key will return null rather than throw an exception.

*Like other JavaScript objects, you can treat the localStorage object as an associative array. Instead of using the `getItem()` and `setItem()` methods, you can simply use square brackets.*


```
var foo = localStorage["bar"];
// ...
localStorage["bar"] = foo;

```


**The syntax for removing the "lastname" localStorage item is as follows:** 
+ `localStorage.removeItem("lastname");`

*Finally, there is a property to get the total number of values in the storage area, and to iterate through all of the keys by index (to get the name of each key).*


```
interface Storage {
  readonly attribute unsigned long length;
  getter DOMString key(in unsigned long index);
};
```

+ If you call key() with an index that is not between 0–(length-1), the function will return null.


## Tracking Changes to the HTML5 Storage Area
*If you want to keep track programmatically of when the storage area changes, you can trap the storage event. For example, if you set an item to its existing value or call `clear()` when there are no named keys, the storage event will not fire, because nothing actually changed in the storage area. The storage event is supported everywhere the localStorage object is supported, which includes Internet Explorer 8. If you prefer to use jQuery or some other JavaScript library to register your event handlers, you can do that with the storage event, too.*

```
if (window.addEventListener) {
  window.addEventListener("storage", handle_storage, false);
} else {
  window.attachEvent("onstorage", handle_storage);
};
```

*The `handle_storage` callback function will be called with a `StorageEvent object`, except in Internet Explorer where the event object is stored in `window.event.function`*

```
function handle_storage(e) {
  if (!e) { e = window.event; }
}

```

## Limitations in Current Browsers
*in order of importance, are “5 megabytes,” “QUOTA_EXCEEDED_ERR,” and “no.”“5 megabytes” is how much storage space each origin gets by default. One thing to keep in mind is that you’re storing strings, not data in its original format. Some browsers (like Opera) allow the user to control each site’s storage quota, but it is purely a user-initiated action, not something that you as a web developer can build into your web application.*

## Beyond Named Key-Value Pairs: Competing Visions
*While the past is littered with hacks and workarounds, the present condition of HTML5 Storage is surprisingly rosy. Oh joy!The Web SQL Database specification has been implemented by four browsers and platforms. Sure, there is an actual SQL specification (it’s called SQL-92), but there is no database server in the world that conforms to that and only that specification. An object store shares many concepts with a SQL database. You can select a subset of records, then enumerate them with a “cursor.” Changes to the object store are handled within `transactions`.*





