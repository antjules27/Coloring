# $\color{red}{C}\color{orange}{O}\color{yellow}{L}\color{green}{O}\color{blue}{R}\color{aqua}{I}\color{purple}{N}\color{indigo}{G}\color{yellow}{S}$

## Installation
- Using [PIP](https://pip.pypa.io/en/stable/) package manager
  ```bash
  pip install Colorings
  ```
- Downloading from github
  ```
    Drag the colorings.py in your projects and import it 
  ``` 

## Usage 
- <h3>Using Constants</h3> 
```py
  >>print(colorings.RED + "Your Text")
  ```
 *type "str"*
 
 - <h3>Using RGB/HEX code (letters for hex must be upper)</h3>
 
 ```py
   >>print(colorings.rgb((255,0,0)) + "YourText")
 ```
  ```py
    >>print(colorings.hex("DC143C") + "YourText")
 ```
   >$\color[rgb]{0.8,0,0}{Your}\color[rgb]{0.8,0,0}{Text}$

    
- <h3>Using Separators(by default = "&") </h3>

 ```py
    >>print(colorings.color("&DC143C&YourText"))
 ```
  ```py
    >>print(colorings.color("&255,0,0&YourText", rgb=True))
 ```
 
 >$\color[rgb]{0.8,0,0}{Your}\color[rgb]{0.8,0,0}{Text}$

- <h4> Notice if you use a color and don't reset it, it will use it for everything after the call.</h4>

 ```py
    >>print(colorings.color("&DC143C&YourText" + "YoursecondText)
 ```
 >$\color[rgb]{0.8,0,0}{Your}\color[rgb]{0.8,0,0}{Text}\color[rgb]{0.8,0,0}{ }\color[rgb]{0.8,0,0}{Your}\color[rgb]{0.8,0,0}{second}\color[rgb]{0.8,0,0}{Text}$

- <h4>to avoid this you can use the special &d& reset or colorings.RESET to not have a color anymore</h4>
 ```py
    >>print(colorings.color("&DC143C&Your Text&d&" + "Your second Text)
 ```
 ```py
    >>print(colorings.color("&DC143C&Your Text" + colorings.RESET + "Your second Text)
 ```
   >$\color[rgb]{0.8,0,0}{Your}\color[rgb]{0.8,0,0}{Text}\color{white}{Your}\color{white}{second}\color{white}{Text}$

## Specials

- BOLD = Colorings.BOLD | &b& 
- UNDERLINE = Colorings.UNDERLINE | &u& 
- REVERSE = Colorings.REVERSE | &r& 
- RESET = Colorings.RESET |&d&
 
