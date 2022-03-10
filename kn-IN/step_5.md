## ಪೆನ್‌ ನಿರ್ಮಿಸಿ

ಈ ಹಂತದಲ್ಲಿ, Stage ಮೇಲೆ ಚಿತ್ರಿಸಲು `Pen`{:class="block3extensions"} ವಿಸ್ತರಿತ ಬ್ಲಾಕ್‌ಗಳನ್ನು ಹೇಗೆ ಉಪಯೋಗಿಸುವುದು ಎನ್ನುವುದನ್ನು ಕಲಿಯುವಿರಿ.

ಮೊದಲಿಗೆ, **Third Country** ಸ್ಪ್ರೈಟ್‌ನ್ನು ರೇಖಾನಕ್ಷೆಯ ಕೆಳಕ್ಕೆ ಚಲಿಸಿ ಅದರಿಂದ ಅದು ಸ್ತಂಭವನ್ನು ಚಿತ್ರಿಸಲು ಪ್ರಾರಂಭಿಸಲು ಸರಿಯಾದ ಸ್ಥಾನದಲ್ಲಿರುತ್ತದೆ.

--- task ---

ನಿಮ್ಮ `when green flag clicked`{:class="block3events"} ಬ್ಲಾಕ್‌ ಅಡಿಯಲ್ಲಿ, ಮೂರು `Motion`{:class="block3motion"} ಬ್ಲಾಕ್‌ಗಳನ್ನು ಒಳಕ್ಕೆ ಸೇರಿಸಿ:
+ `go to x: y:`{:class="block3motion"} ಬ್ಲಾಕ್‌ನಲ್ಲಿ, ಮೌಲ್ಯಗಳನ್ನು `x:`{:class="block3motion"} `120` and `y:`{:class="block3motion"} `-140` ಗೆ ಬದಲಾಯಿಸಿ
+ `set rotation style`{:class="block3motion"} ಬ್ಲಾಕ್, ಮತ್ತು `don't rotate`{:class="block3motion"}ನ್ನು ಡ್ರಾಪ್‌-ಡೌನ್‌ ಮೆನುನಿಂದ ಆಯ್ಕೆಮಾಡಿಕೊಳ್ಳಿ
+ `point in direction 90`{:class="block3motion"} ಬ್ಲಾಕ್

```blocks3
when flag clicked
+ go to x:(120) y: (-140)
+ set rotation style [don't rotate v]
+ point in direction (90)
go to x: (200) y: (70)
say [Third Country]
```

--- /task ---

ಈಗ `Pen`{:class="block3extensions"} ವಿಸ್ತರಿತ ಬ್ಲಾಕ್‌ಗಳ ಮೆನುವನ್ನು ಸೇರಿಸಿ.

--- task ---

ನಿಮ್ಮ **Third Country** ಸ್ಪ್ರೈಟ್‌ನ **Code** ಟ್ಯಾಬ್‌ ಮೇಲೆ ಕ್ಲಿಕ್‌ ಮಾಡಿ, ಮತ್ತು ನಂತರ `Pen`{:class="block3extensions"} ವಿಸ್ತರಿತ ಬ್ಲಾಕ್‌ನ್ನು ಕ್ಲಿಕ್‌ ಮಾಡಿ (ಪರದೆಯ ಕೆಳ ಎಡ ಮೂಲೆಯಲ್ಲಿದೆ).

![pen extension ಬ್ಲಾಕ್‌ನ ಪಿಎನ್‌ಜಿ](images/pen-extension.png){:width="400px"}

--- /task ---

ಪೆನ್ನನ್ನು ಸಿದ್ಧಪಡಿಸಿ ಮತ್ತು ಅದರ ಗಾತ್ರವನ್ನು ಹೊಂದಿಸಿ.

--- task ---

`set pen size to 1`{:class="block3extensions"} ಬ್ಲಾಕ್‌ನ್ನು ಸೇರಿಸಿ, ಮತ್ತು ಮೌಲ್ಯವನ್ನು `2` ಕ್ಕೆ ಬದಲಾಯಿಸಿ ಅದರಿಂದ ಪೆನ್ನನ್ನು ಸ್ವಲ್ಪ ದಪ್ಪ ಮಾಡುತ್ತದೆ. ಚಿತ್ರಿಸಲು ಸಿದ್ಧವಾಗಲು `pen down`{:class="block3extensions"} ಬ್ಲಾಕ್‌ ಒಳಸೇರಿಸಿ.

```blocks3
when flag clicked
go to x:(120) y: (-140)
set rotation style [don't rotate v]
point in direction (90)
+set pen size to (2)
+pen down
go to x: (200) y: (70)
say [Third Country]
```

--- /task ---

ಹಸಿರು ಬಾವುಟವನ್ನು ಕ್ಲಿಕ್‌ ಮಾಡಿದಾಗ ಪ್ರೋಗ್ರಾಮ್‌ Stage ನಿಂದ ಪೆನ್ನಿನ ಗುರುತುಗಳನ್ನು ತೆರವುಗೊಳಿಸುವಂತೆ ಮಾಡುವುದನ್ನು ಮತ್ತು ಪೆನ್ನನ್ನು ಮೇಲೆತ್ತುವಂತೆ ಮಢುವುದನ್ನು ನೀವು ಖಚಿತಪಡಿಸಿಕೊಳ್ಳಬೇಕು.

--- task ---

`erase all`{:class="block3extensions"} ಬ್ಲಾಕ್‌ನ್ನು ಸೇರಿಸಿ ಮತ್ತು `pen up`{:class="block3extensions"} ಬ್ಲಾಕ್‌ನ್ನು ನಿಮ್ಮ ಕೋಡ್‌ ಮೇಲ್ಗಡೆ, `when green flag clicked`{:class="block3events"} ಬ್ಲಾಕ್‌ ಅಡಿಯಲ್ಲಿ ಸೇರಿಸಿ.

```blocks3
when flag clicked
+ erase all
+ pen up
go to x:(120) y: (-140)
set rotation style [don't rotate v]
point in direction (90)
set pen size to (2)
pen down
go to x: (200) y: (70)
say [Third Country]
```

--- /task ---

ಪೆನ್ನು ಪ್ರತಿಯೊಂದು ಸಂಪನ್ಮೂಲವನ್ನು ಚಿತ್ರಿಸುವಾಗ ಅದರ ಬಣ್ಣ ಬದಲಾಗುತ್ತದೆ. ಬಹು ದೇಶಗಳಾದ್ಯಂತ ಉತ್ಪನ್ನವಾಗುವ ಸಂಪನ್ಮೂಲಗಳನ್ನು ಹೋಲಿಸಲು, ಪ್ರತಿಯೊಂದು ಸಂಪನ್ಮೂಲವನ್ನು ಪ್ರತಿನಿಧಿಸುವ ಬಣ್ಣವು ಪ್ರತಿಯೊಂದು ದೇಶಕ್ಕೂ ಒಂದೇ ಆಗಿರಬೇಕು. ಪೆನ್ನು ವರ್ಗಗಳನ್ನು ಚಿತ್ರಿಸಿ ಮುಗಿಸಿದ ನಂತರ, ಅದು ಹಿನ್ನೆಲೆಯ ಬಣ್ಣಕ್ಕೆ ಪರಿವರ್ತನೆಯಾಗುತ್ತದೆ, ಅದು ಬೂದುಬಣ್ಣ.

--- task ---

ನಿಮ್ಮ ಕೋಡ್‌ಗೆ ಏಳು `set pen colour to`{:class="block3extensions"} ಬ್ಲಾಕ್‌ಗಳನ್ನು ಸೇರಿಸಿ. ಇವುಗಳು ಆರು ವರ್ಗಗಳನ್ನು ಪ್ರತಿನಿಧಿಸುತ್ತವೆ ಹಾಗೂ ಹಿನ್ನೆಲೆಯನ್ನು ಪ್ರತಿನಿಧಿಸಲು ಒಂದು ಹೆಚ್ಚುವರಿ ಬಣ್ಣ.

```blocks3
when flag clicked
pen up
go to x:(120) y: (-140)
set rotation style [don't rotate v]
point in direction (90)
set pen size to (2)
pen down
+ set pen color to []
+ set pen color to []
+ set pen color to []
+ set pen color to []
+ set pen color to []
+ set pen color to []
+ set pen color to []
go to x: (200) y: (70)
say [Third Country]
```

--- /task ---

ಸಂಪನ್ಮೂಲಗಳಿಗೆ ನೀವು ಆಯ್ಕೆಮಾಡಿಕೊಂಡ ಬೇರೆ ಬೇರೆ ಬಣ್ಣಗಳನ್ನು ಪ್ರತಿನಿಧಿಸಲು ನೀವು ಪ್ರತಿಯೊಂದು ಬ್ಲಾಕ್‌ನ ಬಣ್ಣಗಳನ್ನು ಬದಲಾಯಿಸಬೇಕು.

--- task ---

ಮೊದಲನೆಯ `set pen colour to`{:class="block3extensions"} ಬ್ಲಾಕ್‌ ಮೇಲೆ ಕ್ಲಿಕ್‌ ಮಾಡಿ ಮತ್ತು **Colour picker** ಟೂಲ್‌ ಆಯ್ಕೆಮಾಡಿ. ನಿಮ್ಮ ಕೀಯಲ್ಲಿ ಮೊದಲನೆಯ ಸಂಪನ್ಮೂಲದ ಮೇಲೆ ಕ್ಲಿಕ್‌ ಮಾಡಿ. ವೃತ್ತವು ನಂತರ ನೀವು ಆಯ್ಕೆ ಮಾಡಿಕೊಂಡ ಬಣ್ಣಕ್ಕೆ ತಿರುಗುತ್ತದೆ.

ಪ್ರತಿಯೊಂದು ಸಂಪನ್ಮೂಲಕ್ಕೂ ಸರದಿಯಲ್ಲಿ ಇದನ್ನು ಪುರಾವರ್ತನೆ ಮಾಡಿ, ಆದರಿಂದ ನೀವು ಸಂಪನ್ಮೂಲ ಬಣ್ಣಗಳ ಕ್ರಮವನ್ನು ಗೊಂದಲಮಯವಾಗಿಸುವುದಿಲ್ಲ.

ಏಳನೆಯ `set pen colour to`{:class="block3extensions"} ಬ್ಲಾಕ್‌ಗೆ ಹಿನ್ನೆಲೆಯ ಬಣ್ಣವನ್ನು ಉಪಯೋಗಿಸಲು ಮರೆಯಬೇಡಿ,ನೀವು ಇದನ್ನು Stage ನ ಹಿನ್ನೆಲೆಯ ಮೇಲೆ ಎಲ್ಲಿಯಾದರೂ ಸುಳಿದಾಡಿ ಪಡೆಯಬಹುದು.

--- /task ---

ಸ್ತಂಭವು ಚಿತ್ರಿಸುವುದನ್ನು ಮುಗಿಸಿದಾಗ ಪೆನ್ನನ್ನು ಮೇಲಕ್ಕೆತ್ತಿ.

--- task ---

ನಿಮ್ಮ ಕೋಡ್‌ಗೆ `pen up`{:class="block3extensions"} ಬ್ಲಾಕ್‌ ಸೇರಿಸಿ.

```blocks3
when flag clicked
pen up
go to x:(120) y: (-140)
set rotation style [don't rotate v]
point in direction (90)
set pen size to (2)
pen down
set pen color to [#5e6766]
set pen color to [#37e4db]
set pen color to [#e4d748]
set pen color to [#169bb0]
set pen color to [#ab7519]
set pen color to [#00a42c]
set pen color to [#dadada]
+pen up
go to x: (200) y: (70)
say [Third Country]
```

--- /task ---

--- task ---

**Third Country** ಸ್ಪ್ರೈಟ್‌ ಸಿದ್ಧವಾಗಿದೆಯಾದರೂ, ಅದು ರೇಖಾನಕ್ಷೆಯ ಮೇಲೆ ಕಾಣಿಸುವುದಿಲ್ಲ ಏಕೆಂದರೆ ನೀವು ಯಾವುದೇ ಸಂಪನ್ಮೂಲ ದತ್ತಾಂಶವನ್ನು ಇನ್‌ಪುಟ್‌ ಮಾಡಿಲ್ಲ. ಮುಂದಿನ ಹಂತದಲ್ಲಿ ದತ್ತಾಂಶವನ್ನು ಇನ್‌ಪುಟ್‌ ಮಾಡಲು ಮತ್ತು ನಿಮ್ಮ ಕೋಡ್‌ ಪರಿಶೀಲಿಸಲು ನಿಮಗೆ ಅವಕಾಶ ಇರುತ್ತದೆ.

--- /task ---

--- save ---
