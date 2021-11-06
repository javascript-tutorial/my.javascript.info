<!-- # An Introduction to JavaScript -->
# JavaScript မိတ်ဆက်

<!-- Let's see what's so special about JavaScript, what we can achieve with it, and what other technologies play well with it. -->
JavaScript ဆိုတာဘာလည်း? JavaScript နဲ့ ဘာတွေလုပ်လို့ရလည်း နောက်ပြီး တခြားသော နည်းပညာတွေနဲ့ ဘယ်လို ချိတ်ဆက်အလုပ်လုပ်လည်း ဆိုတာ လေ့လာရအောင်။

<!-- ## What is JavaScript? -->
## JavaScript ဆိုတာဘာလည်း?

<!-- *JavaScript* was initially created to "make web pages alive".-->
*JavaScript* ကို ပထမ ပိုင်းမှာ web pages တွေ အလုပ်လုပ်နိုင်အောင် ဖန်တီးခဲ့ပြီး Script Language ကို အသုံးပြုထားပါတယ်။ 

<!-- The programs in this language are called *scripts*. They can be written right in a web page's HTML and run automatically as the page loads. -->
JavaScript ဟာ web page တွေရဲ့ HTML တွေထဲမှာ ရေးနိုင်ပြီးတော့ page စလုပ်လုပ်ချင်းမှာ အလုပ်လုပ်နိုင်ပါတယ်။

<!-- Scripts are provided and executed as plain text. They don't need special preparation or compilation to run. -->
Scripts တွေဟာ ဆိုရင်လည်း plain text အနေနဲ့ အလုပ်လုပ်နိုင်ပြီး အထူးတလည်း တခြားလုပ်စရာ မလိုပါဘူး။

<!-- In this aspect, JavaScript is very different from another language called [Java](https://en.wikipedia.org/wiki/Java_(programming_language)). -->
ဒီနေရာမှာ ပြောချင်တာက JavaScript ဆိုတာဟာ တခြား programming language ဖြစ်တဲ့ [Java](https://en.wikipedia.org/wiki/Java_(programming_language)) နဲ့ လုံးဝမတူပါဘူး

```smart header="<u>Java</u>Script လို့ ဘာလို့ခေါ်တာလည်း?"
<!-- When JavaScript was created, it initially had another name: "LiveScript". But Java was very popular at that time, so it was decided that positioning a new language as a "younger brother" of Java would help. -->
အစပိုင်း JavaScript ကို ဖန်တီးစဉ်က သူ့ကို "LiveScript" ကို အမည်ပေးထားခဲ့ပါတယ်။ ဒါပေမယ့် အဲ့အချိန်တုန်းက Java က အရမ်းနာမည်ကြီးသည့်အတွက် သူရဲ့ နာမည်ကို ယူသုံးလိုက်လျှင် ပိုကောင်းမည်လို့ ယူဆခဲ့ပြီး JavaScript လို့အမည်ပေးခဲ့တာ ဖြစ်ပါတယ်။

<!-- But as it evolved, JavaScript became a fully independent language with its own specification called [ECMAScript](http://en.wikipedia.org/wiki/ECMAScript), and now it has no relation to Java at all. -->
သို့သော် တိုးတက်ပြောင်းလဲလာသည်နှင့်အမျှ JavaScript ဟာ [ECMAScript](http://en.wikipedia.org/wiki/ECMAScript) ဟုခေါ်သော ၎င်း၏ ကိုယ်ပိုင် သတ်မှတ်ချက်များနှင့် အပြည့်အဝလွတ်လပ်သော ဘာသာစကားတစ်ခု ဖြစ်လာပြီး ယခုအခါ Java နှင့်လုံးဝမသက်ဆိုင်တော့ပါ။
```
<!-- Today, JavaScript can execute not only in the browser, but also on the server, or actually on any device that has a special program called [the JavaScript engine](https://en.wikipedia.org/wiki/JavaScript_engine). -->
ယခုအခါ JavaScript သည် browser ပေါ်တွင်သာ အလုပ်လုပ်သည် မဟုတ်တော့ဘဲ Server (သို့မဟုတ်) [the JavaScript engine](https://en.wikipedia.org/wiki/JavaScript_engine) ဟုခေါ်သော special program ရှိသည့် မည်သည့် device မှာမဆို အလုပ်လုပ်နေပါပြီ ဖြစ်ပါသည်။

<!-- The browser has an embedded engine sometimes called a "JavaScript virtual machine".

Different engines have different "codenames". For example: -->
Browser တွင် သူ့ရဲ့ ကိုယ်ပိုင် ထည့်သွင်းထားသော "JavaScript virtual machine" လို့ခေါ်သည့် engine ရှိပြီး Browser ပေါ်မူတည်ပြီး engine တွေမှာ ကိုယ်ပိုင် နာမည် များရှိပါသည်။

ဥပမာ အားဖြင့်

- [V8](https://en.wikipedia.org/wiki/V8_(JavaScript_engine)) -- in Chrome, Opera and Edge.
- [SpiderMonkey](https://en.wikipedia.org/wiki/SpiderMonkey) -- in Firefox.
- [Chakra](https://en.wikipedia.org/wiki/Chakra_(JScript_engine)) -- in IE
- "JavaScriptCore","Nitro" and "SquirrelFish" for Safari 

စသည်ဖြင့် ရှိပါသည်။
<!-- The terms above are good to remember because they are used in developer articles on the internet. We'll use them too. For instance, if "a feature X is supported by V8", then it probably works in Chrome, Opera and Edge. -->
အပေါ်က Engine နာမည်တွေဟာ Online စာမျက်နှာတွေ မှာ မကြာမဏ တွေ့မြင်နိုင်ပြီး ကျွန်တော် တို့လည်း ကျွန်တော်တို့လည်း ရှေ့ဆက် သင်ခန်းစာများတွင် အသုံးပြုသွားပါမယ်။ ဥပမာအားဖြင့် X ဆိုသော feature ကို V8 တွင် အလုပ်လုပ်သည်ဆိုလျှင် ထို feature သည် Chrome, Opera and Edge မှာ အလုပ်လုပ်သည်ဟု ယူဆနိုင်ပါသည်။


```smart header="Engine တွေက ဘယ်လိုအလုပ်လုပ်လည်း?"
<!-- Engines are complicated. But the basics are easy. -->
Engines တွေက ရှုပ်ထွေးပါတယ် ဒါပေမယ့် အခြေခံကတော့ ရိုးရှင်းပါတယ်။ 
<!-- 1. The engine (embedded if it's a browser) reads ("parses") the script.
2. Then it converts ("compiles") the script to the machine language.
3. And then the machine code runs, pretty fast. -->
1. Engine (Browser ဆိုလျှင် ကိုယ်ပိုင်ရှိပြီးသား) က Script တွေ ကို ဖတ်တယ်။
2. ဖတ်ထားတဲ့ Script တွေကို machine langulage ကို ပြောင်းပေးတယ်။
3. ပြောင်းထားတဲ့ machine codes တွေကို အလွန်လျင်မြန်စွာ run ပေးတယ်။

<!-- The engine applies optimizations at each step of the process. It even watches the compiled script as it runs, analyzes the data that flows through it, and further optimizes the machine code based on that knowledge. -->
Engine တွေဟာ အလုပ်လုပ်သည့် အဆင့်တိုင်းတွင် ပိုမိုကောင်းမွန်စွာ အလုပ်လုပ်ပေးပါသည်။ ထို့အပြင် Script တွေကို run နေသည့် အဆင့်တိုင်းမှာလည်း ခွဲခြမ်းစိတ်ဖြာပေးပြီး နောက်လာမယ့် machine code တွေမှာ ပိုမိုကောင်းမွန်အောင် ထိုအချက်အလက်တွေကို အသုံးပြုပါသည်။ 
```

<!-- ## What can in-browser JavaScript do? -->
## Browser မှာပါတဲ့ JavaScript တွေက ဘာတွေလုပ်နိုင်လည်း?

<!-- Modern JavaScript is a "safe" programming language. It does not provide low-level access to memory or CPU, because it was initially created for browsers which do not require it. -->
နောက်ပိုင်း JavaScript Version ဟာ လုံခြုံပါတယ်။ သူတို့ကို low-level တွေ ဖြစ်တဲ့ memory ဒါမှမဟုတ် CPU တို့ကို ဆက်သွယ် အလုပ်လုပ်ခွင့် ပေးမထားပါဘူး။ ဘာကြောင့်လည်းဆိုတော့ အစပိုင်းတုန်းက JavaScript တွေကို low-level access မလိုတဲ့ browser တွေအတွက် ဖန်တီးထားခဲ့လို့ပါ။

<!-- JavaScript's capabilities greatly depend on the environment it's running in. For instance, [Node.js](https://wikipedia.org/wiki/Node.js) supports functions that allow JavaScript to read/write arbitrary files, perform network requests, etc. -->
JavaScript ရဲ့လုပ်ဆောင်နိုင်စွမ်းဟာ သူ ဘယ်မှာ Run နေလည်းဆိုတဲ့ environment အပေါ်မှာ မူတည်ပါတယ်။ ဥပမာ - [Node.js](https://wikipedia.org/wiki/Node.js) ဆိုလျှင် JavaScript နဲ့ Files တွေ read/write လုပ်တာ , network request တွေလုပ်တာ စသည်ဖြင့် လုပ်ဆောင်နိုင်ပါတယ်။

<!-- In-browser JavaScript can do everything related to webpage manipulation, interaction with the user, and the webserver. -->
Browser မှာ ပါဝင်တဲ့ JavaScript တွေကတော့ webpage တွေဖော်ပြတာ, အသုံးပြုသူတွေ user နဲ့ webserver ကို ချိတ်ဆက်ပေးတာ စသည်ဖြင့် လုပ်ဆောင်နိုင်ပါတယ်။ 
              
<!-- For instance, in-browser JavaScript is able to: -->
ဥပမာ အားဖြင့် , Browser မှ JavaScript တွေဟာ : 

<!-- - Add new HTML to the page, change the existing content, modify styles. -->
- Html တွေ အလုပ်လုပ်နိုင်အောင် လုပ်ဆောင်ပေးတာ ၊ ရှိနေတဲ့ content တွေကို update လုပ်ပေးတာ ၊ Styles တွေ ချိန်းပေးတာ 
<!-- - React to user actions, run on mouse clicks, pointer movements, key presses. -->
- User actions တွေကို လုပ်ဆောင်ပေးတာ ဥပမာ mouse clicks, pointer movements, key pressess
<!-- - Send requests over the network to remote servers, download and upload files (so-called [AJAX](https://en.wikipedia.org/wiki/Ajax_(programming)) and [COMET](https://en.wikipedia.org/wiki/Comet_(programming)) technologies). -->
- Server ဆီကို network ကနေ တစ်ဆင့် request တွေ ပေးပို့ခြင်း ၊ files တွေ download ချတာ upload တင်တာ (so-called [AJAX](https://en.wikipedia.org/wiki/Ajax_(programming)) and [COMET](https://en.wikipedia.org/wiki/Comet_(programming)) technologies)

<!-- - Get and set cookies, ask questions to the visitor, show messages. -->
- cookies တွေ သိမ်းဆည်းတာ ၊ ထုတ်ယူတာ ၊ website ကို လာတဲ့ သူတွေကို မေးခွန်းတွေမေးတာ ၊ message တွေ ပြပေးတာ

<!-- - Remember the data on the client-side ("local storage"). -->
- client-side (local storage) က data တွေကို ပြန်လည်ထုတ်ယူတာ

စသည်ဖြင့် လုပ်ဆောင်နိုင်ပါတယ်။

<!-- ## What CAN'T in-browser JavaScript do? -->
## Browser မှာ ပါတဲ့ JavaScript တွေက ဘာတွေမလုပ်နိုင်ဘူးလည်း?

<!-- JavaScript's abilities in the browser are limited for the sake of the user's safety. The aim is to prevent an evil webpage from accessing private information or harming the user's data. -->
Browser မှာ အလုပ်လုပ်တဲ့ JavaScript တွေရဲ့ လုပ်ဆောင်နိုင်စွမ်းဟာ အသုံးပြူသူတွေရဲ့ လုံခြုံရေး ကြောင့် ကန်သတ်မှုတွေလုပ်ထားပါတယ်။ ရည်ရွယ်ချက်ကတော့ မသမာတဲ့ webpage တွေကနေ အသုံးပြုသူတွေရဲ့  private အချက်အလက်တွေ ရယူတာ ဒါမှမဟုတ် အသုံးပြုသူတွေရဲ့  အချက်အလက်တွေကို ဖျက်စီးပြစ်တာ စသည့် အကြောင်းအရာတွေ ဖြစ်နိုင်တာကြောင့်ပါ။

<!-- Examples of such restrictions include: -->
ဥပမာ ဘယ်လိုဟာတွေကို ကန့်သတ်ထားလည်းဆိုတော့:

<!-- - JavaScript on a webpage may not read/write arbitrary files on the hard disk, copy them or execute programs. It has no direct access to OS functions. -->
- Webpage တစ်ခုမှာ ရှိတဲ့ JavaScript တွေဟာ hard disk ပေါ်မှာ files တွေကို read/write လုပ်တာ , ကူးယူတာ ဒါမှမဟုတ် program တွေကို run တာ တွေမလုပ်နိုင်ပါဘူး။ သူတို့ကို OS functions တွေနဲ့ တိုက်ရိုက် အလုပ်လုပ်ခွင့် ပေးမထားပါဘူး။

    <!-- Modern browsers allow it to work with files, but the access is limited and only provided if the user does certain actions, like "dropping" a file into a browser window or selecting it via an `<input>` tag. -->
    နောက်ပိုင်း browsers တွေကတော့ files တွေနဲ့ အလုပ်လုပ်ခွင့်ပေးထားပါတယ် ဒါပေမယ့် သတ်မှတ်ထားတဲ့ လုပ်ဆောင်ချက်တွေက လွဲပြီး ကျန်တာလုပ်ခွင့်မပေးပါဘူး ဥပမာ files တွေကို drag and drop လုပ်ပြီး browser ပေါ်တင်တာတို့ ဒါမှမဟုတ် `<input>` tag ကို သုံးပြီး files တွေကို ရွေးချယ်တာ စသည်ဖြင့်ပါ။

    <!-- There are ways to interact with camera/microphone and other devices, but they require a user's explicit permission. So a JavaScript-enabled page may not sneakily enable a web-camera, observe the surroundings and send the information to the [NSA](https://en.wikipedia.org/wiki/National_Security_Agency). -->
    camera/microphone အပြင် တခြား devices တွေ နဲ့ ချိတ်ဆက် အလုပ်လုပ်နိုင် ဖို့ အသုံးပြုသူ User ရဲ့ permission တော့လိုအပ်ပါတယ်။ ထို့မှသာ JavaScript အလုပ်လုပ်ခွင့်ပေးထားတဲ့ webpage တစ်ခုကနေ web-camera ကို အသုံးပြုပြီး နောက်ကွယ်ကနေ User တွေရဲ့ အချက်အလက်တွေကို [NSA](https://en.wikipedia.org/wiki/National_Security_Agency) စသည့် အဖွဲ့အစည်းတွေကို မပေးပို့နိုင်မှာပါ။ 

<!-- - Different tabs/windows generally do not know about each other. Sometimes they do, for example when one window uses JavaScript to open the other one. But even in this case, JavaScript from one page may not access the other if they come from different sites (from a different domain, protocol or port). -->
- မတူညီတဲ့ tabs/window တွေဟာ ပုံမှန်အားဖြင့် အဆက်အစပ်မရှိပါဘူး။ တစ်ခါတစ်လေတော့ ရှိနိုင်ပါတယ်။ ဥပမာအားဖြင့် Browser မှာ tab တစ်ခုကနေ နောက်ထပ် tab တစ်ခုကို ဖွင့်တယ် ဆိုပါစို့ ၊ အဲ့နေရာမှာ အသစ်ဖွင့်လိုက်တဲ့ tab က မူလ tab နဲ့ မတူညီတဲ့ sites (မတူညီတဲ့ domain, protocol or port) တစ်ခုဖြစ်နေမယ်ဆိုရင် access မရနိုင်ပါဘူး။

    <!-- This is called the "Same Origin Policy". To work around that, *both pages* must agree for data exchange and contain a special JavaScript code that handles it. We'll cover that in the tutorial. -->
    ထိုအရာကို "Same Origin Policy" လို ခေါ်ပါတယ်။ သူနဲ့ အလုပ်လုပ်နိုင်ဖို့ဆိုရင် မူလ page နဲ့ အသစ် ဖွင့်လိုက်တဲ့ page နှစ်ခုစလုံးက data exchange လုပ်ဖို့ သဘောတူရမှာ ဖြစ်ပြီး သတ်မှတ်ထားတဲ့ JavaScript Code တွေကနေ လုပ်ဆောင်ပေးမှာ ဖြစ်ပါတယ်။ နောက် သင်ခန်းစာတွေမှာ ထပ်ပြီး ရှင်းပြပါမယ်။


    <!-- This limitation is, again, for the user's safety. A page from `http://anysite.com` which a user has opened must not be able to access another browser tab with the URL `http://gmail.com` and steal information from there. -->
    အဲ့လို ကန့်သတ်မှုတွေက ထပ်ပြောရရင် user တွေရဲ့ လုံခြုံရေး ကြောင့်ပါပဲ။ ဥပမာ user ဖွင့်ထားတဲ့ `http://anysite.com` ဆိုတဲ့ tab တစ်ခုကနေ နောက်ထပ် tab တစ်ခုဖြစ်တဲ့ `http://gmail.com` က အချက်အလက်တွေကို မရယူနိုင်ပါဘူး

<!-- - JavaScript can easily communicate over the net to the server where the current page came from. But its ability to receive data from other sites/domains is crippled. Though possible, it requires explicit agreement (expressed in HTTP headers) from the remote side. Once again, that's a safety limitation. -->
- JavaScript မှာ web server ရဲ့ domain နဲ့ လက်ရှိ web page domain တူတယ်ဆိုရင် အလွယ်တကူ ချိတ်ဆက်နိုင်ပါတယ်။ ဒါပေမယ့် လက်ရှိ website ကနေ တစ်ခြား sites/domains က အချက်အလက်တွေ ရယူဖို့ကတော့ သိပ်တော့ မရိုးရှင်းပါဘူး။ တကယ်လို့ တခြား websites/domain က တိကျတဲ့ သဘောတူညီမှု (ထိုအရာကို HTTP headers တွင် ဖော်ပြကျပါတယ်) တစ်ခုရှိရင်တော့ ဖြစ်နိုင်ပါတယ်။ ထပ်ပြောရရင် ဒါကလည်း လုံခြုံရေး ကန့်သတ်ချက်တစ်ခုပါပဲ။

![](limitations.svg)

<!-- Such limits do not exist if JavaScript is used outside of the browser, for example on a server. Modern browsers also allow plugin/extensions which may ask for extended permissions. -->
တကယ်လို့သာ JavaScript ကို Browser မှာ မဟုတ်ပဲ တစ်ခြားနေရာမှာ သုံးမယဆိုရင် အဲ့လို ကန့်သတ်ချက်တွေ မရှိပါဘူး။ ဥပမာ Server ပေါ်မှာ ဆိုရင်ပေါ့။ နောက်ပိုင်း Browser တွေကတော့ plugin/extensions တွေကို ထပ်တိုး permissions တွေတောင်းပြီး အလုပ်လုပ်နိုင်ပါတယ်။

<!-- ## What makes JavaScript unique? -->
## ဘယ်အရာက JavaScript ကို ထူးခြားစေလည်း?

<!-- There are at least *three* great things about JavaScript: -->
JavaScript နဲ့ ပတ်သတ်ပြီး အကောင်းဆုံး အချက် ၃ ချက်ကတော့:

```compare
<!-- + Full integration with HTML/CSS. -->
+ HTML/CSS တွေနဲ့ အပြည့်အဝ အလုပ်လုပ်တာ.
<!-- + Simple things are done simply. -->
+ ရိုးရှင်းတဲ့ ကိစ္စတွေကို ရိုးရှင်းစွာ လုပ်ဆောင်နိုင်တာ.
<!-- + Support by all major browsers and enabled by default. -->
+ အဓိက browsers အားလုံးမှာ အလုပ်လုပ်ပြီး default ပါဝင်တာ.
```
<!-- JavaScript is the only browser technology that combines these three things. -->
JavaScript ဟာ ထို အချက်သုံးချက်ကို Browser ပေါ်မှာ လုပ်ဆောင်နိုင်တဲ့ တစ်ခုတည်းသော နည်းပညာ ဖြစ်ပါတယ်။

<!-- That's what makes JavaScript unique. That's why it's the most widespread tool for creating browser interfaces. -->
အဲ့ဒီအရာကပဲ JavaScript ကို ထူးခြားစေပြီး browser interfaces တွေကို ဖန့်တီးတဲ့ လူသုံးအများဆုံး tool တစ်ခု ဖြစ်နေတာပါပဲ

<!-- That said, JavaScript also allows to create servers, mobile applications, etc. -->
ဒါအပြင် JavaScript ကိုသုံးပြီး server တွေ mobile applications, စတဲ့ အရာတွေလည်း ဖန်တီးနိုင်ပါတယ်။

<!-- ## Languages "over" JavaScript -->
## JavaScript ကို အခြေခံထားတဲ့ Languages များ

<!-- The syntax of JavaScript does not suit everyone's needs. Different people want different features. -->
JavaScript ရဲ့ ရေးသားပုံတွေ က လူတိုင်းရဲ့ လိုအပ်ချက်နဲ့ တော့ မကိုက်ညီ နိုင်ပါဘူး။ မတူညီတဲ့ သူတွေမှာ မတူညီတဲ features တွေ လိုအပ်ကျပါတယ်။

<!-- That's to be expected, because projects and requirements are different for everyone. -->
ဒါကလည်း ဖြစ်နိုင်ပါတယ်။ ဘာကြောင့်လည်းဆိုတော့ projects and requirements တွေက လူတိုင်း မတူလို့ပါ။

<!-- So recently a plethora of new languages appeared, which are *transpiled* (converted) to JavaScript before they run in the browser. -->
ဒါကြောင့် မကြာသေးမှီ အချိန်အတွင်းမှာ Language အသစ်တွေ အများကြီးပေါ်လာပါတယ်။ အဲ့ဒီ Langulage တွေဟာ browser ပေါ်မှာ အလုပ်မလုပ်ခင် JavaScript code ကို ပြောင်းပြီး အလုပ်လုပ်ပေးပါတယ်။

<!-- Modern tools make the transpilation very fast and transparent, actually allowing developers to code in another language and auto-converting it "under the hood". -->
နောက်ပိုင်း tools တွေဟာ source code တစ်ခုကနေ နောက်တစ်ခုကို လျှင်လျှင်မြန်မြန် နဲ့ တိတိကျကျ ပြောင်းပေးနိုင်ပါတယ်။ တကယ်တော့ ချိတ်ဆက်မှု တစ်ခုအောက်မှာ developers တွေကို langulage ရဲ့ code တွေကို နောက်တစ်ခုကို ပြောင်းပေးတာပါပဲ။ 

<!-- Examples of such languages: -->
အဲ့လို Languages တွေကတော့ :

<!-- - [CoffeeScript](http://coffeescript.org/) is a "syntactic sugar" for JavaScript. It introduces shorter syntax, allowing us to write clearer and more precise code. Usually, Ruby devs like it. -->
- [CoffeeScript](http://coffeescript.org/) ကတော့ JavaScript ကို "syntactic sugar" လုပ်ပေးထားတာပါ (Sugar လုပ်ထားတယ်ဆိုတာက အခြေခံအားဖြင့် ရှည်တဲ့ syntex တွေကို တိုတိုလေး ရေးလို့ရအောင်လုပ်ပေးထားတာပါ). သူမှာ syntex တွေကို တိုတိုလေး နဲ့ ပိုရှင်း ပိုပြီး တိကျတဲ့ syntex တွေနဲ့ ​ရေးနိုင်ပါတယ်။ ပုံမှန်တော့ Reby developer တွေ သဘောကျ ကျပါတယ်။
<!-- - [TypeScript](http://www.typescriptlang.org/) is concentrated on adding "strict data typing" to simplify the development and support of complex systems. It is developed by Microsoft. -->
- [TypeScript](http://www.typescriptlang.org/) ကတော့ "strict data typing" (stick data type ဆိုတာ strong data type ကို ဆိုလိုတာပါ။ ဥပမာ string + number လုပ်လို့မရပါဘူး) ကို ပို အာရုံစိုက်ထားပြီး development တွေကို ပိုမို ရိုးရှင်းအောင် လုပ်ဆောင်ပေးပြီး ရှုပ်ထွေးတဲ့ systems တွေ အတွက်လည်း အထောက်အကူဖြစ်အောင် လုပ်ပေးထားပါတယ်။ သူ့ကို Microsoft က ဖန်တီးထားပါတယ်။
<!-- - [Flow](http://flow.org/) also adds data typing, but in a different way. Developed by Facebook. -->
- [Flow](http://flow.org/) မှာတော့ data type တွေထည့်ပေးထားပါတယ်။ ဒါပေမယ့် မတူတဲ့ ပုံစံနဲ့ပါ။ Facebook က ဖန်တီးထားပါတယ်။.
<!-- - [Dart](https://www.dartlang.org/) is a standalone language that has its own engine that runs in non-browser environments (like mobile apps), but also can be transpiled to JavaScript. Developed by Google. -->
- [Dart](https://www.dartlang.org/) ကတော့ သီခြားဖြစ်နေတဲ့ langulage တစ်ခုဖြစ်ပြီး သူ့ရဲ့ ကိုယ်ပိုင် engine နဲ့ browser မဟုတ်တဲ့ environment မှာ အလုပ်လုပ်နိုင်ပါတယ်။ ဥပမာ mobile apps.သူ့လည်း JavaScript code ကို ပြောင်းနိုင်ပါတယ်။ Google က ဖန်တီးထားပါတယ်။
<!-- - [Brython](https://brython.info/) is a Python transpiler to JavaScript that enables the writing of applications in pure Python without JavaScript. -->
- [Brython](https://brython.info/) ကတော့ Python code က နေ JavaScript code ကို ပြောင်းပေးနိုင်ပြီးတော့ pure python နဲ့ ရေးထားတဲ့ code တွေကို JavaScript ကို ပြောင်းနိုင်ပါတယ်။
<!-- - [Kotlin](https://kotlinlang.org/docs/reference/js-overview.html) is a modern, concise and safe programming language that can target the browser or Node. -->
- [Kotlin](https://kotlinlang.org/docs/reference/js-overview.html) ကတော့ ထွက်လာတာ မကြာသေးတဲ့ language ဖြစ်ပြီး ကျစ်ကျစ်လစ်လစ် နဲ့ safe programming langulage တစ်ခု ဖြစ်ပါတယ်။ သူကို့တော့ browser နဲ့ Node မှာ အသုံးပြုလို့ရပါတယ်။

<!-- There are more. Of course, even if we use one of transpiled languages, we should also know JavaScript to really understand what we're doing. -->
နောက်ထပ်လည်း အများကြီး ရှိနိုင်ပါသေးတယ်။ တကယ်လို့ transpiled language (langulage တစ်ခုကနေ တစ်ခြား langulage တစ်ခုကို ပြောင်းပေးနိုင်သော language) ကို သုံးနေတယ်ဆိုရင်တောင်မှ ကိုယ်ဘာလုပ်နေလည်း ဆိုတာကို သိဖို့ JavaScript ကို နားလည်ဖို့လိုပါတယ်။

<!-- ## Summary -->
## အနှစ်ချုပ်

<!-- - JavaScript was initially created as a browser-only language, but it is now used in many other environments as well. -->
- JavaScript ကို အစပိုင်းမှာ browser အတွက်ပဲ တီထွင်ထားခဲ့ပေမယ် အခုတော့ တစ်ခြား နေရာတွေမှာပါ သုံးလို့ရနေပါပြီ။
<!-- - Today, JavaScript has a unique position as the most widely-adopted browser language with full integration in HTML/CSS. -->
- ဒီကနေ့မှာတော့ JavaScript ဟာ HTML/CSS နဲ့ အပြည့်အဝ အလုပ်လုပ်နိုင်တဲ့ လူသုံးအများဆုံး browser language တစ်ခု ဖြစ်နေပါပြီ။
<!-- - There are many languages that get "transpiled" to JavaScript and provide certain features. It is recommended to take a look at them, at least briefly, after mastering JavaScript. 
-->
- အခုတော့ "transpiled language" တွေ အများကြီးရှိနေပါပြီဖြစ်ပြီး တကယ်လို့ JavaScript ကျွမ်းကျင်သွားပြီလို့ ထင်ရင် တခြား "transpiled language" တွေကိုလည်း လေ့လာသင့်ပါတယ်။
