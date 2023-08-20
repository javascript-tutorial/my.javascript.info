# Hello, world!

<!-- This part of the tutorial is about core JavaScript, the language itself. -->

ဒီ လေ့ကျင့်ခန်းကတော့ JavaScript Lanaguage ရဲ့ အခြေခံအကျဆုံး အကြောင်းအရာတွေကို လေ့လာရမှာ ဖြစ်ပါတယ်။

<!-- But we need a working environment to run our scripts and, since this book is online, the browser is a good choice. We'll keep the amount of browser-specific commands (like `alert`) to a minimum so that you don't spend time on them if you plan to concentrate on another environment (like Node.js). We'll focus on JavaScript in the browser in the [next part](/ui) of the tutorial. -->

ဒါပေမယ့် အဲ့ဒီ အကြောင်းအရာတွေကို မလေ့လာခင် အရင်ဆုံး ကျွန်တော်တို့ရေးထားတဲ့ scripts တွေကို run လို့ရတဲ့ environment တစ်ခုလိုပါတယ်။

အရမ်းတွေးနေစရာမလိုပါဘူး။

ကျွန်တော်တို့ အခုလက်ရှိ သုံးနေတဲ့ browser ကိုပဲ သုံးကျတာပေါ့။ ဒါအပြင် brower ပေါ်မှာပဲ သုံးလို့ရတဲ့ commands တွေကို အခုလေ့ကျင့်ခန်းမှာ အတတ်နိုင်ဆုံး နည်းအောင် သုံးသွားပါမယ်။ ဥပမာ `alert` လိုမျိုးပေါ့။

ဒါကြောင့် တစ်ခြား environment ကို သုံးပြီး လေ့ကျင့်ချင်သူတွေ အတွက်လည်း အဆင်ပြေပါလိမ့်မယ်။ ဆိုတော့ ကျွန်တော်တို့ ဒီ လေ့ကျင့်ခန်းရဲ့ [နောက် တစ်ခန်း](/ui) ကနေ စပြီး browser environment ကိုပဲ သုံးသွားပါမယ်။

<!-- So first, let's see how we attach a script to a webpage. For server-side environments (like Node.js), you can execute the script with a command like `"node my.js"`. -->

အဲ့တော့ အရင်ဆုံး ကျွန်တော်တို့ ရေးထားတဲ့ scripts တွေကို webpage မှာ ဘယ်လို run မလည်း ကြည့်ရအောင်။ တကယ်လို့ server-side environments (ဥပမာ Node.js) ကို သုံးပြီး run မယ်ဆိုရင် `"node my.js"` လို့ ရိုက်ပြီး run လို့ရပါတယ်။ `my.js` ဆိုတာက ကိုယ် run မယ့် js file ကို ပြောတာပါ။

## The "script" tag

<!-- JavaScript programs can be inserted almost anywhere into an HTML document using the `<script>` tag. -->

JavaScript code တွေကို HTML ဖိုင် ရဲ့ ဘယ်နေရာမှာမဆို `<script>` tag နဲ့ ရေးလို့ရပါတယ်။

<!-- For instance: -->

ဥပမာ:

```html run height=100
<!DOCTYPE html>
<html>
  <body>
    <p>Before the script...</p>

    *!*
    <script>
      alert("Hello, world!");
    </script>
    */!*

    <p>...After the script.</p>
  </body>
</html>
```

```online
<!-- You can run the example by clicking the "Play" button in the right-top corner of the box above. -->
အခု ဥပမာ ရဲ့ ညာဖက် ထောင့်နားက "Play" button လေးကို နှိပ်ပြီး run ကြည့်လို့ရတယ်နော်။
```

<!-- The `<script>` tag contains JavaScript code which is automatically executed when the browser processes the tag. -->

Browser က စပြီး အဲ့ဒီ `<script>` tag ခေါ်လိုက်ပြီ ဆိုတာနဲ့ သူ့ထဲက JavaScript code တွေကို အလိုအလျောက် အလုပ်လုပ်ပေးပါတယ်။

## Modern markup

<!-- The `<script>` tag has a few attributes that are rarely used nowadays but can still be found in old code: -->

`<script>` tag ထဲမှာ ထည့်ရေးလို့ရတဲ့ attributes အနည်းငယ်ရှိပါတယ်။ ဒါပေမယ့် အခုတော့ သုံးတာ တော်တော်ရှားသွားပါပြီ။ ဒါပေမယ့် ဟိုးအရင်တုန်းက code တွေမှာတော့ တွေ့နိုင်ပါသေးတယ်။ (စာရေးသူ : attributes နဲ့ properties က မတူပါ)
<br/><br/>

The `type` attribute: <code>&lt;script <u>type</u>=...&gt;</code>
<br/><br/>

<!-- : The old HTML standard, HTML4, required a script to have a `type`. Usually it was `type="text/javascript"`. It's not required anymore. Also, the modern HTML standard totally changed the meaning of this attribute. Now, it can be used for JavaScript modules. But that's an advanced topic, we'll talk about modules in another part of the tutorial. -->

အရင် HTML standard ဖြစ်တဲ့ HTML4 မှာတော့ `type` ဆိုတဲ့ attribute ကို ထည့်ပေးဖို့လိုပါတယ်။ ပုံမှန် ကတော့ `type="text/javascript"` လို့ ထည့်ရေးရပြီး အခုကတော့ ထည့်ရေးစရာ မလိုတော့ပါဘူး။ ဒါ့အပြင် အခုနောက်ပိုင်း HTML standard မှာတော့ အဲ့ `type` ဆိုတဲ့ attribute ရဲ့ အဓိပ္ပါယ်ကတော့ အရင်ကနဲ့ လုံးဝကို မတူတော့ပါဘူး။ 

သူကို JavaScript ရဲ့ modules တစ်ခုအနေနဲ့ သုံးလို့ရနေပါပြီ။ အဲ့ အကြောင်းတွေက အဆင်မြင့် level ဖြစ်လို့ အခုတော့ ထပ်မရှင်းပြတော့ပါဘူး။ နောက်လာမယ့် modules အခန်း ကျမှ ပြောပြပါမယ်။
<br/><br/>

The `language` attribute: <code>&lt;script <u>language</u>=...&gt;</code>
<br/><br/>

<!-- : This attribute was meant to show the language of the script. This attribute no longer makes sense because JavaScript is the default language. There is no need to use it. -->

ဒီ attribute ရဲ့ ရည်ရွယ်ချက်ကတော့ ဘယ် language ကို သုံးပါမယ်ဆိုတာကို သတ်မှတ်ပေးတာ ဖြစ်ပါတယ်။ `<script>` tag ထဲမှာ JavaScript က default langulage ဖြစ်လို့ သိပ်တော့ အဓိပ္ပါယ် မရှိပါဘူး။ အဲ့တော့ ထည့်ရေးစရာ မလိုတော့ပါဘူး။
<br/><br/>

### Comments before and after scripts.

<!-- : In really ancient books and guides, you may find comments inside `<script>` tags, like this: -->

ဟိုးအရင်တုန်းက စာအုပ်တွေ နဲ့ လေကျင့်ခန်းတွေမှာ တစ်ချို့ comments တွေကို `<script>` ထဲထည့်ရေးတာကို တွေ့ပါလိမ့်မယ်။ ဥပမာ:

```html no-beautify
    <script type="text/javascript"><!--
        ...
    //--></script>
```

<!-- This trick isn't used in modern JavaScript. These comments hide JavaScript code from old browsers that didn't know how to process the `<script>` tag. Since browsers released in the last 15 years don't have this issue, this kind of comment can help you identify really old code. -->

Comments တွေကို Browser အား process မလိုစေလိုတဲ့ ဟာတွေကို ထည့်ရေးလေ့ ရှိပါတယ်။ ဟိုးအရင်က Browser တွေမှာ HTML ဖိုင်ထဲက script tag တွေကို ဘယ်လို run ရမလည်း မသိခင်မှာ အာလို comment ပိတ်ထားပြီး သုံးကျပါတယ်။ 

ထိုကဲ့သို့ လုပ်လိုက်ချင်းအားဖြင့် browser က comments လုပ်ထားတဲ့ line တွေကို process မလုပ်တော့ပဲနဲ့ ကျော်ပစ်လိုက်ပြီး ဖြစ်နိုင်ခြေရှိတဲ့ error တွေ မတက်တော့ပါဘူး။ ဒါပေမယ့် အခု အာလိုလုပ်ဖို့မလိုအပ်တော့ပါဘူး။ ကိုယ့် project ထဲမှာ ထို့ကဲ့သို့  comments တွေကို ကြည့်ချင်းအားဖြင့် code က အဟောင်းလား ဆိုတာ သိနိုင်ပါတယ်။

## External scripts

<!-- If we have a lot of JavaScript code, we can put it into a separate file. -->
တကယ်လို့ ကိုယ့်မှာ JavaScript code တွေအရမ်းများလာရင် file တစ်ခုထဲ စုပြုံရေးလို့ မရတော့ပါဘူး။ အာလိုအခြေအနေမျိုးမှာ file တွေ ကို သပ်သပ်စီခွဲရေးလို့ရပါတယ်။

<!-- Script files are attached to HTML with the `src` attribute: -->
ထိုသို့ ခွဲရေးထားတဲ့ Javascript file တွေကို HTML ဖိုင်ထဲ ထည့်ပြီး အလုပ်လုပ်စေချင်တယ်ဆိုရင် script tag ထဲ src ဆိုတဲ့ attribute နဲ့ point လုပ်ပေးရပါတယ်။

```html
<script src="/path/to/script.js"></script>
```
<!-- 
Here, `/path/to/script.js` is an absolute path to the script from the site root. One can also provide a relative path from the current page. For instance, `src="script.js"`, just like `src="./script.js"`, would mean a file `"script.js"` in the current folder. -->
အပေါ်က ဥပမာ ထဲမှာဆိုရင် `/path/to/script.js` ဆိုတဲ့ file path အတိအကျကို ညွှန်ပြထားသလိုပဲ JavaScript file ရဲ့ တည့်နေရာနဲ့ HTML ရဲ့ တည်နေရာကို မူတည်ပြီး လည်း ညွှန်ပြလို့ရပါတယ်။ ဥပမာ `src="script.js"`, `src="./script.js"` အာလိုရေးထားမယ်ဆိုရင် သူက လက်ရှိ HTML file ရှိတဲ့ same folder ထဲက script.js file ကို ညွှန်ပြပေးတာ ဖြစ်ပါတယ်။


တကယ်လို့ ကိုယ်က တစ်ခြား website က JavaScript ကို သုံးချင်တယ်ဆိုရင်လည်း URL အတိအကျကို ညွှန်ပြပြီး သုံးလို့ရပါတယ်။ ဥပမာ : 

<!-- We can give a full URL as well. For instance: -->

```html
<script src="https://cdnjs.cloudflare.com/ajax/libs/lodash.js/4.17.11/lodash.js"></script>
```

တစ်ခုထပ်ပိုတဲ့ JavaScript file တွေကို သုံးချင်တယ်ဆိုရင် script tag တွေ ထပ်ဖွင့်ပြီး ရေးသွားလို့ရပါတယ်။
<!-- To attach several scripts, use multiple tags: -->

```html
<script src="/js/script1.js"></script>
<script src="/js/script2.js"></script>
…
```

```smart
<!-- As a rule, only the simplest scripts are put into HTML. More complex ones reside in separate files. -->
စည်းကမ်းအရကတော့ ရိုးရှင်းတဲ့ scripts တွေကို ပဲ HTML ထဲ တိုက်ရိုက်ရေးသင့်ပါတယ်။ ရှုပ်ထွေးတဲ့ scripts တွေကို တစ်ခြား JavaScript file ထဲမှာ ခွဲရေးပါ။

<!-- The benefit of a separate file is that the browser will download it and store it in its [cache](https://en.wikipedia.org/wiki/Web_cache). -->
အဲ့လို file သတ်သတ်ခွဲရေးလိုက်ခြင်းရဲ့ ကောင်းတဲ့ အချက်က ပထမဆုံး run လိုက်တာနဲ့  browser က အဲ့ဒီ JavaScript file ကို download လုပ်ပြီး [cache](https://en.wikipedia.org/wiki/Web_cache) ထဲမှာ သိမ်းထားလိုက်ပါတယ်။

<!-- Other pages that reference the same script will take it from the cache instead of downloading it, so the file is actually downloaded only once. -->
တကယ်လို့ နောက်ထပ် HTML file တွေကနေ အဲ့ဒီ script file ကို ပဲ ထပ်သုံးမယ်ဆိုရင် နောက်တစ်ခါ download ထပ်လုပ်စရာမလိုတော့ပဲ cache ထဲကနေပဲ တိုက်ရိုက် သုံးလိုက်လို့ loading time ကို ပိုမြန်သွားစေပါတယ်။
<!-- That reduces traffic and makes pages faster. -->
```

<!-- ````warn header="If `src`is set, the script content is ignored." -->
````warn header="တကယ်လို့ `src` attribute ကို သုံးထားတယ်ဆိုရင် script tag ထဲမှာ ရေးထားတဲ့ ဟာတွေကို ကျော်ပစ်လိုက်ပါတယ်။"
<!-- A single`<script>`tag can't have both the`src` attribute and code inside. -->
သဘောတရားကတော့ `<script>`tag တစ်ခုမှာ `src` attribute နဲ့ code တွေကို တစ်ပြိုင်တည်း သုံးလို့မရပါဘူး။ တစ်ခုပဲ ရပါတယ်။

<!-- This won't work: -->
ဒါမျိုးရေးမယ်ဆိုရင် အလုပ်မလုပ်ပါဘူး:

```html
<script *!*src*/!*="file.js">
  alert(1); // ဒီ content က အလုပ်မလုပ်ပါဘူး။ ဘာလို့လည်းဆိုတော့ အပေါ်မှာ src attribute ကို သုံးထားလို့ပါ။
</script>
```
ဒါကြောင့်မို့လို့ `<script src="…">` လား (သို့မဟုတ်) ပုံမှန် `<script>` ဆိုတာကို ရွေးချယ်သုံးရပါမယ်။
<!-- We must choose either an external `<script src="…">` or a regular `<script>` with code. -->

အပေါ်က ဥပမာ ကို အလုပ်လုပ်စေချင်ရင် script tag နှစ်ခု ခွဲပြီး ရေးပေးရပါမယ်။ ဥပမာ
<!-- The example above can be split into two scripts to work: -->

```html
<script src="file.js"></script>
<script>
  alert(1);
</script>
```

```

## အနှစ်ချုပ်

- `<script>` tag ကို သုံးပြီးတော့ JavaScript code တွေကို run လို့ရပါတယ်။
- `type` နဲ့ `language` attributes တွေက မတူပါဘူး။
- ခွဲရေးထားတဲ့ JavaScript file တွေကို <script src=..> ကို သုံးပြီး ညွှန်ပြလို့ရပါတယ်။ ဥပမာ `<script src="path/to/script.js"></script>`

Browser scripts တွေနဲ့ webpage တွေ ဘယ်လို အလုပ်လုပ်တယ်ဆိုတာလေ့လာဖို့က အများကြီး ကျန်ပါသေးတယ်။ အခု လက်ရှိ ကျွန်တော်တို့က JavaScript language ကိုပဲ လေ့လာနေတာကြောင့် တခြား browser နဲ့ ပတ်သတ်တဲ့ အလုပ်လုပ်ပုံတွေကို ဖယ်ထားလိုက်ပါအုန်းမယ်။ ဒါကြောင့် Browser ကို ကျွန်တော်တို့ လက်ရှိ လေ့လာနေတဲ့ JavaScript ကို run ဖို့အတွက်ပဲ လိုအပ်တာတွေကို လေ့လာကျတာပေါ့။ 

```
