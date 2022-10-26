# $\color{red}{C}\color{orange}{O}\color{yellow}{L}\color{green}{O}\color{blue}{R}\color{aqua}{I}\color{purple}{N}\color{indigo}{G}$

## Installation
- Using [PIP](https://pip.pypa.io/en/stable/) package manager
  ```bash
  pip install Coloring
  ```
- Downloading from github
  ```
    Drag and drop the coloring.py in your projects and import it 
  ``` 

## Usage 
- in the coloring class there is some color constants that can be used like
```py
  >>print(coloring.RED + "Your Text")
  ```
 *type "str"*
 
 - You can also type directly the hex or rgb code (letters for hex must be upper)
 
 ```py
   >>print(coloring.rgb((255,0,0)) + "YourText")
 ```
  ```py
    >>print(coloring.hex("DC143C") + "YourText")
 ```
   >$\color{red}{Your}\color{red}{Text}$

    
- You can  create a string with color codes using a separators(by default = "&") 

 ```py
    >>print(coloring.color("&DC143C&YourText"))
 ```
  ```py
    >>print(coloring.color("&255,0,0&YourText", rgb=True))
    
 ```
 >$\color{red}{Your}\color{red}{Text}$

- Notice if you use a color and don't reset it, it will use it for everything after the call.

 ```py
    >>print(coloring.color("&DC143C&YourText" + "YoursecondText)
 ```
 >$\color{red}{Your}\color{red}{Text}\color{red}{ }\color{red}{Your}\color{red}{second}\color{red}{Text}$

  to avoid this you can use the special &d& reset or coloring.RESET to not have a color anymore
 ```py
    >>print(coloring.color("&DC143C&Your Text&d&" + "Your second Text)
 ```
  >$\color{red}{Your}\color{red}{Text}\color{white}{Your}\color{white}{second}\color{white}{Text}$
 ```py
    >>print(coloring.color("&DC143C&Your Text" + coloring.RESET + "Your second Text)
 ```
 
