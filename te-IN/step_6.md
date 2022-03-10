## రిసోర్స్ వేరియబుల్స్ సృష్టించండి

ఈ దశలో, మీరు **Third Country** sprite కోసం కొత్త రిసోర్స్ వేరియబుల్‌లను సృష్టించబోతున్నారు. మీరు వేరియబుల్స్‌కు విలువలను జోడించి, ఆపై **Third Country** sprite కోసం నిలువు వరుసను గీయడానికి ఆ విలువలను ఉపయోగిస్తారు.

ముందుగా, మీరు పునరుత్పాదకం కాని వనరుల కోసం వేరియబుల్‌ని సృష్టిస్తారు.

--- task ---

కొత్త వేరియబుల్ సృష్టించడానికి, `Variables`{:class="block3variables"} బ్లాక్స్ మెనుపై క్లిక్ చేయండి.

**Make a Variable** బటన్ పై క్లిక్ చేయండి.

--- /task ---

వేరియబుల్ కోసం మీకు శీర్షిక అవసరం. వేరియబుల్ ఈ sprite కోసం మాత్రమే సృష్టించబడిందని మీరు నిర్ధారించుకోవాలి, తద్వారా మీరు ఈ sprite కోసం విలువను అప్‌డేట్ చేస్తే, అది ఇతరులకు మార్చబడదు. ఇతర sprite లు కూడా `nonrenewable`{:class="block3variables"} పేరుతో వేరియబుల్‌ని కలిగి ఉన్నప్పటికీ, ప్రతి వేరియబుల్ ఒక్కో దేశానికి వేర్వేరు విలువలను కలిగి ఉంటుంది.

--- task ---

ఈ వేరియబుల్‌ని `nonrenewable`అని పిలవండి.

**ముఖ్యవిషయం**: **For this sprite only** ని క్లిక్ చేయండి.

ఆపై **OK** ని క్లిక్ చేయండి.

![ఎలక్ట్రిసిటీ నేమింగ్ వేరియబుల్స్ యొక్క png](images/electricity-naming-variables.png){:width="400px"}

--- /task ---

మిగిలిన రిసోర్స్ వేరియబుల్స్ సృష్టించండి.

--- task ---

అదే విధంగా కొత్త వేరియబుల్స్ సృష్టించండి. ప్రతి కొత్త వేరియబుల్ కోసం **For this sprite only** ఎంచుకోవాలని గుర్తుంచుకోండి:
+ `wind`{:class="block3variables"}
+ `solar`{:class="block3variables"}
+ `hydro`{:class="block3variables"}
+ `geothermal`{:class="block3variables"}
+ `bioenergy`{:class="block3variables"}

--- /task ---

కనబడకుండా వేరియబుల్స్‌ను దాచండి.

--- task ---

అన్ని కొత్త శక్తి వేరియబుల్స్ `Variables`{:class="block3variables"} బ్లాక్స్ మెనులో జాబితా చేయబడ్డాయి. అవి కూడా Stage లో ఆటోమేటిక్‌గా చూపబడతాయి, కానీ ఈ ప్రాజెక్ట్ కోసం వాటిని అక్కడ చూపించాల్సిన అవసరం లేదు.

కనబడకుండా వాటిని దాచడానికి ప్రతి వేరియబుల్ పక్కన ఉన్న చెక్‌బాక్స్‌లపై క్లిక్ చేయండి.

--- no-print ---

![దాగిన వేరియబుల్స్ యొక్క gif](images/hiding-variables.gif)

--- /no-print ---

--- /task ---

ఇప్పుడు మీరు ఎంచుకున్న దేశం కోసం వనరుల డేటాను ఇన్‌పుట్ చేయవచ్చు. డేటాను ఇన్‌పుట్ చేయడంలో మళ్లీ మీకు సహాయపడటానికి దిగువ పట్టిక ఉంది.

Resource type | Brazil | Canada | Iceland | India | Ireland | Norway | Singapore | S.Africa | USA | | --- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | **Non-renewable** | 18 | 34 | 0 | 81 | 64 | 2 | 99 | 94 | 83 | **Wind** | 9 | 5 | 0 | 5 | 32 | 4 | 0 | 3 | 7 | **Solar** | 1 | 1 | 0 | 3 | 0 | 0 | 1 | 1 | 2 | **Hydro** | 63 | 58 | 70 | 11 | 4 | 94 | 0 | 2 | 7 | **Geothermal** | 0 | 0 | 30 | 0 | 0 | 0 | 0 | 0 | 0 | **Bioenergy** | 9 | 2 | 0 | 0 | 0 | 0 | 0 | 0 | 1 |

--- task ---

ఒక్కొక్క వనరుకు ఒకటి, మొత్తం ఆరు `set my variable to`{:class="block3variables"} బ్లాకులను జోడించండి. దిగువ కోడ్ **Third Country** sprite కోసం ఉదాహరణ డేటాగా South Africa ను ఉపయోగిస్తుంది, కానీ మీరు ఎంచుకున్న దేశం కోసం మీరు గణాంకాలను ఇన్‌పుట్ చేస్తారు.

```blocks3
when flag clicked
erase all
+set (nonrenewable) to (94)
+set (wind) to (3)
+set (solar) to (1)
+set (hydro) to (2)
+set (geothermal) to (0)
+set (bioenergy) to (0)
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
pen up
go to x: (160) y: (70)
say [Third Country]
```

--- /task ---

--- task ---

వనరుల విలువలు 100 వరకు జోడించబడిందో లేదో ఒకటికి రెండుసార్లు తనిఖీ చేయండి.

--- /task ---

--- save ---
