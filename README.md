# $\color{red}{C}\color{orange}{O}\color{yellow}{L}\color{green}{O}\color{blue}{R}\color{aqua}{I}\color{purple}{N}\color{indigo}{G}$

## Installation
- Using [PIP](https://pip.pypa.io/en/stable/) package manager
  ```bash
  pip install Coloring
  ```
- Downloading from github
  ```
    Drag the coloring.py in your projects and import it 
  ``` 

## Usage 
- <h3>Using Constants</h3> 
```py
  >>print(coloring.RED + "Your Text")
  ```
 *type "str"*
 
 - <h3>Using RGB/HEX code (letters for hex must be upper)</h3>
 
 ```py
   >>print(coloring.rgb((255,0,0)) + "YourText")
 ```
  ```py
    >>print(coloring.hex("DC143C") + "YourText")
 ```
   >$\color[rgb]{0.8,0,0}{Your}\color[rgb]{0.8,0,0}{Text}$

    
- <h3>Using Separators(by default = "&") </h3>

 ```py
    >>print(coloring.color("&DC143C&YourText"))
 ```
  ```py
    >>print(coloring.color("&255,0,0&YourText", rgb=True))
 ```
 
 >$\color[rgb]{0.8,0,0}{Your}\color[rgb]{0.8,0,0}{Text}$

- <h4> Notice if you use a color and don't reset it, it will use it for everything after the call.</h4>

 ```py
    >>print(coloring.color("&DC143C&YourText" + "YoursecondText)
 ```
 >$\color[rgb]{0.8,0,0}{Your}\color[rgb]{0.8,0,0}{Text}\color[rgb]{0.8,0,0}{ }\color[rgb]{0.8,0,0}{Your}\color[rgb]{0.8,0,0}{second}\color[rgb]{0.8,0,0}{Text}$

- <h4>to avoid this you can use the special &d& reset or coloring.RESET to not have a color anymore</h4>
 ```py
    >>print(coloring.color("&DC143C&Your Text&d&" + "Your second Text)
 ```
 ```py
    >>print(coloring.color("&DC143C&Your Text" + coloring.RESET + "Your second Text)
 ```
   >$\color[rgb]{0.8,0,0}{Your}\color[rgb]{0.8,0,0}{Text}\color{white}{Your}\color{white}{second}\color{white}{Text}$

## Specials

- BOLD = Coloring.BOLD | &b& 
- UNDERLINE = Coloring.UNDERLINE | &u&
- REVERSE = Coloring.REVERSE | &r&
- RESET = Coloring.RESET |&d& 
 
