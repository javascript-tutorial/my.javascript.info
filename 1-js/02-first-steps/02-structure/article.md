# Code ဖွဲ့စည်းပုံ

<!-- The first thing we'll study is the building blocks of code. -->

ပထမဆုံး ကျွန်တော်တို့ code အပိုင်းတွေ ဖွဲစည်းတည်ဆောက်ပုံကို လေ့လာပါမယ်။

## Statements

<!-- Statements are syntax constructs and commands that perform actions. -->

Statement တွေဆိုမှာ စာကြောင်း တည်ဆောက်ပုံ နဲ့ အလုပ်လုပ် နိုင်တဲ့ commands တွေ ပါဝင်ပါတယ်။

<!-- We've already seen a statement, `alert('Hello, world!')`, which shows the message "Hello, world!". -->

ကျွန်တော်တို့ statement တွေကို တွေ့ဖူးပြီးပါပြီ ။ ဥပမာ အားဖြင့် `alert('Hello, world!')` ဆိုတဲ့ statement က "Hello, world!" ဆိုတဲ့ message ကို ပြပေးပါလိမ့်မယ်။

<!-- We can have as many statements in our code as we want. Statements can be separated with a semicolon. -->

ကျွန်တော်တို့ရဲ့ code ထဲမှာ statement တွေ ကြိုက်သလောက် ရေးလို့ရပြီး statements တစ်ခုချင်းစီကို semicolon(;) နဲ့ ခွဲခြားပေးပါတယ်။

<!-- For example, here we split "Hello World" into two alerts: -->

ဥပမာ "Hello World" ဆိုတဲ့ alert ၂ ခုကို ခွဲပြီး ရေးနိုင်ပါတယ်။

```js run no-beautify
alert("Hello");
alert("World");
```

<!-- Usually, statements are written on separate lines to make the code more readable: -->

ပုံမှန်အားဖြင့်တော့ statements တွေကို ဖတ်ရတာ လွယ်အောင် တစ်ကြောင်းချင်။စီ ရေးပါတယ်။

```js run no-beautify
alert("Hello");
alert("World");
```

## Semicolons [#semicolon]

<!-- A semicolon may be omitted in most cases when a line break exists. -->

တကယ်လို့ စာကြောင်းအဆုံးမှာ ဆိုရင်တော့ semicolon ကို ဖြုတ်ထားခဲ့လို့ရပါတယ်။

<!-- This would also work: -->

ဥပမာ ဒီလိုပုံစံ မျိုးဆိုလည်း အလုပ်လုပ်ပါတယ်။

```js run no-beautify
alert("Hello");
alert("World");
```

<!-- Here, JavaScript interprets the line break as an "implicit" semicolon. This is called an [automatic semicolon insertion](https://tc39.github.io/ecma262/#sec-automatic-semicolon-insertion). -->

ဒီလိုပုံစံမျိုးရေးလည်း ဘာလို့ အလုပ်လုပ်လည်းဆိုတော့ JavaScript က စာကြောင်းအဆုံး (line break) တွေကို statement အဆုံးလို့ သတ်မှတ်ပေးလို့ဖြစ်ပါတယ်။ အဲ့ဒါကို [automatic semicolon insertion](https://tc39.github.io/ecma262/#sec-automatic-semicolon-insertion) (အလိုအလျာက် semicolon ထည့်ပေးခြင်း) လို့ခေါ်ပါတယ်။

<!-- **In most cases, a newline implies a semicolon. But "in most cases" does not mean "always"!** -->

**များသောအားဖြင့် စာကြောင်း နောက်တစ်ကြောင်းကို semicolon တစ်ခုလို့ သတ်မှတ်ပေးပါတယ်။ ဒါပေမယ့် "များသောအားဖြင့်" ဆိုတာက အမြဲတမ်းလို့ မဆိုလိုပါဘူး။**

<!-- There are cases when a newline does not mean a semicolon. For example: -->

စာကြောင်း နောက်တစ်ကြောင်းကို semicolon လို့ မသတ်မှတ်ပေးတဲ့ ဟာတွေလည်း ရှိပါတယ်။ ဥပမာ

```js run no-beautify
alert(3 + 1 + 2);
```

<!-- The code outputs `6` because JavaScript does not insert semicolons here. It is intuitively obvious that if the line ends with a plus `"+"`, then it is an "incomplete expression", so a semicolon there would be incorrect. And in this case, that works as intended. -->

အပေါ်က code ရဲ့ output က `6` လို့ထွက်ပါတယ်။ ဘာကြောင့်လည်းဆိုတော့ JavaScript က စာကြောင်းအဆုံးမှာ semicolon မထည့်ပေးလို့ဖြစ်ပါတယ်။ JavaScript က စာကြောင်းအဆုံးမှာ `"+"` ပါရင် အလိုအလျောက် "မပြည့်စုံ တဲ့ စာကြောင်း" လို့ သိပြီး semicolon မထည့်ပေးလို့ဖြစ်ပါတယ်။ ဒါကြောင့် အဲ့ နေရာမှာ semicolon ထည့်ပေးလိုက်ရင် မှားမှာပါ။

<!-- **But there are situations where JavaScript "fails" to assume a semicolon where it is really needed.** -->

**ဒါပေမယ့် တစ်ခါတစ်လေကျ JavaScript က semicolon လိုအပ်တဲ့နေရာကို ထည့်ပေးဖို့ ပျက်ကွက်တာမျိုးတွေလည်း ရှိပါတယ်**

<!-- Errors which occur in such cases are quite hard to find and fix. -->

အဲ့လို အခြေအနေ errors တွေကတော့ ဖြစ်တဲ့နေရာကို ရှာပြီး ပြင်ဖို့ ခက်တက်ပါတယ်။

<!-- ````smart header="An example of an error" -->

````smart header="ဥပမာ"
<!-- If you're curious to see a concrete example of such an error, check this code out: -->
တကယ်လို့ အဲ့လို error ကို ဥပမာ အနေနဲ့ သိချင်တယ်ဆိုရင် အောက်က code ကို ကြည့်ပါ။

```js run
alert("Hello");

[1, 2].forEach(alert);
```

<!-- No need to think about the meaning of the brackets `[]` and `forEach` yet. We'll study them later. For now, just remember the result of running the code: it shows `Hello`, then `1`, then `2`. -->
`[]` နဲ့ `forEach` တွေကို ဖယ်ပြီး ကြည့်ပါ။ အဲ့ အကြောင်းတွေကို နောက်ကျ ထပ်ပြီး လေ့လာပါမယ်။ အခု လောလောဆယ် သိထားရမှာက အပေါ်က code ကို run လိုက်ရင် `Hello` ပြီးရင် `1` ,`2` ဆိုပြီး alert ပြပါလိမ့်မယ်။

<!-- Now let's remove the semicolon after the `alert`: -->
အာဆို အပေါ် စာကြောင်းဖြစ်တဲ့ `alert` က semicolon ကို ဖယ်ကြည့်ရအောင်

```js run no-beautify
alert("Hello")

[1, 2].forEach(alert);
```

<!-- The difference compared to the code above is only one character: the semicolon at the end of the first line is gone. -->
အပေါ်က code ၂ ခုကို နှိုင်းယှဉ်ကြည့်ရင် alert လိုင်းက semicolon ပါတာ မပါတာ တစ်ခုပဲ ကွာတာ တွေ့ပါလိမ့်မယ်။

<!-- If we run this code, only the first `Hello` shows (and there's an error, you may need to open the console to see it). There are no numbers any more. -->
တကယ်လို့ ကျွန်တော်တို့ အဲ့ code ကိုသာ run လိုက်ရင် `Hello` ဆိုတဲ့ alert ကို ပဲ ပြပေးပါလိမ့်မယ်။ ပြီးရင် developer tools ကို ဖွင့်လိုက်ရင် error တစ်ခု တွေ့ပါလိမ့်မယ်။ 1 နဲ့ 2 ဆိုတဲ့ alert တွေ ထွက်မှာ မဟုတ်ပါဘူး။

<!-- That's because JavaScript does not assume a semicolon before square brackets `[...]`. So, the code in the last example is treated as a single statement. -->
အဲ့ဒါက ဘာကြောင့်လည်းဆိုတော့ JavaScript က `[...]` မတိုင်ခင် semicolon ရှိတယ်လို့ မယူဆလို့ ဖြစ်ပါတယ်။ဒါကြောင့် ဥပမာ ပေးထားတဲ့ code ကို စာကြောင်းတစ်ကြောင်းတည်း အဖြစ် ယူဆပါလိမ့်မယ်။

<!-- Here's how the engine sees it: -->
Engine က ဘယ်လို မြင်မလည်းဆိုတော့

```js run no-beautify
alert("Hello")[1, 2].forEach(alert);
```

<!-- Looks weird, right? Such merging in this case is just wrong. We need to put a semicolon after `alert` for the code to work correctly. -->
ကြည့်ရတာ ထူးဆန်းတယ်မလား? အဲ့လိုမျိုး တစ်ကြောင်းတည်းလို့ ယူဆတာက မှားယွင်းပါတယ်။ ဒါကြောင့် ကျွန်တော်တို့ `alert` code ပြီးတာနဲ့ semicolon ထည့်ပေးမှာသာ မှန်မှာပါ။

<!-- This can happen in other situations also. -->
အဲ့လို ဖြစ်တာက တစ်ခြားပုံစံ အခြေအနေတွေမှာလည်း ဖြစ်နိုင်ပါတယ်။
````

<!-- We recommend putting semicolons between statements even if they are separated by newlines. This rule is widely adopted by the community. Let's note once again -- *it is possible* to leave out semicolons most of the time. But it's safer -- especially for a beginner -- to use them. -->

ဒါကြောင့် နောက်တစ်ကြောင်းဆင်းပြီး ရေးမယ် ဆိုတာထပ် စာကြောင်းဆုံးတိုင်းမှာ semicolon ကို ထည့်ဖို့ ကျွန်တော်တို့ recommend ပေးပါတယ်။ JS community ကလည်း အဲ့လို ရေးပုံကို လက်ခံကျင်သုံးပါတယ်။ ဒါကြောင့် နောက်တစ်ခေါက် မှတ်ထားရမှာက semicolon ကို _များသောအားဖြင့်_ ဖြုတ်ထားခဲ့နိုင်ပါတယ်။ ဒါပေမယ့် -- အထူးသဖြင့် အခုမှ စလေ့လာမယ့်သူ -- တွေအတွက်တော့ semicolon ကို စာကြောင်းဆုံးတိုင်းထည့်သင့်ပါတယ်။

<!-- ## Comments [#code-comments] -->

## Comments [#code-comments]

<!-- As time goes on, programs become more and more complex. It becomes necessary to add *comments* which describe what the code does and why. -->

Comments can be put into any place of a script. They don't affect its execution because the engine simply ignores them.

**One-line comments start with two forward slash characters `//`.**

The rest of the line is a comment. It may occupy a full line of its own or follow a statement.

Like here:

```js run
// This comment occupies a line of its own
alert("Hello");

alert("World"); // This comment follows the statement
```

**Multiline comments start with a forward slash and an asterisk <code>/\*</code> and end with an asterisk and a forward slash <code>\*/</code>.**

Like this:

```js run
/* An example with two messages.
This is a multiline comment.
*/
alert("Hello");
alert("World");
```

The content of comments is ignored, so if we put code inside <code>/\* ... \*/</code>, it won't execute.

Sometimes it can be handy to temporarily disable a part of code:

```js run
/* Commenting out the code
alert('Hello');
*/
alert("World");
```

```smart header="Use hotkeys!"
In most editors, a line of code can be commented out by pressing the `key:Ctrl+/` hotkey for a single-line comment and something like `key:Ctrl+Shift+/` -- for multiline comments (select a piece of code and press the hotkey). For Mac, try `key:Cmd` instead of `key:Ctrl` and `key:Option` instead of `key:Shift`.
```

````warn header="Nested comments are not supported!"
There may not be `/*...*/` inside another `/*...*/`.

Such code will die with an error:

```js run no-beautify
/*
  /* nested comment ?!? */
*/
alert( 'World' );
```
````

Please, don't hesitate to comment your code.

Comments increase the overall code footprint, but that's not a problem at all. There are many tools which minify code before publishing to a production server. They remove comments, so they don't appear in the working scripts. Therefore, comments do not have negative effects on production at all.

Later in the tutorial there will be a chapter <info:code-quality> that also explains how to write better comments.
