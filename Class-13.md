## Read:13 - Local Storage

In the early stages of local storage, the web used cookies. Their were a lot of issues
which involved being limited to the amount of data that could be stored. Cookies 
could only store 4kb of data and it also bogs down your application due to sending and resending the same data over and over. 

HTML5 changed this, it created a way for the user to store data locally. Within the client
web browser. Even if the user leaves the page or even closes their browser, the data persists.
Despite it being saved it does not make it to the server. 

Data stored locally gets saves as a string. When retreiving data, the developer is responsible for 
converting the string to the necessary data type. If it is a boolean, int etc. 

setItem() = Calling a named key that already exists will overwrite the previous value.
getItem() = Calling a non existent key will return null.

To delete the or clear the entire storage area: 
interface Storage {
    deleter void removeItem(in DOMString key);
    void clear();
};

To retreive the total number of values in the storage area: 
interface Storage {
    readonly attribute unsigned long length;
    getter DOMString key(in unsinged long index);
};

Local Storage is great for storing and calling data for a developer. Storing a clients
game place is a excellent example. If the user is in the middle of a game and leaves the page. They are able
to go back to the site and continue where they left off. 
