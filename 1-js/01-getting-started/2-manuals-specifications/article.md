# Manual နဲ့ သတ်မှတ်ချက်

<!-- # Manuals and specifications -->


<!-- This book is a *tutorial*. It aims to help you gradually learn the language. But once you're familiar with the basics, you'll need other sources. -->
ဒီစာအုပ်က *tutorial* တစ်ခုဖြစ်ပါတယ်။ JavaScript ကို တစ်ဖြည်းဖြည်းချင်း လေ့လာနိုင်အောင် ရည်ရွယ်ထားတယ်။ တကယ်လို့ အခြေခံ အချက်တွေကို နားလည်သွားပြီဆိုရင် တခြား လေ့လာစရာတွေကို ထပ်လေ့လာဖို့ လိုပါလိမ့်မယ်။

<!-- ## Specification -->
## သတ်မှတ်ချက်

<!-- [The ECMA-262 specification](https://www.ecma-international.org/publications/standards/Ecma-262.htm) contains the most in-depth, detailed and formalized information about JavaScript. It defines the language. -->
[The ECMA-262 specification](https://www.ecma-international.org/publications/standards/Ecma-262.htm) ဆိုတဲ့ သတ်မှတ်ချက် တွေမှာ JavaScript နဲ့ ပတ်သတ်ပြီး အသေးစိတ် , အခြေခံကျကျ နဲ့ တိကျတဲ့ အချက်အလက်တွေ ပါဝင်ပါတယ်။

<!-- But being that formalized, it's difficult to understand at first. So if you need the most trustworthy source of information about the language details, the specification is the right place. But it's not for everyday use. -->
အဲ့လို အသေးစိတ် အချက်အလက်တွေ ကြောင့်ပဲ အစပိုင်းမှာ နားလည်ဖို့ ခက်ခဲ့ပါတယ်။ ဒါကြောင့် language ရဲ့ အချက်အလက် တွေနဲ့ ပတ်သတ်ပြီး ယုံကြည်ရတဲ့ ရင်းမြစ်တစ်ခုလိုနေတယ် ဆိုရင် သတ်မှတ်ချက်တွေ ကို လေ့လာတာက မှန်ကန်တဲ့ အရာပါပဲ။ ဒါပေမယ့် နေစဉ်အသုံးပြုဖို့တော့ မဟုတ်ပါဘူး။

<!-- A new specification version is released every year. In-between these releases, the latest specification draft is at <https://tc39.es/ecma262/>. -->
နှစ်စဉ်နှစ်တိုင်း သတ်မှတ်ချက် အသစ်တွေ ထွက်ပါတယ်။ အဲ့ မထွက်ခင် အတောအတွင်း သတ်မှတ်ချက်တွေကို <https://tc39.es/ecma262/> မှာ သွားကြည့်လို့ရပါတယ်။

<!-- To read about new bleeding-edge features, including those that are "almost standard" (so-called "stage 3"), see proposals at <https://github.com/tc39/proposals>. -->
အသစ်ထွက်လာမယ့် features တွေ "almost standard" (so-called "stage 3") လို့ခေါ်တဲ့ standard ဖြစ်တော့မယ့် features တွေအကြောင်းဖတ်ချင်ရင် <https://github.com/tc39/proposals> သွားဖတ်လို့ရပါတယ်။

<!-- Also, if you're developing for the browser, then there are other specifications covered in the [second part](info:browser-environment) of the tutorial. -->
နောက်ပြီးတော့ တကယ်လို့ သင်ဟာ brower အတွက် ဖန်တီးနေတဲ့သူဆိုရင် browser environment တွေအတွက် သတ်မှတ်မှတ်ချက် တွေကို ဒီ tutorial ရဲ့ [second part](info:browser-environment) မှာ ပြောပြသွားပါမယ်။

<!-- ## Manuals -->
## Manual

<!-- - **MDN (Mozilla) JavaScript Reference** is the main manual with examples and other information. It's great to get in-depth information about individual language functions, methods etc. -->
**MDN (Mozilla) JavaScript Reference** ကတော့ ဥပမာ တွေနဲ့ အခြားအချက်အလက်တွေအတွက် အဓိက ဖြစ်ပါတယ်။ language နဲ့ ပတ်သတ်တဲ့ functions တွေ methods တွေ နဲ့ ပတ်သတ်ပြီး အသေးစိတ် အချက်အလက်တွေ လေ့လာဖို့အတွက် ကောင်းတဲ့ နေရာပါပဲ။
    <!-- One can find it at <https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference>. -->
    <https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference> ဒီမှာ သွားကြည့်လို့ရပါတယ်။

<!-- Although, it's often best to use an internet search instead. Just use "MDN [term]" in the query, e.g. <https://google.com/search?q=MDN+parseInt> to search for `parseInt` function. -->
တစ်ခါတစ်လေကျရင် internet မှာပဲ ကိုသိချင်တာကို ရှာလိုက်တာက ပိုကောင်းနိုင်ပါတယ်။ အဲ့လို အခြေမျိုးဆိုရင် "MDN [term]" ဆိုတဲ့ စာလုံးလေး ထည့်ပြီးရှာပါ။ ဥပမာ <https://google.com/search?q=MDN+parseInt> ဆိုပြီး `parseInt` အကြောင်းကို ရှာနိုင်ပါတယ်။

<!-- ## Compatibility tables -->
## တွဲဖက်လုပ်ဆောင်နိုင်မှု

<!-- JavaScript is a developing language, new features get added regularly. -->
JavaScript ဟာ တိုးတက်နေဆဲ language တစ်ခုဖြစ်ပါတယ်။ features အသစ်တွေကိုလည်း ပုံမှန် ထည့်သွင်းပေးနေပါတယ်။

<!-- To see their support among browser-based and other engines, see: -->
သူရဲ့ browser အခြေခံ နဲ့ တစ်ခြား engines တွေမှာ တွဲဖက်လုပ်ဆောင်နိုင်စွမ်းကို ကြည့်ချင်ရင် : 

<!-- - <http://caniuse.com> - per-feature tables of support, e.g. to see which engines support modern cryptography functions: <http://caniuse.com/#feat=cryptography>. -->
- <http://caniuse.com> - feature တစ်ခုချင်းစီအတွက် ထောက်ပံမှု , ဥပမာ ဘယ် engines က တော့ ဘယ် cryptography funnctions ကို ထောက်ပံပေးထားတယ် ဆိုတာမျိုး <http://caniuse.com/#feat=cryptography>
<!-- - <https://kangax.github.io/compat-table> - a table with language features and engines that support those or don't support. -->
- <https://kangax.github.io/compat-table> - ဘယ် engines တွေက ဘယ် language features တွေကို ထောက်ပံပေးလည်းဆိုတာ ဖော်ပြထားတဲ့ table တစ်ခုပါ။

<!-- All these resources are useful in real-life development, as they contain valuable information about language details, their support etc. -->
အပေါ်က အချက်အလက်တွေက တကယ်လက်တွေ့ ဖန်တီးမှုတွေမှာ အရမ်းကို အသုံးဝင်ပါတယ်။ သူတို့မှာ တန်ဖိုးရှိတဲ့ language အသေးစိတ် အချက်အလက်တွေ နဲ့ သူတို့ရဲ့ ထောက်ပံမှုတွေ စသည်ဖြင့် ပါဝင်ပါတယ်။

<!-- Please remember them (or this page) for the cases when you need in-depth information about a particular feature. -->
ဒါကြောင့် အကြောင်းအရာ တစ်ခုခုနဲ့ ပတ်သတ်ပြီး အသေးစိတ်လေ့လာဖို့ လိုအပ်လာပြီဆိုရင် အဲ့ဒီ page တွေကို သွားရောက် လေ့လာဖို့ သတိရပါ။
