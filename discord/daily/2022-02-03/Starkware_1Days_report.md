# **Starkware** summary for **2022-02-02** - **2022-02-03**

<details>
<summary>

## **✨-starknet** - [54 new messages 📨](https://discord.com/channels/793094838509764618/853954510515208192)

</summary>

---


### 🔝 **Topics and related messages**

1. **l2, eth, bridge**

    Solo --- *Why would they need a bridge?couldnt they just alsohave a L2 wallet and send L2 to L2.* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/853954510515208192/938740977806503946)

    RoboTeddy --- *At the end of the day, even an L2 bridge will have a contract on the ethereum side that holds a bunch of ether that was sent over the bridge. If that contract had a critical bug, funds could be taken from it.* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/853954510515208192/938557771031388190)

    RoboTeddy --- *Yes. (But L2s aren't vulnerable at all to bridge governance attacks.)* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/853954510515208192/938557486355591230)

2. **starknet, nitro, using**

    odin free --- *StarkEx is a standalone system for exchanges that uses the STARK proof system in order to provide scalability for the exchanges using it.  See https://starkware.co/product/starkex/  StarkNet is a general-purpose system, where you can write and deploy your own contracts, interact with other contracts, and so on, just like Ethereum. See https://starkware.co/product/starknet/  Have a good day Oli* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/853954510515208192/938794996411269180)

    Stortal --- *oh ok, I was wondering how I can find out fees on ImmutableX since it uses starknet* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/853954510515208192/938794591027621918)

    Stortal --- *Isn't there a simple page like: https://l2fees.info/ that includes starknet fees?* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/853954510515208192/938793637440016474)

3. **wormhole hack, hack, wormhole**

    RoboTeddy --- *(Might even be possible to formally prove certain security aspects.)* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/853954510515208192/938558167451840563)

    decendegegn --- *so it is safe they cannot "steal" anything like wormhole hack?* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/853954510515208192/938557467900670013)

    decendegegn --- *like an exploit possible of wormhole hack* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/853954510515208192/938557164442746961)

</details>

&nbsp;  

---

<details>
<summary>

## **🤗-dev-support** - [42 new messages 📨](https://discord.com/channels/793094838509764618/793094838987128844)

</summary>

---

### 💌 **Most reacted messages**

1. *any feedback / feature requests are very welcome* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128844/938748635137605642)

2. *Hey there! We plan to implement perlin noise in cairo (as part of a starknet smartcontract). Do you have any suggestions, especially about handling floats (we have only handled integers so far)?* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128844/938579169896439818)

3. *I don't understand Cairo integer maths* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128844/938531615309725746)


---

### ↩️ **Messages with most replies**

* [2 ↩️] *is it correct to assume having more memory holes leads to less memory efficiency which leads to higher contract deployment costs? are there some known best practices to reduce memory holes?* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128844/938644210830168074)


---


### 🔝 **Topics and related messages**

1. **function, mod, integer**

    exp.table --- *In particular, if you try the 7 / 3 div with the appropiate function, it returns `5380300354831952554` which has to be divided by `2**61` and it yields .... 2.333333 😉* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128844/938545739787821067)

    Martin Krug --- *Sorry, I was meaning 3 * 4 = 4 (12 - 8); 3 * 5 = 7 (15 - 8)* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128844/938533538976911370)

    Martin Krug --- *When you use a very large mod, like P, you will find a very large number, probably, for simple divisions. It's how cyclic groups work.* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128844/938533304582418503)

2. **account, felt, version**

    Da Blob StarkIt --- *thanks <@!260514830006485002> i'll take a look* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128844/938780282843177040)

    mierzwik --- *please note it is a passive endpoint, we are working on active public/subscribe version but it will take a little bit more time* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128844/938748894051975269)

    guiltygyoza --- *<@117430577891639300> may have thought about this / gave it a shot* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128844/938614136370262016)

</details>

&nbsp;  

---

<details>
<summary>

## **🦅-cairo-lang-support** - [24 new messages 📨](https://discord.com/channels/793094838509764618/793094838987128843)

</summary>

---


### 🔝 **Topics and related messages**

1. **let, cairo, local**

    Monkstep --- *Does Cairo support empty interfaces as parameters ( `any` / `interface{}` in most languages)? Was something Solidity seems to have a gap in https://www.reddit.com/r/solidity/comments/sj8ajc/inheritance_and_overriding_functions_with/, and was just wondering if it's possible in Cairo. Thanks!* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128843/938832278824562709)

    Oleh --- *Maybe there are another way to implement something like that I have been thinking about L1<>L2 messaging Contratc.sol will create contracts, while Contract.cairo will do all job* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128843/938695755936440340)

    RoboTeddy --- *if you'd like one contract to deploy another contract, that isn't possible yet but will be in a future release of starknet/cairo-lang* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128843/938695330701115402)

2. **storage slot, felts, 251**

    codemedian --- *not that I'd ever hit that limit either way, but still curious 🙂* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128843/938569149632888852)

    codemedian --- *ah, right, that makes sense. so the key gets hashed to the where and it's considered "empty" if the contents are all zeroes* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128843/938563661864251454)

    RoboTeddy --- *I think of the key as "part of" the storage slot. the key gets hashed down to an index which identifies the storage slot. each storage slot requires ~2 felts worth of space in L1 calldata (because have to record both the slot index and the slot value to L1 calldata)* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128843/938563433043984475)

</details>

&nbsp;  

---

## **🥙-türkçe** - [8 new messages 📨](https://discord.com/channels/793094838509764618/899302454020177970)
&nbsp;  

---

## **🌐-argent-extension** - [8 new messages 📨](https://discord.com/channels/793094838509764618/908663762150645770)
&nbsp;  

---

## **🍯-русский** - [6 new messages 📨](https://discord.com/channels/793094838509764618/895711335801819187)
&nbsp;  

---

## **🕗-gm-gn** - [3 new messages 📨](https://discord.com/channels/793094838509764618/884341617992024105)
&nbsp;  

---

<details>
<summary>

## **🐠-random** - [3 new messages 📨](https://discord.com/channels/793094838509764618/893514287887294526)

</summary>

---

### ↩️ **Messages with most replies**

* [2 ↩️] *My question is why Ethereum plans to use SNARKs particularly in stateless clients? why not STARKs? when we know that STARKs are more scalable, less verification time and post quantum secure too.* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/893514287887294526/938687746069901342)


---
</details>

&nbsp;  

---

## **🐞-starknet-bug-report** - [3 new messages 📨](https://discord.com/channels/793094838509764618/920304241376104488)
&nbsp;  

---

## **🥐-français** - [2 new messages 📨](https://discord.com/channels/793094838509764618/802928244139360306)
&nbsp;  

---

## **🥨-deutsch** - [2 new messages 📨](https://discord.com/channels/793094838509764618/915844624176803882)
&nbsp;  

---

## **🗓-introduce-your-project** - [1 new message 📨](https://discord.com/channels/793094838509764618/892380563497947156)
&nbsp;  

---

## **🥗-עברית** - [1 new message 📨](https://discord.com/channels/793094838509764618/898211189446836284)
&nbsp;  

---

## **🌮-español** - [1 new message 📨](https://discord.com/channels/793094838509764618/899344999509033011)
&nbsp;  

---

## **☎-community-calls** - [1 new message 📨](https://discord.com/channels/793094838509764618/912378208370950215)
&nbsp;  

---

## **🐍-starknet-py** - [1 new message 📨](https://discord.com/channels/793094838509764618/928219862327754812)
&nbsp;  

---

## **warp-transpiler** - [1 new message 📨](https://discord.com/channels/793094838509764618/935889632124616765)
&nbsp;  

---

