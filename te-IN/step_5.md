## పెన్ ని నిర్మించండి

ఈ దశలో, మీరు Stage పై డ్రా చేయడానికి `Pen`{:class="block3extensions"} ఎక్సటెన్షన్ బ్లాక్‌లను ఎలా ఉపయోగించాలో నేర్చుకుంటారు.

ముందుగా, **Third Country** sprite ను గ్రాఫ్ దిగువకు తరలించండి, తద్వారా నిలువు వరుసను గీయడం ప్రారంభించడానికి ఇది సరైన స్థితిలో ఉంటుంది.

--- task ---

`when green flag clicked`{:class="block3events"} బ్లాక్‌ కింద, మూడు `Motion`{:class="block3motion"} బ్లాక్‌లను చొప్పించండి:
+ `go to x: y:`{:class="block3motion"} బ్లాకులో, విలువలను `x:`{:class="block3motion"} `120` మరియు `y:`{:class="block3motion"} `-140` కి మార్చండి
+ `set rotation style`{:class="block3motion"} బ్లాకు, మరియు డ్రాప్ డౌన్ మెను నుంచి, `don't rotate`{:class="block3motion"} ను ఎంచుకోండి
+ `point in direction 90`{:class="block3motion"} బ్లాకు

```blocks3
when flag clicked
+ go to x:(120) y: (-140)
+ set rotation style [don't rotate v]
+ point in direction (90)
go to x: (200) y: (70)
say [Third Country]
```

--- /task ---

ఇప్పుడు, ఎక్స్‌టెన్షన్ బ్లాక్స్ మెను నుండి, `Pen`{:class="block3extensions"} ను జోడించండి.

--- task ---

మీ **Third Country** sprite కోసం **Code** ట్యాబ్‌పై క్లిక్ చేసి, ఆపై `Pen`{:class="block3extensions"} ఎక్స్‌టెన్షన్ బ్లాకుని క్లిక్ చేయండి (స్క్రీన్ దిగువ ఎడమవైపు మూలలో).

![పెన్ ఎక్స్‌టెన్షన్ బ్లాక్ యొక్క png](images/pen-extension.png){:width="400px"}

--- /task ---

పెన్ ను సిద్ధం చేసి దాని పరిమాణాన్ని సెట్ చేయండి.

--- task ---

`set pen size to 1`{:class="block3extensions"} బ్లాక్‌ ని జోడించి, విలువను `2` కి మార్చండి, తద్వారా పెన్ కొద్దిగా మందంగా ఉంటుంది. డ్రా చేయడానికి సిద్ధంగా ఉండటానికి `pen down`{:class="block3extensions"} బ్లాక్‌ని చొప్పించండి.

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

ప్రోగ్రామ్ Stage నుండి పెన్ మార్కులను క్లియర్ చేస్తుందని మరియు ఆకుపచ్చ జెండాను క్లిక్ చేసినప్పుడు పెన్ ని పైకి లేపుతుందని మీరు నిర్ధారించుకోవాలి.

--- task ---

`erase all`{:class="block3extensions"} బ్లాకుని జోడించండి మరియు మీ కోడ్ పైన `pen up`{:class="block3extensions"} బ్లాకు, కింద `when green flag clicked`{:class="block3events"} బ్లాకు.

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

ప్రతి వనరును గీసినప్పుడు పెన్ రంగు మారుతుంది. బహుళ దేశాలలో ఉత్పత్తి చేయబడిన వనరులను పోల్చడానికి, ప్రతి వనరును సూచించే రంగు ప్రతి దేశానికి ఒకేలా ఉండాలి. పెన్ విభాగాలను గీయడం పూర్తయిన తర్వాత, అది బ్యాక్‌డ్రాప్ రంగుకు అంటే బూడిద రంగులోకి మారుతుంది.

--- task ---

మీ కోడ్‌లో ఏడు `set pen colour to`{:class="block3extensions"} బ్లాక్‌లను జోడించండి. ఇవి ఆరు వర్గాలను సూచిస్తాయి మరియు నేపథ్యాన్ని సూచించడానికి అదనపు రంగును సూచిస్తాయి.

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

వనరుల కోసం మీరు ఎంచుకున్న విభిన్న రంగులను సూచించడానికి మీరు ఇప్పుడు ప్రతి బ్లాక్ యొక్క రంగులను మార్చాలి.

--- task ---

మొదటి `set pen colour to`{:class="block3extensions"} బ్లాక్‌పై క్లిక్ చేసి, **Colour picker** సాధనాన్ని ఎంచుకోండి. మీ కీ లోని మొదటి వనరుపై క్లిక్ చేయండి. సర్కిల్ మీరు ఎంచుకున్న రంగుకు మారుతుంది.

ప్రతి వనరుల కోసం దీన్ని పునరావృతం చేయండి, తద్వారా మీరు వనరుల రంగుల క్రమాన్ని గజిబిజిగా పొందరు.

ఏడవ `set pen colour to`{:class="block3extensions"} బ్లాక్ కోసం బ్యాక్‌డ్రాప్ కలర్‌ని ఉపయోగించడం మర్చిపోవద్దు, మీరు Stage బ్యాక్‌గ్రౌండ్‌లో ఎక్కడైనా హోవర్ చేయడం ద్వారా దీన్ని పొందవచ్చు.

--- /task ---

కాలమ్ డ్రాయింగ్ పూర్తయిన తర్వాత పెన్ ను లిఫ్ట్ చేయండి.

--- task ---

మీ కోడ్‌కి `pen up`{:class="block3extensions"} బ్లాక్‌ను జోడించండి.

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

**Third Country** sprite సెటప్ చేయబడినప్పటికీ, మీరు ఏ రిసోర్స్ డేటాను ఇన్‌పుట్ చేయనందున ఇది గ్రాఫ్‌లో కనిపించదు. మీరు తదుపరి దశలో డేటాను ఇన్‌పుట్ చేసి, మీ కోడ్‌ని తనిఖీ చేసే అవకాశం ఉంటుంది.

--- /task ---

--- save ---
