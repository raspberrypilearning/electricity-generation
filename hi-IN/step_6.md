## संसाधन वेरिएबल बनाएं

इस चरण में आप **Third Country** स्प्राइट के लिए नए संसाधन वेरिएबल बनाने जा रहे हैं। आप वेरिएबल्स में मान जोड़ेंगे, और फिर उन मानों का उपयोग **Third Country** स्प्राइट के लिए कॉलम बनाने के लिए करेंगे।

सबसे पहले, आप गैर-नवीकरणीय संसाधनों के लिए एक वेरिएबल बनाएंगे।

--- task ---

`Variables`{:class="block3variables"} ब्लॉक मेन्यू पर क्लिक करके एक नया वेरिएबल बनाएं।

फिर, **Make a Variable** बटन पर क्लिक करें।

--- /task ---

आपको वेरिएबल के लिए एक शीर्षक की आवश्यकता है। आपको यह भी सुनिश्चित करने की आवश्यकता है कि वेरिएबल केवल इस स्प्राइट के लिए बनाया गया है ताकि यदि आप इस स्प्राइट के लिए मान को अपडेट(अद्यतन) करते हैं, तो यह इसे दूसरों के लिए नहीं बदलता है। यद्यपि दुसरे स्प्राइट के पास भी `nonrenewable`{:class="block3variables"} नामक एक वेरिएबल है, प्रत्येक वेरियबल प्रत्येक देश के लिए एक अलग मान रखता है।

--- task ---

इस वेरियबल को `nonrenewable` कहें।

**महत्वपूर्ण**: **For this sprite only** पर क्लिक करें ।

फिर, **OK** पर क्लिक करें ।

![बिजली के नामकरण वेरिएबल का पीएनजी](images/electricity-naming-variables.png){:width="400px"}

--- /task ---

शेष संसाधन वेरिएबल बनाएँ।

--- task ---

इसी तरह नए वेरिएबल बनाएं। प्रत्येक नए वेरिएबल के लिए **For this sprite only** का चयन करना याद रखें:
+ `wind`{:class="block3variables"}
+ `solar`{:class="block3variables"}
+ `hydro`{:class="block3variables"}
+ `geothermal`{:class="block3variables"}
+ `bioenergy`{:class="block3variables"}

--- /task ---

वेरिएबल को दृश्य से छिपाएं।

--- task ---

सभी नए ऊर्जा वेरिएबल `Variables`{:class="block3variables"} ब्लॉक मेनू में सूचीबद्ध हैं। वे स्वचालित रूप से Stage पर भी दिखाए जाते हैं, लेकिन आपको इस प्रोजेक्ट के लिए उन्हें वहां दिखाने की आवश्यकता नहीं है।

प्रत्येक वेरिएबल को दिखने से छिपाने के लिए उनके बगल में स्थित चेकबॉक्स पर क्लिक करें।

--- no-print ---

![वेरिएबल छुपाने का जीआईएफ](images/hiding-variables.gif)

--- /no-print ---

--- /task ---

अब आप अपने चुने हुए देश के लिए संसाधन डेटा इनपुट कर सकते हैं। डेटा इनपुट करने में आपकी सहायता के लिए तालिका नीचे फिर से दी गई है।

संसाधन प्रकार | Brazil | Canada | Iceland | India | Ireland | Norway | Singapore | S.Africa | USA |
| --- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
**Non-renewable** | 18 | 34 | 0 | 81 | 64 | 2 | 99 | 94 | 83 |
**Wind** | 9 | 5 | 0 | 5 | 32 | 4 | 0 | 3 | 7 |
**Solar** | 1 | 1 | 0 | 3 | 0 | 0 | 1 | 1 | 2 |
**Hydro** | 63 | 58 | 70 | 11 | 4 | 94 | 0 | 2 | 7 |
**Geothermal** | 0 | 0 | 30 | 0 | 0 | 0 | 0 | 0 | 0 |
**Bioenergy** | 9 | 2 | 0 | 0 | 0 | 0 | 0 | 0 | 1 |

--- task ---

छह `set my variable to`{:class="block3variables"} ब्लॉक जोड़ें, प्रत्येक प्रकार के संसाधन के लिए एक। नीचे दिया गया कोड **Third Country** स्प्राइट के उदाहरण डेटा के रूप में दक्षिण अफ्रीका का उपयोग करता है, लेकिन आप अपने चुने हुए देश के लिए आंकड़े इनपुट करेंगे।

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

दोबारा जांचें कि संसाधनों के लिए मान का कुल योग 100 हैं।

--- /task ---

--- save ---
