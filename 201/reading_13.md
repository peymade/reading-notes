# Reading 13

## THE PAST, PRESENT & FUTURE OF LOCAL STORAGE FOR WEB APPLICATIONS

Cookies were invented in the early days of web storage, and store small amounts of data. They slow down web applications and send unencrypted data. This is counter to what one wants in web storage- which is lots of space and speed. 

HTML5 attempted to make an API that could work without third-party plugins, across lots of browsers. 

HTML5 Storage = Local Storage = DOM Storage = Web Storage
- Stores key/value pairs in the client's browser
- Data stays even after navigating away or refreshing
- Works with many browsers, including chrome, IE, and safari
- Access HTML5 Storage with `localStorage` object on the `window` object.  
- Make sure to check that the browser supports HTML5 storage. You can use "Modernizer" to do so. 

### Using HTML5 Local Storage

- Data is stored in key/value pairs. The key is a string, and the value can be any data type supported by JavaScript.
- Use parseInt() or similar functions to coerce data types- since it will automatically be stored as a string
- Call `setItem()` to overwrite a previous value in a key
- Call `getItem()` on a non-existent key to return null
- Values in storage can be iterated through with index

### Tracking Changes to HTML5 Storage Area

- When storage area changes, you can add the `storage` event to alert you. First check though if the `localStorage` object is supported. 
- A StorageEvent object has these properties:
  - `key` is a string- named key that was changed
  - `oldValue` any data type- the previous value, or null for new items
  - `newValue` any data type- the new value, or null for removed item
  - `url` is a string- the page that called the method that changed the object

By default, each origin gets 5 megabytes. You can't ask for more storage space, and you will get an error if you exceed it. 

### HTML5 Storage in Action

Progress or data can be stored locally in the browser. In the game example linked on [This Site](http://diveinto.html5doctor.com/storage.html) each time a move is made, a function is called to store that information. The game can check if there is a previous game to resume, and then can load the data from localStorage. 
 
### Beyond Name Key Value Pairs

*SQL = Structured Query Language*
- Used to communicate with databases. However, it is not completely standarized. 

*Indexed Database API*
- This is similar to SQL, but is has no structured query language. 
- Not currently widely used



[Home](https://peymade.github.io/reading-notes/)