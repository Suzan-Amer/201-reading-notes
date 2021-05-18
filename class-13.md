# Read: 13 - Local Storage

# THE PAST, PRESENT & FUTURE OF LOCAL STORAGE FOR WEB APPLICATIONS

## what is **Local Storage**
### ersistent local storage is one of the areas where native client applications have held an advantage over web applications. For native applications, the operating system typically provides an abstraction layer for storing and retrieving application-specific data like preferences or runtime state.

### web applications have had none of these luxuries. Cookies were invented early in the web’s history, and indeed they can be used for persistent local storage of small amounts of data. But they have three potentially dealbreaking downsides:

* *Cookies are included with every HTTP request*, thereby slowing down your web application by needlessly transmitting the same data over and over
* *Cookies are included with every HTTP request*, thereby sending data unencrypted over the internet (**unless your entire web application is served over SSL**)
* *Cookies are limited to about 4 KB of data* — enough to slow down your application, but not enough to be terribly useful

## What we really want ??

* a lot of storage space
* on the client
* that persists beyond a page refresh
* and isn’t transmitted to the server

### **userData** allows web pages to store up to 64 KB of data per domain, in a hierarchical XML-based structure

### In 2002, Adobe introduced a feature in Flash 6 that gained the unfortunate and misleading name of “Flash cookies.” Within the Flash environment, the feature is properly known as Local Shared Objects. Briefly, it allows Flash objects to store up to 100 KB of data per domain.

## INTRODUCING HTML5 STORAGE
### What I will refer to as “HTML5 Storage” is a specification named Web Storage, which was at one time part of the HTML5 specification proper, but was split out into its own specification for uninteresting political reasons. Certain browser vendors also refer to it as “Local Storage” or “DOM Storage.” The naming situation is made even more complicated by some related, similarly-named, emerging standards that I’ll discuss later in this chapter.

## HTML5 STORAGE SUPPORT
![img](https://imgs.developpaper.com/imgs/2885411287-587d9361eda0f_articlex.png)


## check for HTML5 Storage

*function supports_html5_storage*() {
  try {
    return '*localStorage*' in window && window['*localStorage*'] !== null;
  } catch (e) {
    return false;
  }
}

## USING HTML5 STORAGE
### HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like parseInt() or parseFloat() to coerce your retrieved data into the expected JavaScript datatype.

**interface Storage {**
 **getter any getItem(in DOMString key);**
 **setter creator void setItem(in DOMString key, in any data);**
};

## TRACKING CHANGES TO THE HTML5 STORAGE AREA
### If you want to keep track programmatically of when the storage area changes, you can trap the storage event. The storage event is fired on the window object whenever setItem(), removeItem(), or clear() is called and actually changes something. For example, if you set an item to its existing value or call clear() when there are no named keys, the storage event will not fire, because nothing actually changed in the storage area.

### The storage event is supported everywhere the localStorage object is supported, which includes Internet Explorer 8. IE 8 does not support the W3C standard addEventListener (although that will finally be added in IE 9). Therefore, to hook the storage event, you’ll need to check which event mechanism the browser supports. (If you’ve done this before with other events, you can skip to the end of this section. Trapping the storage event works the same as every other event you’ve ever trapped. If you prefer to use jQuery or some other JavaScript library to register your event handlers, you can do that with the storage event, too.)

if (window.addEventListener) {
  window.addEventListener("storage", handle_storage, false);
} else {
  window.attachEvent("onstorage", handle_storage);
};

## STORAGEEVENT OBJECT
### 
![i](https://image.slidesharecdn.com/html5localstorage-140511235722-phpapp01/95/html5-local-storage-12-638.jpg?cb=1399852926)

## LIMITATIONS IN CURRENT BROWSERS
### in talking about the history of local storage hacks using third-party plugins, I made a point of mentioning the limitations of each technique, such as storage limits. I just realized that I haven’t mentioned anything about the limitations of the now-standardized HTML5 Storage. I’ll give you the answers first, then explain them. The answers, in order of importance, are “5 megabytes,” “QUOTA_EXCEEDED_ERR,” and “no.”


## BEYOND NAMED KEY-VALUE PAIRS: COMPETING VISIONS
### While the past is littered with hacks and workarounds, the present condition of HTML5 Storage is surprisingly rosy. A new API has been standardized and implemented across all major browsers, platforms, and devices. As a web developer, that’s just not something you see every day, is it? But there is more to life than “5 megabytes of named key/value pairs,” and the future of persistent local storage is… how shall I put it… well, there are competing visions.

### One vision is an acronym that you probably know already: SQL. In 2007, Google launched Gears, an open source cross-browser plugin which included an embedded database based on SQLite. This early prototype later influenced the creation of the Web SQL Database specification. Web SQL Database (formerly known as “WebDB”) provides a thin wrapper around a SQL database, allowing you to do things like this from JavaScript: