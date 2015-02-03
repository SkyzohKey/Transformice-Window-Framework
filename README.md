![Project Maintened](https://img.shields.io/badge/Project-maintened-green.svg)    ![Version 0.0.1](https://img.shields.io/badge/Version-0.0.1-green.svg)

Transformice-Window-Framework
=============================

Installation :
--------------
  * Copy the content of the twf.lua before all your code.
  * Enjoy availables functions. :3

Examples of availables functions (proto) :
------------------------------------------

  * **Create a new popup (if id exists it will update the one with this id) :**
  ``` lua  
  twf.ui.createPopup(int id, string title, string content, string targetPlayer,
                     array buttons, boolean closable, int x, int y, int width,
                     int height, hex backgroundColor, hex borderColor, 
                     double backgroundAlpha, boolean fixedPos);
  ```
  
  * **Remove a popup (nil in targetPlayer will remove for all) :**
  ``` lua
  twf.ui.removePopup(int id, string targetPlayer);
  ```
  
  * **Create a new label :**
  ``` lua
  twf.ui.createLabel(int id, string text, string targetPlayer, int x, int y);
  ```

Examples of availables triggers :
---------------------------------

 * **Trigger when player want to close a popup :**

 ``` lua
 function eventTextAreaCallback (textAreaId, playerName, callback)
   twf.trigger.popupClose(textAreaId, playerName, callback);
   
   -- Your code goes here.
 end
 ```

More features for later !
-------------------------
