# Developer console

<!-- Code is prone to errors. You will quite likely make errors... Oh, what am I talking about? You are *absolutely* going to make errors, at least if you're a human, not a [robot](https://en.wikipedia.org/wiki/Bender_(Futurama)). -->
Code ရေးတဲ့ နေရာမှာ အမှားတွေလည်း ရှိနိုင်ပါတယ်။ သင်လည်း အမှားတွေလုပ် မိပါလိမ့်မယ်... ငါဘာတွေပြောနေတာပါလိမ့်? သင်ဟာ လူတစ်ယောက်ဆိုရင် *လုံးဝ* အမှားလုပ်မိပါလိမ့်မယ် ။ [robot](https://en.wikipedia.org/wiki/Bender_(Futurama)) ဆိုရင်တော့ တစ်မျိုးပေါ့။

<!-- But in the browser, users don't see errors by default. So, if something goes wrong in the script, we won't see what's broken and can't fix it. -->
ပုံမှန်အားဖြင့် browser တွေမှာ error တွေကို အသုံးပြူသူတွေ မြင်အောင် လုပ်ပေးမထားပါဘူး။ ဒါဆိုရင် ကိုယ်ရေးလိုက်တဲ့ script တွေမှာ တစ်ခုခုမှားနေရင် ဘာမှားနေတာလည်း မသိနိုင်သလို ဘယ်လိုပြင်ရမလည်း ဆိုတာလည်း မသိနိုင်ပါဘူး။

<!-- To see errors and get a lot of other useful information about scripts, "developer tools" have been embedded in browsers. -->
ဒါကြောင့် အဲ့လို errors တွေကို ကြည့်ဖို့နဲ့ ကိုယ်ရေးတဲ့ script ရဲ့ error information တွေ သိရဖို့ browser တွေမှာ "developer tools" ကို ထည့်သွင်းပေးထားပါတယ်။

<!-- Most developers lean towards Chrome or Firefox for development because those browsers have the best developer tools. Other browsers also provide developer tools, sometimes with special features, but are usually playing "catch-up" to Chrome or Firefox. So most developers have a "favorite" browser and switch to others if a problem is browser-specific. -->
များသောအားဖြင့် developer တော်တော်များများက Chrome ဒါမှမဟုတ် Firefox ကို development လုပ်တဲ့နေရာမှာ ရွေးချယ်ကျပါတယ်။ ဘာလို့လည်းဆိုတော့ သူတို့မှာ ကောင်းမွန်တဲ့ "developer tools" ရှိလို့ပါ။ 

<!-- Developer tools are potent; they have many features. To start, we'll learn how to open them, look at errors, and run JavaScript commands. -->
Developer tools တွေမှာ features တွေ အများကြီးပါပြီး တော်တော် အသုံးဝင်ကျပါတယ်။ အဲ့တော့ ကျွန်တော်တို့ သူ့ကို ဘယ်လိုဖွင့်တယ် ၊ errors တွေ ဘယ်လိုကြည့်တယ် ဒါအပြင် Javascript commands တွေ ဘယ်လို run တယ်ဆိုတာ လေ့လာရအောင်။

## Google Chrome

<!-- Open the page [bug.html](bug.html). -->
[bug.html](bug.html) ကို နှိပ်လိုက်ပါ။

<!-- There's an error in the JavaScript code on it. It's hidden from a regular visitor's eyes, so let's open developer tools to see it. -->
သူရဲ့ JavaScript Code မှာ error တစ်ခုရှိပြီး ပုံမှန်တော့ အဲ့ဒီ error ကို မတွေ့ရအောင် ဖျောက်ထားပါတယ်။ အာဒါဆို developer tools ကို ဖွင့်ပြီး ကြည့်ရအောင်..

<!-- Press `key:F12` or, if you're on Mac, then `key:Cmd+Opt+J`. -->
`key:F12` (F12) ကို နှိပ်ပါ။ ဒါမှမဟုတ် Mac ကိုသုံးနေတယ်ဆိုရင် `key:Cmd+Opt+J` (Cmd+Opt+J) ကို တွဲနှိပ်ပါ။

<!-- The developer tools will open on the Console tab by default. -->
အဲ့ဒါဆိုရင် developer tools ပွင့်လာမှာ ဖြစ်ပြီး Console tab ကို ပုံသေ အဖြစ် ရွေးပေးထားပါလိမ့်မယ်။

<!-- It looks somewhat like this: -->
ဒီလိုပုံစံမျိုး :

![chrome](chrome.png)

<!-- The exact look of developer tools depends on your version of Chrome. It changes from time to time but should be similar. -->
Developer tools တွေရဲ့ ပုံစံကတော့ ကိုယ်သုံးနေတဲ့ brower version ပေါ်မူတည်ပြီး ပြောင်းနိုင်ပါတယ်။ ဒါပေမယ့် သိပ်တော့ မကွာပါဘူး။

<!-- - Here we can see the red-colored error message. In this case, the script contains an unknown "lalala" command. -->
- ဒီမှာဆိုရင် ကျွန်တော်တို့ အနီရောင် စာတန်းနဲ့ error message ကို တွေရမှာ ဖြစ်ပါတယ်။ Error ကတော့ JavaScript မှာ "lalala" ဆိုတဲ့ command မရှိလို့ဖြစ်တဲ့ error ပါ။
<!-- - On the right, there is a clickable link to the source `bug.html:12` with the line number where the error has occurred. -->
- သူရဲ့ နောက်ဆုံးမှာ နှိပ်လို့ရတဲ့ link တစ်ခုအနေနဲ့ `bug.html:12` ကို ပြထားမှာ ဖြစ်ပြီး အဲ့နေရာက ဒီ error ကို ဖြစ်စေတဲ့ နေရာပါပဲ။

<!-- Below the error message, there is a blue `>` symbol. It marks a "command line" where we can type JavaScript commands. Press `key:Enter` to run them. -->
အဲ့ဒီ error message တွေရဲ အောက်ဆုံးမှာ အပြာရောင် `>` ကိုတွေ့ရမှာ ဖြစ်ပါတယ်။ ထို သင်္ကေတ ဟာ JavaScript commands တွေ ရိုက်လို့ရတဲ့ နေရာဖြစ်ပြီး `key:Enter` ကို နှိပ်ပြီး run နိုင်ပါတယ်။

<!-- Now we can see errors, and that's enough for a start. We'll come back to developer tools later and cover debugging more in-depth in the chapter <info:debugging-chrome>. -->
အခုမြင်ရတဲ့ error information တွေဟာ စစခြင်း လေ့လာသူတွေအတွက်လုံလောက်ပါတယ်။ ဒါပေမယ် နောက်ပိုင်း အခန်း <info:debugging-chrome> မှာ ကျွန်တော်တို့ debugging ကို အတွင်းကျကျ ထပ်ပြီး လေ့လာကျအောင်ပါ။

```smart header="Multi-line input"
<!-- Usually, when we put a line of code into the console, and then press `key:Enter`, it executes. -->
ပုံမှန်အားဖြင့် ကျွန်တော်တို့ console မှာ command တစ်ကြောင်းကို run ချင်ရင် တစ်ကြောင်းရေးပြီးတာနဲ့ `key:Enter` ကို နှိပ်ပြီး run ပါတယ်။

တကယ်လို့ တစ်ကြောင်းထပ် ပိုတဲ့ command တွေကို run ချင်တယ်ဆိုရင် `key:Shift+Enter` ကို သုံးပြီး တော့ run လို့ရပါတယ်။ အဲ့ဒီနည်းနဲ့ JavaScript Code အရှည်တွေကို run လို့ရပါတယ်။

<!-- To insert multiple lines, press `key:Shift+Enter`. This way one can enter long fragments of JavaScript code. -->
```

## Firefox, Edge, and others

<!-- Most other browsers use `key:F12` to open developer tools. -->
Browsers တော်တော်များများက `key:F12` ကို သုံးပြီးတော့ developer tools ကို ဖွင့်လို့ရပါတယ်။

<!-- The look & feel of them is quite similar. Once you know how to use one of these tools (you can start with Chrome), you can easily switch to another. -->
သူတို့ရဲ့ ပုံစံတွေ တွေက တော်တော် ဆင်တူပါတယ်။ ဒါကြောင့် တစ်ခုကို နားလည်သွားပြီဆိုရင် နောက်တစ်ခုကို အလွယ်လေး သုံးလို့ရပါတယ်။ (Chrome ကို စသုံးကြည့်ပါ)

## Safari

<!-- Safari (Mac browser, not supported by Windows/Linux) is a little bit special here. We need to enable the "Develop menu" first. -->
Safari (Mac browser, not supported by Windows/Linux) ကတော့ နည်နည်း ထူးဆန်းပါတယ်။ သူမှာ developer tool ကို သုံးဖို့ အတွက် "Develop menu" ကို အရင် ဆုံး enable လုပ်ဖို့လိုပါတယ်။

<!-- Open Preferences and go to the "Advanced" pane. There's a checkbox at the bottom: -->
Perferences ကို ဖွင့်ပါ။ ပြီးရင် "Advanced" ကို သွားပါ။ အဲ့စာမျက်နှာရဲ့ အောက်နားမှာ checkbox တစ်ခုရှိပါတယ်။

![safari](safari.png)

<!-- Now `key:Cmd+Opt+C` can toggle the console. Also, note that the new top menu item named "Develop" has appeared. It has many commands and options. -->
`key:Cmd+Opt+C` ကို သုံးပြီး enable​ လိုနိုင်ပါတယ်။ ဒါအပြင် ထိပ်မှာ "Develop" ဆိုတဲ့ menu item တစ်ခုပေါ်လာမှာဖြစ်ပြီး တစ်ခြား commands တွေနဲ့ options တွေ ရှိပါတယ်။

<!-- ## Summary -->
## အနှစ်ချုပ်

<!-- - Developer tools allow us to see errors, run commands, examine variables, and much more. -->
- Developer tools တွေက နေတစ်ဆင့် ကျွန်တော်တို့ erros တွေ ၊ run command တွေ ၊ variable တန်ဖိုးတွေ နဲ့ တခြား ဟာတွေ အများကြီး လုပ်လို့ရပါတယ်။
<!-- - They can be opened with `key:F12` for most browsers on Windows. Chrome for Mac needs `key:Cmd+Opt+J`, Safari: `key:Cmd+Opt+C` (need to enable first). -->
- Windows browsers တွေမှာ များသော အားဖြင့် `key:F12` ကိုသုံးပြီး ဖွင့်နိုင်ပါတယ်။ Chrome for Mac needs `key:Cmd+Opt+J`, Safari: `key:Cmd+Opt+C` (need to enable first).

<!-- Now we have the environment ready. In the next section, we'll get down to JavaScript. -->
အခုဆိုရင် ကျွန်တော်တို့မှာ  JavaScript environment အဆင်သင့်ဖြစ်ပါပြီ ။ နောက် သင်ခန်းစာတွေမှာ JavaScript နဲ့ ပတ်သတ်ပြီး ပိုနက်နဲတဲ့ အရာတွေကို လေ့လာကျပါစို့
