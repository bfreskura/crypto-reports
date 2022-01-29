# **Starkware** summary for **2022-01-28** - **2022-01-29**

<details>
<summary>

## **🤗-dev-support** - [44 new messages 📨](https://discord.com/channels/793094838509764618/793094838987128844)

</summary>

---


### 🔝 **Topics and related messages**

1. **cost, list, array**

    Julian Okuyiga --- *It's basically just allocating space for a continuous block (a "segment") of memory.  In that example, it's being used to store a list of the `Location*` structs* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128844/936772970305683506)

    RoboTeddy --- *if you wanted to get fancy you could maintain a list of deleted indices, and if it's non-empty when you're doing an insertion you could grab the last index off that list and put the value in that place.  if num_appends > num_deletes over the long run, then that free list would generally be small, and your list generally wouldn't have lots of holes in it. but maintaining that free list isn't free since it costs ya some storage writes* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128844/936765682404704306)

    RoboTeddy --- *reading is much cheaper than writing in starknet, so it may actually be "surprisingly" worthwhile to just leave the tombstones in place. but it does depend on how the numbers work out — if you know the ratio of reads/appends/deletes you could calculate it out* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128844/936765330729099324)

2. **cairo, stack deep, docs starknet**

    timothyyyy --- *so there is still some sort of stack too deep when you write a starknet contract?* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128844/937037530677792828)

    Gman --- *https://github.com/dydxprotocol/dydx-v3-python/blob/master/dydx3/modules/onboarding.py  dydx seems to derive a stark key from an eth signature. Does that mean anyone with that signature will be able to gain access to the dydx account and control it without further signatures / approvals?* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128844/936736372964864070)

    Gman --- *nvm I found the tutorial section* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128844/936726304928194630)

</details>

&nbsp;  

---

<details>
<summary>

## **✨-starknet** - [17 new messages 📨](https://discord.com/channels/793094838509764618/853954510515208192)

</summary>

---

### ↩️ **Messages with most replies**

* [2 ↩️] *Starknet commits to Ethereum every few hours right? In the worst case scenario where for some reason Starkware is told to shut all provers and verifiers, if your transaction doesn't get committed to L1 is it lost or can you still use the escape hatch and force include transactions?* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/853954510515208192/936949351509524540)


---
</details>

&nbsp;  

---

## **🦅-cairo-lang-support** - [11 new messages 📨](https://discord.com/channels/793094838509764618/793094838987128843)
&nbsp;  

---

## **🌐-argent-extension** - [8 new messages 📨](https://discord.com/channels/793094838509764618/908663762150645770)
&nbsp;  

---

## **🥐-français** - [4 new messages 📨](https://discord.com/channels/793094838509764618/802928244139360306)
&nbsp;  

---

## **🕗-gm-gn** - [2 new messages 📨](https://discord.com/channels/793094838509764618/884341617992024105)
&nbsp;  

---

## **🍚-فارسی** - [2 new messages 📨](https://discord.com/channels/793094838509764618/912406778204012564)
&nbsp;  

---

## **🐞-starknet-bug-report** - [2 new messages 📨](https://discord.com/channels/793094838509764618/920304241376104488)
&nbsp;  

---

## **warp-transpiler** - [2 new messages 📨](https://discord.com/channels/793094838509764618/935889632124616765)
&nbsp;  

---

## **⚒-dev-tools** - [1 new message 📨](https://discord.com/channels/793094838509764618/894580545311359026)
&nbsp;  

---

## **🍯-русский** - [1 new message 📨](https://discord.com/channels/793094838509764618/895711335801819187)
&nbsp;  

---

## **🥙-türkçe** - [1 new message 📨](https://discord.com/channels/793094838509764618/899302454020177970)
&nbsp;  

---

## **📚-tutorials-support** - [1 new message 📨](https://discord.com/channels/793094838509764618/932633376563802152)
&nbsp;  

---

