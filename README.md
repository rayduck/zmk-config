# zmk-config
For Corne or any 36 key split

Modifiers will be sticky (one-shot) keys, but due to limitations of ZMK, SFT and CMD are normal keys.
CAP is caps word, which capitalizes letter until a non-letter character is entered.

Combos: Q+W is TAB, SPC+RET is ESC

```
---------------------------------------------------------------------------
|     |  Q  |  W  |  F  |  P  |  B  | |  J  |  L  |  U  |  Y  |BKSPC|     |
|     |  A  |  R  |  S  |  T  |  G  | |  M  |  N  |  E  |  I  |  O  |     |
|     |  Z  |  X  |  C  |  D  |  V  | |  K  |  H  |  ,  |  .  | NAV |     |
                  | CMD |-SYB-| SPC | | RET |—NUM-| SFT |
---------------------------------------------------------------------------
|     | DEL |  \  |  %  |  $  |  £  | |     |  ^  |  {  |  }  |BKSPC|     |
|     |  #  |  (  |  )  |  :  |     | |     |  "  |  [  |  ]  |  ;  |     |
|     | ESC |  @  |  !  |  &  |     | |     |  `  |  <  |  >  |  ?  |     |
                  | CMD |_SYB_| SPC | | RET |-NXT-| ALT |
---------------------------------------------------------------------------
|     |     |  6  |  5  |  4  |     | |     |  *  |  -  |  /  |BKSPC|     |
|     |  3  |  2  |  1  |  0  |     | |     |  '  |  _  |  =  |  +  |     |
|     |     |  9  |  8  |  7  |     | |     |  |  |  ,  |  .  |  ~  |     |
                  | CTL |-NXT-| SPC | | RET |_NUM_| SFT |
---------------------------------------------------------------------------
|     |BTCLR| F 6 | F 5 | F 4 | BLE | | USB |BRIDN|BRIUP|VOLDN|VOLUP|     |
|     | F 3 | F 2 | F 1 | F10 | F11 | |left |down | up  |right|VMUTE|     |
|     | CAP | F 9 | F 8 | F 7 | F12 | | END |PG_DN|PG_UP| HOM |_NAV_|     |
                  | CTL | BT0 | BT1 | | BT2 | BT3 | ALT |
```





## Design principles

1. Comfy do
2. Rolls good
3. Thumb strong, pinkie weak
4. Mod-tap bad


## Key effort analysis
The main models referred to are colemak-dh and workman's effort models. In addition, I had a think about how easy it is to press chorded keys with thumb modifiers.

TODO.

### Single keys
### Chorded keys
### Complications with thumb and enter.

## Character frequency

For sensible placements of the symbol and number layers, I have done character and bigram frequency analyses for programming in Python.

### Results
![Overall bigram frequency](https://user-images.githubusercontent.com/16619392/144720903-15cf79a0-70f3-4f00-86f8-926414630da6.png)

![Bigram frequency, excluding whitespaces and alphas](https://user-images.githubusercontent.com/16619392/144720912-830ccb45-9b4f-41be-a178-8d265666c51b.png)

![Symbol frequency](https://user-images.githubusercontent.com/16619392/144720920-5529625f-2b92-4f9c-add3-8fd3388deb25.png)

![Character frequency](https://user-images.githubusercontent.com/16619392/144720959-8a6bd4d2-cf2a-4d77-88cf-151e2b0cffc6.png)

### Analysis
TODO



### Corpus

The corpus used for analysis incorporates popular Python and Jupyter notebook repositories.

#### Python
- cpython
- django
- flask
- requests

Total 5338 python files

(Pro tip: shallow clone to reduce size)

#### Jupyter Notebooks
- CLIP
- homemade-machine-learning
- deepmind-research
- introduction_to_ml_with_python
- mathematics_conjectures
- notebooks (huggingface)
- PythanDataScienceHandbook

Total 319 ipynb files and 5982 code cells
