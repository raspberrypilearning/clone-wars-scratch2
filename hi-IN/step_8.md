## फ्रूट बैट

गेम को कुछ कठिन बनाने के लिए, चलिए फ्रूट बैट बनाएँ जो स्पेसशिप पर संतरे फेंकगा।

+ `बैट` स्प्राइट शामिल करें और इसकी चक्कर शैली केवल **बाईं–दाईं** की ओर सेट करें।

+ `बैट` स्प्राइट `चले`{:class="blockmotion"} को साइड से साइड स्टेज के शीर्ष से `हमेशा के लिए`{:class="blockcontrol"} से ऊपर जाने दें। अपने कोड का परीक्षण करना याद रखें।

![screenshot](images/invaders-bat.png)

--- hints ---
--- hint ---
फ्लैग पर क्लिक करने पर, `बैट` बैट को हमेशा यह करना चाहिए
- 10 कदम स्थानांतरित होना
- किनारे पर पहुंचने पर उछलना
--- /hint ---
--- hint ---
ये वे कोड हैं, जिनकी आपको आवश्यकता होगी:

```blocks
जब ⚑ क्लिक किया गया हो
हमेशा के लिए
end
    (10) कदम चले
    अगर किनारे पर है तो उछाले
end
```
--- /hint ---
--- /hints ---

यदि आप बैट की पोशाक की ओर देखें, तो आप देखेंगे कि इसमें पहले से ही भिन्न-भिन्न दो हैं:

![screenshot](images/invaders-bat-costume.png)

+ बैट के स्थानांतरित होने पर इसके पंख फड़फड़ाते हुए दिखाने के लिए `अगली पोशाक`{:class="blocklooks"} ब्लॉक का उपयोग करें।

--- hints ---
--- hint ---
बैट के स्थानांतरित होने के बाद, इसे `अगली पोशाक`{:class="blocklooks"} दिखानी चाहिए और फिर कुछ समय के लिए `ठहरें`{:class="blockcontrol"} करना चाहिए।
--- /hint ---
--- hint ---
ये वे कोड हैं, जिनकी आपको आवश्यकता होगी:

```blocks
अगली पोशाक
(0.3) सेकेंड तक ठहरे
```
--- /hint ---
--- hint ---
नए कोड सहित जोड़ गया पूर्ण कोड इस प्रकार है:

```blocks
जब ⚑ क्लिक किया गया हो
हमेशा के लिए
end
    (10) कदम चले
    अगर किनारे पर है तो उछाले
    अगली पोशाक
    (0.3) सेकेंड तक ठहरे
end
```
--- /hint ---
--- /hints ---

चलिए अब बैट से संतरे फिंकवाए जाएँ।

+ Scratch लाइब्रेरी से नई `संतरा` स्प्राइट शामिल करें।

![screenshot](images/invaders-orange.png)

+ अपने बैट में कोड शामिल करें, ताकि जब फ्लैग पर क्लिक किया जाता है, तो यह 5 और 10 सेकंड के मध्य बेतरतीब समय तक प्रतीक्षा करे और फिर `संतरा` स्प्राइट का क्लोन बनाए।

--- hints ---
--- hint ---
वह कोड देखें, जो आपने `बिजली` स्प्राइट बनाने पर लिखा था। आपके लिए अभी आवश्यक कोड बहुत ही समान है, सिवाय इसके कि **स्थान** बार दबाने पर संतरा दिखाई नहीं देता, यह आपके द्वारा `5-10`{:class="blockoperators"} सेकंड के `ठहरें`{:class="blockcontrol"} के बाद दिखाई देता है।
--- /hint ---
--- hint ---
`जब ⚑ क्लिक किया गया हो`{:class="blockcontrol"}, तो `बैट` स्प्राइट को यह करना चाहिए
`हमेशा के लिए`{:class="blockcontrol"}
- `5-10`{:class="blockoperators"} सेकंड के बीच `क्रमरहित`{:class="blockoperators"} समय के लिए `ठहरें`{:class="blockcontrol"}
- `संतरा` स्प्राइट का `क्लोन बनाएँ`{:class="blockcontrol"}
--- /hint ---
--- hint ---
ये वे कोड हैं, जिनकी आपको आवश्यकता होगी:

```blocks
जब ⚑ क्लिक किया गया हो
हमेशा के लिए
end
	((5) से (10) तक क्रमरहित चुनने) सेकेंड तक ठहरे
	[संतरा v] का क्लोन बनाए
end
```
--- /hint ---
--- /hints ---

+ अपने `संतरा` स्प्राइट पर क्लिक करें और कोई कोड जोड़ें, ताकि प्रत्येक `संतरा` स्प्राइट यों गिरे कि ये `बैट` स्प्राइट से शुरू हों और स्टेज के नीचे की ओर गिरें।

--- hints ---
--- hint ---
यह कोड जो आप चाहते हैं, `बिजली` स्प्राइट के मध्य कोड के लगभग समान है, सिवाय इसके कि `संतरा` स्प्राइट `पर जाएँ`{:class="blockmotion"} `बैट` स्प्राइट की स्थिति में जाए, और उपर की बजाय नीचे की ओर स्थानांतरित होने के लिए `() से y बदले`{:class="blockcontrol"} ब्लॉक का उपयोग करे।
--- /hint ---
--- hint ---
ये वे कोड हैं, जिनकी आपको आवश्यकता होगी:

```blocks
	जब ⚑ क्लिक किया गया हो
	छुपाएँ

	मेरे एक क्लोन के रूप में शुरू होने पर
	[बैट1 v] पर जाएँ
	दिखाएं
	<[किनारा v] को छू रहा है?> तक दोहराते रहे
end
		(-4) से y बदले
	end
	इस क्लोन को डिलिट करें

```
--- /hint ---
--- /hints ---


+ `संतरा` स्प्राइट में कुछ और कोड शामिल करें, ताकि जब `अंतरिक्ष यान` स्प्राइट इससे टकराए, तो खिलाड़ी को रीसेट करने का मौका देने के लिए यह गायब भी हो जाए:

```blocks
	मुझे [hit v] मिलने पर
  इस क्लोन को डिलिट करें
```

+ आपको अपने `अंतरिक्ष यान` स्प्राइट में कोड में भी परिवर्तन करना होगा, ताकि यह `Hippo` स्प्राइट या `संतरा` स्प्राइट को छूने पर टकरा जाए:

```blocks
	<<[Hippo1 v] को छू रहा है?> या <[संतरा v] को छू रहा है?>> होने तक ठहरे
```

+ अपने गेम का परीक्षण करें। गिरते हुए संतरे से टकरा जाने पर क्या होता है?