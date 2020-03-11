#### Earthdate 10032020

# Local Storage for Web Applications

Since the earliest times of the internet, web applications' greatest hinderance when compared to local application has been storage. In 2011, HTML5 changed the game.

The earliest form of persistent storage was cookies. Unfortunately, there are some pretty big drawbacks to cookies:
  - cookies are transmitted with every HTTP request, potentially slowing down application load
  - The data they transmit is unencrypted unless your entire application is served on an **SSL (Security Socket Layer)** or **TLS (Transport Layer Security)**
  - stoage is limited to 4KB

in 2007, Google launched an open source web browser plugin called **Gears**. Gears provides an **API (Application Program Interface)** to an embedded SQL database. It gains permission from the user once, then hs access to storing *unlimited* amounts of data per domain in this database.

While grand in its capabilities, the fact that it neccessitates a third-party plugin makes this storage option still less than optimal.  

(Enter **Web Storage**)

**Web Storage** or **HTML5 Storage** is a way for web pages to store named key/value pairs locally, within a users browser. It is like cookies in that the data persists even after a user navigates away from a web site, or even closes or exits their browser. Unlike cookies, the data is never transmitted to a remote web server. *And* it is implemented natively, so no additional plugins or applications are neccessary for it to function. As of now, almost all of the world's most popular web browsers support it, too.

And accessing it is quite simple through JavaScript! Here's a code example accessing the storage:

```javascript
function saveGameState() {
    if (!supportsLocalStorage()) { return false; }
    localStorage["halma.game.in.progress"] = gGameInProgress;
    for (var i = 0; i < kNumPieces; i++) {
	localStorage["halma.piece." + i + ".row"] = gPieces[i].row;
	localStorage["halma.piece." + i + ".column"] = gPieces[i].column;
    }
    localStorage["halma.selectedpiece"] = gSelectedPieceIndex;
    localStorage["halma.selectedpiecehasmoved"] = gSelectedPieceHasMoved;
    localStorage["halma.movecount"] = gMoveCount;
    return true;
}
``` 
This piece of code iterates every time an action is performed in this particular game, and if the browser has access to the HTML5 storage, it saves the current game state. And this game state can be accessed even if the browser is quickly closed or errors out.

The potential for this ability is amazing, allowing developers to create states of their application that can persist for a faster and more fluid user experience or by remembering user inputs. And these technologies are still fast-evolving.