# Hebrew in Windows Console

* install win_unicode_console module:

      pip install win_unicode_console

* find out where your [usercustomize module](<https://docs.python.org/3/tutorial/appendix.html#the-customization-modules>) is. In a python interactive shell, run the following commands. They will return a folder name:

      import site
      site.getusersitepackages()
      
* If the folder doesn't exist, create it. 

* Create a `usercustomize.py` file in the folder (if there isn't one already)

* Add the following lines to your `usercustomize.py`:

      import win_unicode_console
      win_unicode_console.enable()

