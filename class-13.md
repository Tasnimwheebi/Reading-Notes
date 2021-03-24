# INTRODUCING HTML5 STORAGE 
“HTML5 Storage” is a specification named Web Storage, which was at one time part of the HTML5 specification proper, but was split out into its own specification for uninteresting political reasons. it’s a way for web pages to store named key/value pairs locally, within the client web browser.
## USING HTML5 STORAGE
HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or float.

- function supports_html5_storage() {
         try {

      return 'localStorage' in window && window ['localStorage'] !== null;
          } catch (e) {
                     return false;
             }
        }
        Instead of writing this function yourself, you can use Modernizr to detect support for      HTML5 Storage.

        if (Modernizr.localstorage) {
         // window.localStorage is available!
        } else {
         // no native support for HTML5 storage :(
         // maybe try dojox.storage or a third-party solution
        }`
## TRACKING CHANGES TO THE HTML5 STORAGE AREA
If you want to keep track programmatically of when the storage area changes, you can trap the storage event. The storage event is fired on the window object whenever setItem(), removeItem(), or clear() is called and actually changes something.
## STORAGEEVENT OBJECT
- key(string) :	the named key that was added, removed, or modified
- oldValue (any) : the previous value (now overwritten), or null if a new item was added
- newValue(	any) : the new value, or null if an item was removed
- url(string):the page which called a method that triggered this change
## HTML5 STORAGE IN ACTION
There’s a small problem with the game: if you close the browser window mid-game, you’ll lose your progress. But with HTML5 Storage, we can save the progress locally, within the browser itsel.
