# **Starkware** summary for **2022-01-29** - **2022-01-30**

<details>
<summary>

## **🤗-dev-support** - [38 new messages 📨](https://discord.com/channels/793094838509764618/793094838987128844)

</summary>

---


### 🔝 **Topics and related messages**

1. **address, signature, struct**

    dhruvkelawala.eth | Mesh Finance --- *Yes… that’s what I am referring to. I thought it was already deployed. Please let me know when you deploy on Monday* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128844/937292655296118815)

    martriay --- *so I cannot pass the signature as a parameter to the constructor, because that would have an effect on the deployment address* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128844/937233647491248128)

    FeedTheFed | StarkWare --- *Pretty sure that today you can't, as we don't yet support deploying from another contract (so this agrees with the current state of the system)* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128844/937232410658111490)

2. **stack, cairo, paper**

    timothyyyy --- *So there is no such thing as an actual stack in Cairo CPU* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128844/937347444839174185)

    xjonathanlei --- *it's not like a real stack where you can unwind things* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128844/937346591579336745)

    xjonathanlei --- *but even in that case I don't think you'll ever get stack too deep* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128844/937346520632676372)

3. **14, result, distance 14**

    th0rgal --- *It looks like it found the right result: ``get_distance_return_type(distance=14)``, but I think I am not using the right syntax* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128844/937406073831297055)

    th0rgal --- *```>       assert(d.result == 14) E       AssertionError: assert get_distance_return_type(distance=14) == 14 E        +  where get_distance_return_type(distance=14) = StarknetTransactionExecutionInfo(result=get_distance_return_type(distance=14), main_call_events=[], raw_events=[], l2_...tput_builtin': 0, 'ecdsa_builtin': 0, 'bitwise_builtin': 0, 'ec_op_builtin': 0}, n_memory_holes=0)), internal_calls=[]).result ```* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128844/937405910945525770)

    th0rgal --- *```py @pytest.mark.asyncio async def test_increase_balance():     """Test increase_balance method."""     # Create a new Starknet class that simulates the StarkNet     # system.     starknet = await Starknet.empty()      # Deploy the contract.     contract = await starknet.deploy(         source=CONTRACT_FILE,     )      d = await contract.get_distance(0, 0, 10, 10).call()     assert(d.result == 14)      d = await contract.get_distance(-5, -5, 5, 5).call()     assert(d.result == 14) ```* **&rarr;** [Discord Discussion](https://discord.com/channels/793094838509764618/793094838987128844/937405749171216384)

</details>

&nbsp;  

---

## **🦅-cairo-lang-support** - [18 new messages 📨](https://discord.com/channels/793094838509764618/793094838987128843)
&nbsp;  

---

## **✨-starknet** - [14 new messages 📨](https://discord.com/channels/793094838509764618/853954510515208192)
&nbsp;  

---

## **🥐-français** - [12 new messages 📨](https://discord.com/channels/793094838509764618/802928244139360306)
&nbsp;  

---

## **📚-tutorials-support** - [5 new messages 📨](https://discord.com/channels/793094838509764618/932633376563802152)
&nbsp;  

---

## **🥙-türkçe** - [4 new messages 📨](https://discord.com/channels/793094838509764618/899302454020177970)
&nbsp;  

---

## **🍯-русский** - [3 new messages 📨](https://discord.com/channels/793094838509764618/895711335801819187)
&nbsp;  

---

## **🐞-starknet-bug-report** - [3 new messages 📨](https://discord.com/channels/793094838509764618/920304241376104488)
&nbsp;  

---

## **🕗-gm-gn** - [2 new messages 📨](https://discord.com/channels/793094838509764618/884341617992024105)
&nbsp;  

---

## **🐠-random** - [2 new messages 📨](https://discord.com/channels/793094838509764618/893514287887294526)
&nbsp;  

---

## **🍱-日本語** - [2 new messages 📨](https://discord.com/channels/793094838509764618/899298454201835530)
&nbsp;  

---

## **🌐-argent-extension** - [2 new messages 📨](https://discord.com/channels/793094838509764618/908663762150645770)
&nbsp;  

---

## **🌮-español** - [1 new message 📨](https://discord.com/channels/793094838509764618/899344999509033011)
&nbsp;  

---

## **🍚-فارسی** - [1 new message 📨](https://discord.com/channels/793094838509764618/912406778204012564)
&nbsp;  

---

## **-dutch** - [1 new message 📨](https://discord.com/channels/793094838509764618/930527380265652264)
&nbsp;  

---

