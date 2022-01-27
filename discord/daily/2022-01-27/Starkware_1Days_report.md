# **Starkware** summary for **2022-01-26** - **2022-01-27**

<details>
<summary>

## **🦅-cairo-lang-support** - [41 new messages 📨](https://discord.com/channels/793094838509764618/793094838987128843)

</summary>

---

### 💌 **Most reacted messages**

1. *No but we need a Package Manager! Could someone do a Crate like solution?* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128843/935960879067959326)


---

### ↩️ **Messages with most replies**

* [2 ↩️] *in cairo you only have values in the range [0,p-1], integers in the range [(p-1)/2,p-1] are "treated as" negative.  to use the number properly in python code you can use the as_int helper, example; https://github.com/starkware-libs/cairo-lang/blob/master/src/starkware/cairo/common/math.cairo#L298* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128843/936284630695411862)


---


### 🔝 **Topics and related messages**

1. **rust, pretty, think**

    Verde --- *I'd love to work in a project like that, I want to work on my Rust* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128843/936235709260517466)

    milan --- *fwiw, I welcome the move to a more Rusty environment, my thesis is that Rust is eating blockchain dev, it's popping up everywhere, Rust's adoption among blockchain and smart contract engineers will only grow, so it's a reasonable choice* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128843/936166675752042548)

    martriay --- *the target should be existing smart contract devs* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128843/936141336590032927)

2. **felt, value, distance**

    wraitii --- *I'm not certain it's much better than checking for 0-valued felt, but it works if you want to store arbitrary-length data neatly* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128843/936312470920912916)

    wraitii --- *So you can just store 31 characters, then a 0/1 to mark the end of the string or not, and it's completely transparent as an array of felt* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128843/936311491534151750)

    wraitii --- *I've made a 'long string' system by storing a 0 / 1 in the LSB* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128843/936311244657393815)

3. **legal, computation, positions**

    ilya.lesokhin --- *To prove a Cairo run the memory need to be continuous, with no gaps between the addresses. But making the memory continuous when you don't know the size of each segment is difficult. Our solution is to allow the runner to use (segment number, segment_offset) pairs rather than the field elements for addresses. Once the run is complete we know the sizes of the segments, we assign an absolution address (a field element) to each segment and replace every (segment number, segment_offset) pair with a field element to create a provable run. https://github.com/starkware-libs/cairo-lang/blob/64a7f6aed9757d3d8d6c28bd972df73272b0cb0a/src/starkware/cairo/lang/vm/cairo_runner.py#L328* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128843/936161738330624040)

    FeedTheFed | StarkWare --- *hhmmm which computation? verification if a move is legal? I don't think you should go over all legal moves, but just check that a given move was legal (if you're writing Cairo rather than a StarkNet contract then you have hints available, so you can get a hint if e.g. you're in check and what piece is causing it, and then verify it in Cairo). Other than checks you just need to know that the position the piece moved to is empty, and that the path was clear (e.g. if it's a rook move then I have at most 6 positions that I need to verify are empty).* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128843/936001562759790622)

    FeedTheFed | StarkWare --- *IIUC the vm first executes the program without outputs (just collects them), and then decides in retrospect the start location of output_ptr (and also the end since it collected all the intermediate values sent to the output).  Re halting condition, I think that in the playground the vm just runs until pc reaches a certain address as you suggested (something along the lines of https://github.com/starkware-libs/cairo-lang/blob/64a7f6aed9757d3d8d6c28bd972df73272b0cb0a/src/starkware/cairo/lang/vm/cairo_runner.py#L278) When actually proving the execution of Cairo programs the start_pc, end_pc, and #steps are part of the proven statement (definition 2 in the paper).  tagging <@!825258293266087937> who will know more* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128843/936000464493883412)

</details>

&nbsp;  

---

<details>
<summary>

## **✨-starknet** - [34 new messages 📨](https://discord.com/channels/793094838509764618/853954510515208192)

</summary>

---

### ↩️ **Messages with most replies**

* [2 ↩️] *What are the best tutorials for deploying a contract to Starknet Alpha?* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/853954510515208192/936029704853532704)


---


### 🔝 **Topics and related messages**

1. **starknet, argent, cairo**

    odin free --- *Do you feel like hunting down information about StarkNet is a constant game of “Where’s Waldo?” If so, this article by  <@!317704806204571659> is of great help:   StarkNet and the future of Ethereum scaling With rising Ethereum gas fees, a hero emerges... https://twitter.com/odin_free/status/1486727010403553283* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/853954510515208192/936287072447246376)

    ameya --- *Also, could anyone guide me to resources about NFTs on StarkNet?* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/853954510515208192/936283317962178570)

    odin free --- *Hey anon, good point. With the launch of the new version, we are currently experiencing massive demand. StarkNet's capacity is still locked and therefore it can take a long time for transactions to be processed. Once the training wheels are removed, transaction time will be massively reduced. Thank you for your enthusiasm to try StarkNet in these early days. It should now get better any day/week. Have a good day.* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/853954510515208192/936235409158053888)

2. **twitter, maybe, job**

    ameya --- *Awesome! Yes I've gone through these. Something a little more technical maybe? Or should I just explore the docs and see where it goes from there?* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/853954510515208192/936285353462083594)

    ameya --- *Please do🙏! I have very limited reach on Twitter My handle is:@0xameya* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/853954510515208192/936279128968159312)

    odin free --- *great read ser! did you share it on twitter?* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/853954510515208192/936273561792966726)

</details>

&nbsp;  

---

## **🤗-dev-support** - [17 new messages 📨](https://discord.com/channels/793094838509764618/793094838987128844)
&nbsp;  

---

<details>
<summary>

## **📚-tutorials-support** - [16 new messages 📨](https://discord.com/channels/793094838509764618/932633376563802152)

</summary>

---

### ↩️ **Messages with most replies**

* [2 ↩️] *I tried what you suggested and user_counters returns 0* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/932633376563802152/936114362656100423)

* [2 ↩️] *I understand that I need to manipulate the values but what im asking is: where do i enter all these things in? In Voyager? In Github? I dont understand where I actually get to manipulate and change the code.... for example on the read tab of voyager ex.3 it only gives me 2 opportunities to "write" anything at all....and that is only in boxes 5 & 6 in which i'm just typing in my CA. Like, WHERE am I able to "manipulate the code or actually "execute" the tasks?* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/932633376563802152/936098905920258088)


---
</details>

&nbsp;  

---

## **🍯-русский** - [9 new messages 📨](https://discord.com/channels/793094838509764618/895711335801819187)
&nbsp;  

---

<details>
<summary>

## **🌐-argent-extension** - [6 new messages 📨](https://discord.com/channels/793094838509764618/908663762150645770)

</summary>

---

### 💌 **Most reacted messages**

1. *Multicalls are coming to Argent X https://github.com/argentlabs/argent-contracts-starknet/pull/26. Let me know what you think <@!430806303212961803>* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/908663762150645770/936204664859414539)


---
</details>

&nbsp;  

---

## **👷-hardhat-plugin** - [5 new messages 📨](https://discord.com/channels/793094838509764618/912735106899275856)
&nbsp;  

---

<details>
<summary>

## **☎-community-calls** - [4 new messages 📨](https://discord.com/channels/793094838509764618/912378208370950215)

</summary>

---

### ↩️ **Messages with most replies**

* [2 ↩️] *How about Google Meet? I think it's better than Zoom for the video chatting. https://workspaceupdates.googleblog.com/2021/11/host-meetings-with-500-participants.html#:~:text=Google%20Workspace%20Updates%3A%20Host%20Google%20Meet%20meetings%20with%20up%20to%20500%20participants* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/912378208370950215/936074492764094575)


---
</details>

&nbsp;  

---

## **🐍-starknet-py** - [4 new messages 📨](https://discord.com/channels/793094838509764618/928219862327754812)
&nbsp;  

---

## **🕗-gm-gn** - [3 new messages 📨](https://discord.com/channels/793094838509764618/884341617992024105)
&nbsp;  

---

## **🍚-فارسی** - [3 new messages 📨](https://discord.com/channels/793094838509764618/912406778204012564)
&nbsp;  

---

<details>
<summary>

## **🏗-starknet-js** - [3 new messages 📨](https://discord.com/channels/793094838509764618/927918707613786162)

</summary>

---

### ↩️ **Messages with most replies**

* [2 ↩️] *we want to use the new 'blockNumber=pending' param when calling call_contract. the API for starknet.provider.callContract() accepts an optional integer for 'blockId' but 'blockNumber' is not available. Am I missing something, or is this feature not present yet?* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/927918707613786162/936247872326881291)


---
</details>

&nbsp;  

---

## **🍛-ไทย** - [2 new messages 📨](https://discord.com/channels/793094838509764618/903336291645661204)
&nbsp;  

---

## **🔭-voyager-block-explorer** - [2 new messages 📨](https://discord.com/channels/793094838509764618/912410047236149298)
&nbsp;  

---

## **🥐-français** - [1 new message 📨](https://discord.com/channels/793094838509764618/802928244139360306)
&nbsp;  

---

## **🥮-中文** - [1 new message 📨](https://discord.com/channels/793094838509764618/893106432046690324)
&nbsp;  

---

## **👷-community-jobs** - [1 new message 📨](https://discord.com/channels/793094838509764618/898210860030386178)
&nbsp;  

---

## **🍱-日本語** - [1 new message 📨](https://discord.com/channels/793094838509764618/899298454201835530)
&nbsp;  

---

## **☕-tiếng-việt** - [1 new message 📨](https://discord.com/channels/793094838509764618/910608609803653140)
&nbsp;  

---

## **🐞-starknet-bug-report** - [1 new message 📨](https://discord.com/channels/793094838509764618/920304241376104488)
&nbsp;  

---

