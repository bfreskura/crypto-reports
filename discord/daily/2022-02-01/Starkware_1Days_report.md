# **Starkware** summary for **2022-01-31** - **2022-02-01**

<details>
<summary>

## **✨-starknet** - [38 new messages 📨](https://discord.com/channels/793094838509764618/853954510515208192)

</summary>

---

### ↩️ **Messages with most replies**

* [2 ↩️] *why are storage diffs posted in L1. couldnt you find the diff if you just knew the fuction inputs?* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/853954510515208192/937945533505499177)


---


### 🔝 **Topics and related messages**

1. **starknet, tokens, l1**

    alex_aRB --- *Where to get test tokens for myswap and jediswap* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/853954510515208192/938114311476351007)

    AlexGrek --- *Hello, where to get some test tokens?* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/853954510515208192/938081340933427260)

    odin free --- *Hey Sempai,  With the launch of the new version, we are currently experiencing massive demand. StarkNet's capacity is still locked and therefore it can take a long time for transactions to be processed. Once the training wheels are removed, transaction time will be massively reduced. Thank you for your enthusiasm to try StarkNet in these early days. It should now get better any day/week. Have a good day.* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/853954510515208192/938044033702453308)

2. **balance, felt, bytes**

    Richeza --- *Thank you! I will wait for more stability work, you have the great project* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/853954510515208192/938049588902891570)

    sulaiman --- *Thank you will let you know if I encounter any error* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/853954510515208192/938013890716000337)

    Ashitaka --- *the balance is a Uint256, which means a felt for the lowest bytes, and another felt for the highest bytes And your points will appear in ArgentX in a while, you just have to wait* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/853954510515208192/937833527410573362)

</details>

&nbsp;  

---

<details>
<summary>

## **🦅-cairo-lang-support** - [33 new messages 📨](https://discord.com/channels/793094838509764618/793094838987128843)

</summary>

---

### ↩️ **Messages with most replies**

* [2 ↩️] *(I hope I understood the question) For example: https://github.com/starkware-libs/cairo-lang/blob/master/src/starkware/starknet/core/os/transactions.cairo#L345 `global_state_changes` is a dict of `StateEntry` structs, which in turn contain a pointer to another dict (it would have worked the same if instead of `StateEntry` you'd have a pointer directly). It works as follows: you "guess" (using a hint) the value of the main dict, compute from it the new value of the pointer, and finally call `dict_update` which verifies the guess and performs the update. Note that due to the use of a hint you won't be able to use it as-is in StarkNet contracts (but I believe that it can be fixed by using `dict_read`, `dict_write`  and a default dict).* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128843/937790124761182309)


---


### 🔝 **Topics and related messages**

1. **assert, result, spiral**

    RoboTeddy --- *I suspect that as currently implemented it will always return `P-n`, but I'm not sure if they'll change it in a future version* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128843/937836077127979129)

    RoboTeddy --- *I haven't understood your problem carefully, but it's likely that the starknet testing library returns `-1` as `P-1`. those two values behave the same way, because e.g. `(3 + (-1)) % P == 2`, just like `(3 + (P - 1)) % P == 2`. so a couple of options — you could either specifically test for e.g. `assert l.result == (1, P-1)`, or you could write some kind of python test wrapper that returns `-1` instead of `P-1`.* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128843/937834308977193030)

    th0rgal --- *```         l = await contract.spiral(4, 0).call() >       assert l.result == (1, -1) E       assert spiral_return...6135872020480) == (1, -1) E         At index 1 diff: 3618502788666131213697322783095070105623107215331596699973092056135872020480 != -1 E         Use -v to get the full diff ```* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128843/937830515988373585)

2. **native, windows, native way**

    Dave_ --- *tried on m1 Mac, and ubuntu ARM VM's on said Mac, didn't work* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128843/938118723095629846)

    Dave_ --- *finally got the cairo environment setup* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128843/938118513254625360)

    LauriP --- *ah by 'native' I mean not native to Windows.* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128843/938000358981140511)

</details>

&nbsp;  

---

<details>
<summary>

## **☎-community-calls** - [31 new messages 📨](https://discord.com/channels/793094838509764618/912378208370950215)

</summary>

---

### 💌 **Most reacted messages**

1. *hey <@&836861133700202526> , don't forget our 7th community call today in 30mn! https://discord.com/events/793094838509764618/935902512622473307* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/912378208370950215/938056294584164443)

2. *For those who missed todays community call and don't want to wait for the release of the official recording, there's an unofficial one:* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/912378208370950215/938078486906683475)

3. *hi, ofc i know briq is a cool project. lets try! and pls check it 😎  Hey, thank you for your curiosity. Here are some things you can explore.   15 projects in production or test phase: https://twitter.com/odin_free/status/1479470476606980101?s=20  Argent X, the first StarkNet wallet, follow this link: https://twitter.com/0x6f6c6567/status/1468157947528159234?s=20  And this tutorial from Henri: https://discord.com/channels/793094838509764618/853954510515208192/917728614022266881  Have fun and let us know what you think* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/912378208370950215/938074258813382736)


---


### 🔝 **Topics and related messages**

1. **starknet, issue, tutorial**

    s0lness --- *This is due both to our poorly optimized contracts and the recent performance issues on StarkNet. We have an update coming up soon which solves this "briqs are loading" problem* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/912378208370950215/938074561038147594)

    Cyberviking.dao --- *I tried this, always tells me ..Please wait while briqs are loading... when minting* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/912378208370950215/938074090395295795)

    Cyberviking.dao --- *Great, thanks for your answer. By the way, since Starknet is still new, any projects already running on Starknet?* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/912378208370950215/938073267292504106)

2. **, great community organizing, todays community wait**

    abbaspuya --- *Is the audience given a poap to attend the community ?! Thanks* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/912378208370950215/938058496358875196)

    Henri-l | Starkware --- *hey <@&836861133700202526> , don't forget our 7th community call today in 30mn! https://discord.com/events/793094838509764618/935902512622473307* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/912378208370950215/938056294584164443)

    abbaspuya --- *Hello guys🙌, where and when will Community Call be held ?!* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/912378208370950215/938050315511558216)

</details>

&nbsp;  

---

## **🤗-dev-support** - [26 new messages 📨](https://discord.com/channels/793094838509764618/793094838987128844)
&nbsp;  

---

<details>
<summary>

## **📚-tutorials-support** - [20 new messages 📨](https://discord.com/channels/793094838509764618/932633376563802152)

</summary>

---

### ↩️ **Messages with most replies**

* [2 ↩️] *assert [ap] = [ap-1] * [ap-1] * [ap-1] mixes high level (assert) syntax, with low level register access (ap). Using ap directly in compound expressions is not well defined.* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/932633376563802152/937994105408061460)


---


### 🔝 **Topics and related messages**

1. **advance, advance ap, semicolon**

    ilya.lesokhin --- *let only gives a name to an expression it does not generate opcodes on its own so definitely does not increase ap.* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/932633376563802152/937996461315063858)

    ilya.lesokhin --- *[ap] = 3 does not advance ap.* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/932633376563802152/937993569631879178)

    kmd --- *But, “[ap] = 3” only also advances ap?* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/932633376563802152/937992997969203200)

2. **ap ap ap, assert, assert ap**

    ilya.lesokhin --- *Maybe not well defined wasn't the best way of phrasing it. The generated code is deterministic.  but assert [ap] = [ap-1] * [ap-1] * [ap-1] Asks the compiler  to assign a value to [ap] and the compiler also uses [ap] as temporary storage for the computation of the  [ap-1] * [ap-1] * [ap-1] compound expression. So you get an error.* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/932633376563802152/937998434777038859)

    kmd --- *So, I need to count `ap` implicitly increated by `assert` instruction? like,  `assert [ap+8] = x3 + x2 + x1 + 67` worked.* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/932633376563802152/937997150053359676)

    kmd --- *Thanks you! I asked this question because I'm trying to solve polynomial exercise in 5 instructions. https://starknet.io/docs/how_cairo_works/cairo_intro.html#a-simple-cairo-program-exercise code below won't work. ``` func main():     [ap] = 100; ap++      let x = [ap-1]     let x1 = x * 45     let x2 = 23 * x * x     let x3 = x * x * x     assert [ap] = x3 + x2 + x1 + 67      ret end ``` This is an error I got. ``` An ASSERT_EQ instruction failed: 10000 != 1234567.     assert [ap] = x3 + x2 + x1 + 67     ^*****************************^ ``` Maybe, `let` doesn't increment `ap`?* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/932633376563802152/937996085425745920)

</details>

&nbsp;  

---

## **⚒-dev-tools** - [7 new messages 📨](https://discord.com/channels/793094838509764618/894580545311359026)
&nbsp;  

---

## **🌐-argent-extension** - [7 new messages 📨](https://discord.com/channels/793094838509764618/908663762150645770)
&nbsp;  

---

<details>
<summary>

## **🏗-starknet-js** - [7 new messages 📨](https://discord.com/channels/793094838509764618/927918707613786162)

</summary>

---

### ↩️ **Messages with most replies**

* [2 ↩️] *Hey guys, I need some help. I got really frustrated after a few days of trying. I already report a bug on github and I made another post here. The problem is using starknet js to interact with cairo contracts that have a Uint256 parameter.   I created a repo on github with a simple ERC20 deployment script that fail. https://github.com/FilipLaurentiu/starknet_js_interaction Argent X use the starknet js library to interact with ERC20 tokens and I thought that maybe I use it wrong on any other problem... I take a look into the argent-x repo and it seems to be the same. Please help 😦* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/927918707613786162/937971314105384991)


---
</details>

&nbsp;  

---

## **🍯-русский** - [6 new messages 📨](https://discord.com/channels/793094838509764618/895711335801819187)
&nbsp;  

---

## **🕗-gm-gn** - [3 new messages 📨](https://discord.com/channels/793094838509764618/884341617992024105)
&nbsp;  

---

## **🐠-random** - [3 new messages 📨](https://discord.com/channels/793094838509764618/893514287887294526)
&nbsp;  

---

## **🍚-فارسی** - [3 new messages 📨](https://discord.com/channels/793094838509764618/912406778204012564)
&nbsp;  

---

## **🌮-español** - [2 new messages 📨](https://discord.com/channels/793094838509764618/899344999509033011)
&nbsp;  

---

## **🥙-türkçe** - [1 new message 📨](https://discord.com/channels/793094838509764618/899302454020177970)
&nbsp;  

---

## **🔭-voyager-block-explorer** - [1 new message 📨](https://discord.com/channels/793094838509764618/912410047236149298)
&nbsp;  

---

## **-bahasa-indonesia** - [1 new message 📨](https://discord.com/channels/793094838509764618/930526767259717712)
&nbsp;  

---

## **-हिन्दी** - [1 new message 📨](https://discord.com/channels/793094838509764618/930528209882185748)
&nbsp;  

---

