# **Starkware** summary for **2022-02-05** - **2022-02-06**

<details>
<summary>

## **🦅-cairo-lang-support** - [44 new messages 📨](https://discord.com/channels/793094838509764618/793094838987128843)

</summary>

---


### 🔝 **Topics and related messages**

1. **cairo, contracts, felt**

    th0rgal --- *So we use local when we lost the value with ap (but alloc_local can do it for us) And we use tempvar when we have multiple possibilities and we want them to be at the same location in the stack?* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128843/939928064245239878)

    FeedTheFed | StarkWare --- *see the links I gave, they explained precisely this (tldr, you want the reference value to be independent of the branch chosen, by adding this tempvar to both branches the reference is to [ap-1])* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128843/939927255608623175)

    th0rgal --- *> If I understand correctly, by calling _merge_util, I have shifted an indeterminate number of cells in ap, and the compiler doesn't have much way to find it. > So here the idea is to create a local reference using the keyword local. So my variable will no longer be in ap but in fp To face the "revoked reference issue" which I understood as an unknown shift in ap we used fp (local). But for the conditional example in the documentation, they are using tempvar. How would that work?* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128843/939926422254911618)

2. **652210513886969902, revoke, next_best_plots_amount end understand**

    th0rgal --- *Sure. It's at the end of this section:* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128843/939926830717235301)

    FeedTheFed | StarkWare --- *can you link the example you're talking about?* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128843/939926723963805697)

    th0rgal --- *Thank you, I'll make sure to read those. I have a question though* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128843/939925950831943700)

</details>

&nbsp;  

---

<details>
<summary>

## **🤗-dev-support** - [26 new messages 📨](https://discord.com/channels/793094838509764618/793094838987128844)

</summary>

---

### ↩️ **Messages with most replies**

* [2 ↩️] *Let's do the math together according the SN fee formula. For the sake of this calculation let's assume you don't have any L2->L1 messages and even you don't change any state (storage) in your transaction (which has relatively very high cost and will push the numbers even higher). Just the 250K steps. Let's assume the following: gas_price = 100 gwei gas_per_step = 0.3 (**Starkware team**, if you have a more accurate estimation, pls correct me) Eth price = $3K  So, 100 * 10^(-9) * (250K *0.3) * 3000 = $22.5* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128844/939806921052016640)

* [2 ↩️] *Is it fine to deploy contracts with computationally expensive calls to the testnet? Not sure the kind of things that have been deployed before, but a small test in chess.cairo of checking the legality of 3 moves, advancing the board, and getting the result of a state currently takes 2M steps. (we haven't tackled on improving performance yet) This takes around 3 min in my computer and 4 GB RAM so I'm asking if it's "civic" to deploy this as it is to testnet, or should we fix performance first?* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128844/939739556075438102)


---


### 🔝 **Topics and related messages**

1. **gas_per_step, takes, precise**

    Verde --- *If uploading 250k steps costs 75k gas then yeah it'd be pretty insane. I'm not sure if 0.3 is excessive or not, but it'd make many use cases prohibitively expensive, what would be the point then? Getting a more precise estimate (at least, the order of magnitude) for the gas_per_step is very important to me, because I'm deliberately making it more expensive computationally to require less storage updates. So far, all it takes it 1 state change (so, 2 slots of calldata) + steps to move. But, I'll work on reducing the number of steps, I got a bunch of ideas* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128844/939927426035761302)

    mottyl --- *Let's do the math together according the SN fee formula. For the sake of this calculation let's assume you don't have any L2->L1 messages and even you don't change any state (storage) in your transaction (which has relatively very high cost and will push the numbers even higher). Just the 250K steps. Let's assume the following: gas_price = 100 gwei gas_per_step = 0.3 (**Starkware team**, if you have a more accurate estimation, pls correct me) Eth price = $3K  So, 100 * 10^(-9) * (250K *0.3) * 3000 = $22.5* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128844/939806921052016640)

    Verde --- *Does it cost dozens of dollars to emit 250k steps?* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128844/939789011755614218)

2. **using, 986, py line**

    smchala --- *Hello, just following : https://starknet.io/docs/hello_starknet/account_setup.html#installation got the following error while trying to Creating an account: deploy_account:  Got ClientConnectorCertificateError Traceback (most recent call last):   File "/cairo_venv/lib/python3.8/site-packages/aiohttp/connector.py", line 986, in _wrap_create_connection     return await self._loop.create_connection(*args, **kwargs)  # type: ignore[return-value]  ...  would you please help? not sure if my mac setup is not using the same python version or something else...?* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128844/939923483188658217)

    kmd --- *Thank you so much! many things are getting clearer.* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128844/939816365248901120)

    kmd --- *Great! I'll look into the code more. Thank you!* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128844/939727702083125269)

</details>

&nbsp;  

---

<details>
<summary>

## **✨-starknet** - [13 new messages 📨](https://discord.com/channels/793094838509764618/853954510515208192)

</summary>

---

### 💌 **Most reacted messages**

1. *https://twitter.com/ahboyash/status/1485939275065868289?s=20&t=H8fAugcbwKgMJWswEvBkpw  Added Starknet here! Lemme know if I missed out on anything 😮* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/853954510515208192/939585433938051132)


---
</details>

&nbsp;  

---

## **🍯-русский** - [7 new messages 📨](https://discord.com/channels/793094838509764618/895711335801819187)
&nbsp;  

---

## **🧹-report-a-spammer** - [4 new messages 📨](https://discord.com/channels/793094838509764618/908073673183862874)
&nbsp;  

---

## **🌐-argent-extension** - [4 new messages 📨](https://discord.com/channels/793094838509764618/908663762150645770)
&nbsp;  

---

## **🏗-starknet-js** - [4 new messages 📨](https://discord.com/channels/793094838509764618/927918707613786162)
&nbsp;  

---

## **🥐-français** - [3 new messages 📨](https://discord.com/channels/793094838509764618/802928244139360306)
&nbsp;  

---

## **🍚-فارسی** - [3 new messages 📨](https://discord.com/channels/793094838509764618/912406778204012564)
&nbsp;  

---

## **🕗-gm-gn** - [2 new messages 📨](https://discord.com/channels/793094838509764618/884341617992024105)
&nbsp;  

---

## **👷-community-jobs** - [2 new messages 📨](https://discord.com/channels/793094838509764618/898210860030386178)
&nbsp;  

---

## **👷-hardhat-plugin** - [2 new messages 📨](https://discord.com/channels/793094838509764618/912735106899275856)
&nbsp;  

---

## **🥨-deutsch** - [2 new messages 📨](https://discord.com/channels/793094838509764618/915844624176803882)
&nbsp;  

---

## **🐠-random** - [1 new message 📨](https://discord.com/channels/793094838509764618/893514287887294526)
&nbsp;  

---

## **⚒-dev-tools** - [1 new message 📨](https://discord.com/channels/793094838509764618/894580545311359026)
&nbsp;  

---

## **🥙-türkçe** - [1 new message 📨](https://discord.com/channels/793094838509764618/899302454020177970)
&nbsp;  

---

## **🔭-voyager-block-explorer** - [1 new message 📨](https://discord.com/channels/793094838509764618/912410047236149298)
&nbsp;  

---

## **🐞-starknet-bug-report** - [1 new message 📨](https://discord.com/channels/793094838509764618/920304241376104488)
&nbsp;  

---

## **📚-tutorials-support** - [1 new message 📨](https://discord.com/channels/793094838509764618/932633376563802152)
&nbsp;  

---

