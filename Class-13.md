## “The Past, Present, and Future of Local Storage for Web Applications”

#### ersistent local storage is one of the areas where native client applications have held an advantage over web applications.
#### web applications have had none of these luxuries.
#### they have three potentially dealbreaking downsides:
1. a lot of storage space
2. on the client
3. that persists beyond a page refresh
4. and isn’t transmitted to the server


### A BRIEF HISTORY OF LOCAL STORAGE HACKS BEFORE HTML5

#### userData allows web pages to store up to 64 KB of data per domain, in a hierarchical XML-based structure.

#### In 2002, Adobe introduced a feature in Flash 6 that gained the unfortunate and misleading name of “Flash cookies.” Within the Flash environment, the feature is properly known as Local Shared Objects.

#### In 2007, Google launched Gears, an open source browser plugin aimed at providing additional capabilities in browsers. 

![storageWork](https://lh3.googleusercontent.com/proxy/pUFF5Lk5XDG0gek4fKYzlhEPzlgWPzF52zvVo7bbfYPEvYicT25wurmRx6DZl-gt4h77TKMsXNWvH3CgR0BJfOUQbNASR-ll7Is8SjF5xaZHnhjl)

### INTRODUCING HTML5 STORAGE

#### HTML5 STORAGE SUPPORT :
1. IE 8.0+
2. FIREFOX 3.5+
3. SAFARI 4.0+	
4. CHROME 4.0+	
5. OPERA 10.5+	
6. IPHONE 2.0+	
7. ANDROID 2.0+

##### Example :
###### if (Modernizr.localstorage) { // window.localStorage is available! } else { // no native support for HTML5 storage :(// maybe try dojox.storage or a third-party solution }


#### The storage event is supported everywhere the localStorage object is supported, which includes Internet Explorer 8. IE 8 does not support the W3C standard addEventListener

#### “QUOTA_EXCEEDED_ERR” is the exception that will get thrown if you exceed your storage quota of 5 megabytes. “No” is the answer to the next obvious question, 

![Storage](https://miro.medium.com/max/1134/1*OpOBcqJpawgs4ehT1eKZnA.png)