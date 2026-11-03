<a id="top"></a>

<p align="center">
  <img src="https://i.imgur.com/hSLVhdU.png" alt="Lusty Looters logo" width="180">
</p>

<h1 align="center">Lusty Looters — Daily &amp; Weekly Quest Rework</h1>

<p align="center">
  Dailies cover quick goals across different playstyles. Weeklies focus on gathering, crafting and useful supplies that players can work towards throughout the week.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Daily%20Quests-121-8b5cf6?style=for-the-badge" alt="121 daily quests">
  <img src="https://img.shields.io/badge/Weekly%20Quests-100-22c55e?style=for-the-badge" alt="100 weekly quests">
  <img src="https://img.shields.io/badge/Status-In-game%20Checks%20Pending-f59e0b?style=for-the-badge" alt="completion testing pending">
  <img src="https://img.shields.io/badge/Live%20Rollout-Unconfirmed-3b82f6?style=for-the-badge" alt="cluster-wide live rollout unconfirmed">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Daily%20Reward-5%2C000%20Gold%20Nuggets-eab308?style=for-the-badge" alt="5000 Gold Nuggets per daily">
  <img src="https://img.shields.io/badge/Weekly%20Reward-25%2C000%20Gold%20Nuggets-eab308?style=for-the-badge" alt="25000 Gold Nuggets per weekly">
</p>

> [!IMPORTANT]
> **All 121 dailies and 100 weeklies are configured.** Dailies award **5,000 Gold Nuggets** and weeklies award **25,000 Gold Nuggets**, with no additional item or dino rewards. Two weekly quest views have been shown in-game, confirming that they load and display. Completion credit, payouts, reset behaviour and availability on every map still need testing.

> [!NOTE]
> Daily and weekly configuration work is complete. **Permanent quest balancing is the next phase**, followed by a possible review of shop prices and the wider Gold Nugget economy. The current payouts are not a declaration that the economy review is finished.

> [!WARNING]
> Cross-map availability is a design goal, not a completed test. Creature spawns, resource access, engrams and crafting-station compatibility still need checking on each map. Element gathering credit also needs a specific in-game test.

## Quick links

- [Overview](#overview)
- [Rewards and store changes](#rewards-and-store-changes)
- [How objectives and counters work](#how-objectives-and-counters-work)
- [Daily rules and variant support](#daily-rules-and-variant-support)
- [Weekly rules](#weekly-rules)
- [Daily quest list](#daily-quest-list)
  - [Biome hunts](#biome-hunts)
  - [Creature hunts](#creature-hunts)
  - [Creature class hunts](#creature-class-hunts)
  - [Gathering](#gathering)
  - [Crafting](#crafting)
  - [Special & mixed](#special--mixed)
- [Weekly quest list](#weekly-quest-list)
  - [Supplies and ammunition](#weekly-supplies-and-ammunition)
  - [Manufacturing](#weekly-manufacturing)
  - [Weapons and tools](#weekly-weapons-and-tools)
  - [Saddles](#weekly-saddles)
  - [Clothing](#weekly-clothing)
- [Configuration checks](#configuration-checks)
- [Testing and rollout](#testing-and-rollout)
- [Credits](#credits)

## Overview

Updated **3 November 2026**.

| Quest pool | Configured | Reward per quest |
| :-- | --: | --: |
| Daily | 121 | 5,000 Gold Nuggets |
| Weekly | 100 | 25,000 Gold Nuggets |
| Permanent | 126 | Existing rewards; balance review pending |
| **Total in the config** | **347** | |

The daily pool replaces the previous 31 dailies: 18 were retained or reworked, 13 were retired and 103 new quests were added. The weekly pool replaces the previous 17 weeklies with **100 progression quests**. The earlier hunt-based weekly draft has been superseded.

### Status tags

- `configured` means the quest is included in the current JSON, with its objectives, counters and reward set.
- It does **not** mean completion credit, payouts or every map have been tested. Cluster-wide live rollout remains unconfirmed.

### Rewards and store changes

- **Dailies:** exactly 5,000 Gold Nuggets each, with no extra rewards.
- **Weeklies:** exactly 25,000 Gold Nuggets each, with no extra rewards.
- **Assignments:** the config currently allows up to 3 dailies and 2 weeklies at a time. The listed pools are the selection pools, not simultaneous assignments.
- **Reset Dailies:** removed from the prepared shop config. Its removal from the live store still needs confirming.
- **Other shop settings:** existing prices, previous product removals and the reduced Red Gem selling rule are unchanged by this quest update.
- **Next phase:** permanent quest requirements and rewards, followed by a possible wider economy review.

## How objectives and counters work

Alternatives within one objective share **one total**. Separate requirements must **all** be completed.

- A hunt requiring 20 Sarcos, Kaprosuchus or Piranhas means **20 qualifying kills total**, in any combination.
- A gathering objective requiring 50,000 Wood, Fungal Wood, Stone or Metal Ore means **50,000 resources total**, not 50,000 of each.
- A weekly requiring a daily completion, gathering and two crafted supplies has four separate requirements.
- Eligible materials and items are listed in the description. A short progress label does not expand what counts.

### Counter labels

| Objective | Progress label |
| :-- | :-- |
| A shared gathering group | Resources Gathered |
| A single resource | Metal Ore Gathered, Element Gathered or the matching resource name |
| Crafted supplies | Tranq Arrows Crafted, Shotgun Shells Crafted or the matching item name |
| Required daily completion | Daily Quests Completed |

Internal group names and unrelated map prefixes have been removed from the relevant counter labels. The display-label review changed no tracking keys, targets, quantities or rewards.

## Daily rules and variant support

- No daily taming objectives.
- Biome hunts require **20 kills each**.
- Grouped hunts count eligible variants towards the same total.
- The cross-map goal remains playable objectives without needing to transfer; live spawn coverage still needs checking.

The supplied **12 EVO paths** are included in the relevant daily hunt groups.

| EVO group | Included variants |
| :-- | :-- |
| Rex / Tarbo | Tarbo, Paleo Rex, Legacy Rex, Volcano Rex and Tek Rex |
| Alpha Rex / Tarbo | Alpha Tarbo, Alpha Rex and Alpha Legacy Rex |
| Giganotosaurus | EVO Giga, Paleo Giga, Volcano Giga and Wasteland Giga |

Ordinary Rex hunts also accept the configured Alpha Rex/Tarbo variants. Alpha objectives require qualifying Alphas; ordinary Rex or Giga variants do not satisfy them. Actual spawning and kill credit still need checking.

## Weekly rules

Weeklies focus on gathering and crafting that players can chip away at throughout normal play.

- **Every weekly requires exactly 1 daily completion**, plus its listed gathering and crafting objectives.
- **No weekly hunting, taming, boss, structure or placeable objectives.**
- Crafting quantities vary by cost. Cheap ammunition and powders have larger counts; expensive supplies and equipment have smaller counts.
- Persistent weapons, tools and saddles are limited to **1–2 items combined per weekly**. Ammunition and consumables have their own listed quantities.
- Clothing objectives require **one matching five-piece set**, with a separate requirement for each slot. Five helmets cannot replace a complete set.
- Multiple listed crafting requirements are all required. Alternatives inside one crafting group share its total.

### Weekly gathering targets

| Resource tier | Required total | Eligible materials used in the pool |
| :-- | --: | :-- |
| Common | 50,000 | Wood, Fungal Wood, Stone, Flint, Metal Ore, Fibre, Thatch and Hide |
| Rare | 10,000 | Crystal, Obsidian, Oil, Silica Pearls, Rare Flowers, Rare Mushrooms, Organic Polymer, Chitin, Keratin and Pelt |
| Element | 5,000 | Actual Element |
| Black Pearls | 5,000 | Black Pearls |

Each quest lists its own eligible resources. Common and rare materials do not share a counter. Element and Black Pearls have separate objectives; Element Dust, Shards and Ore are not configured as substitutes for Element.

The weekly pool contains **63 common-resource quests, 33 rare-resource quests, 2 Element quests and 2 Black Pearl quests**. Gathering credit must still be tested, particularly for Element acquisition methods.

<a id="quest-list"></a>
## Daily quest list

**Every daily below awards 5,000 Gold Nuggets.** Open a section to view its quests.
Open each section to see its quests.

<a id="biome-hunts"></a>
<details>
<summary><strong>🌿 Biome hunts (36)</strong></summary>

### Swamp — Bogged Down

1. **Bogged Down 1** — Kill 20 creatures in any combination: Sarco, Deinosuchus, Kaprosuchus, Beelzebufo, Piranha, or Titanoboa. `configured`
2. **Bogged Down 2** — Kill 20 creatures in any combination: Rhyniognatha, Baryonyx, Piranha, Paraceratherium, Sarco, or Titanoboa. `configured`
3. **Bogged Down 3** — Kill 20 creatures in any combination: Titanoboa, Dimetrodon, Meganeura, Spinosaurus, Kaprosuchus, or Piranha. `configured`

### Beach Cleanup

4. **Beach Cleanup 1** — Kill 20 creatures in any combination: Dodo, Dilophosaur, Lystrosaurus, Parasaur, Moschops, or Raptor. `configured`
5. **Beach Cleanup 2** — Kill 20 creatures in any combination: Carbonemys, Trilobite, Ichthyosaurus, Pteranodon, Coelacanth, or Raptor. `configured`
6. **Beach Cleanup 3** — Kill 20 creatures in any combination: Phiomia, Coelacanth, Sabertooth Salmon, Piranha, Dilophosaur, or Parasaur. `configured`

### Snow Rundown

7. **Snow Rundown 1** — Kill 20 creatures in any combination: Direwolf, Mammoth, Yutyrannus, Sabertooth, Woolly Rhino, or Purlovia. `configured`
8. **Snow Rundown 2** — Kill 20 creatures in any combination: Daeodon, Purlovia, Kairuku, Megatherium, Snow Owl, or Raptor. `configured`
9. **Snow Rundown 3** — Kill 20 creatures in any combination: Cryolophosaurus, Managarmr, Direwolf, Mammoth, Sabertooth, or Purlovia. `configured`

### Cave Culling

10. **Cave Culling 1** — Kill 20 creatures in any combination: Araneo, Arthropluera, Onyc, Pulmonoscorpius, or Megalania. `configured`
11. **Cave Culling 2** — Kill 20 creatures in any combination: Piranha, Meganeura, Titanoboa, Megalosaurus, or Purlovia. `configured`
12. **Cave Culling 3** — Kill 20 creatures in any combination: Nameless, Ravager, Karkinos, Basilisk, Reaper Queen, Araneo, or Arthropluera. `configured`

### Jungle Sweep

13. **Jungle Sweep 1** — Kill 20 creatures in any combination: Raptor, Carnotaurus, Iguanodon, Pachy, or Therizinosaur. `configured`
14. **Jungle Sweep 2** — Kill 20 creatures in any combination: Gallimimus, Terror Bird, Megatherium, Dilophosaur, Troodon, or Raptor. `configured`
15. **Jungle Sweep 3** — Kill 20 creatures in any combination: Microraptor, Moschops, Ceratosaurus, Gigantoraptor, or Raptor. `configured`

### Mountain Mayhem

16. **Mountain Mayhem 1** — Kill 20 creatures in any combination: Argentavis, Doedicurus, Ankylosaurus, Carnotaurus, or Allosaurus. `configured`
17. **Mountain Mayhem 2** — Kill 20 creatures in any combination: Rex, Sabertooth, Procoptodon, Equus, or Ovis. `configured`
18. **Mountain Mayhem 3** — Kill 20 creatures in any combination: Griffin, Giganotosaurus, Ceratosaurus, Quetzal, Carnotaurus, or Ankylosaurus. `configured`

### Redwoods Reckoning

19. **Redwoods Reckoning 1** — Kill 20 creatures in any combination: Thylacoleo, Terror Bird, Dire Bear, Megaloceros, or Raptor. `configured`
20. **Redwoods Reckoning 2** — Kill 20 creatures in any combination: Troodon, Gigantopithecus, Purlovia, Allosaurus, or Carnotaurus. `configured`
21. **Redwoods Reckoning 3** — Kill 20 creatures in any combination: Archaeopteryx, Microraptor, Diplodocus, Acrocanthosaurus, or Thylacoleo. `configured`

### Ocean Sweep

22. **Ocean Sweep 1** — Kill 20 creatures in any combination: Megalodon, Manta, Electrophorus, Cnidaria, Anglerfish, or Piranha. `configured`
23. **Ocean Sweep 2** — Kill 20 creatures in any combination: Mosasaurus, Plesiosaur, Tusoteuthis, Dunkleosteus, Xiphactinus, or Piranha. `configured`
24. **Ocean Sweep 3** — Kill 20 creatures in any combination: Basilosaurus, Ichthyosaurus, Archelon, Leedsichthys, Manta, or Piranha. `configured`

### Desert — Our Home

25. **Our Home 1** — Kill 20 creatures in any combination: Morellatops, Thorny Dragon, Mantis, Lymantria, Vulture, or Pulmonoscorpius. `configured`
26. **Our Home 2** — Kill 20 creatures in any combination: Deathworm, Rock Elemental, Pulmonoscorpius, Equus, Jerboa, or Carnotaurus. `configured`
27. **Our Home 3** — Kill 20 creatures in any combination: Carnotaurus, Wyvern, Arthropluera, Fasolasuchus, Concavenator, or Pulmonoscorpius. `configured`

### Plains Patrol

28. **Plains Patrol 1** — Kill 20 creatures in any combination: Triceratops, Stegosaurus, Brontosaurus, Parasaur, Phiomia, or Equus. `configured`
29. **Plains Patrol 2** — Kill 20 creatures in any combination: Ovis, Gallimimus, Equus, Procoptodon, or Iguanodon. `configured`
30. **Plains Patrol 3** — Kill 20 creatures in any combination: Therizinosaur, Giganotosaurus, Bison, Stegosaurus, Triceratops, or Equus. `configured`

### River Run

31. **River Run 1** — Kill 20 creatures in any combination: Castoroides, Baryonyx, Sarco, Deinosuchus, Spinosaurus, or Piranha. `configured`
32. **River Run 2** — Kill 20 creatures in any combination: Titanoboa, Coelacanth, Sabertooth Salmon, Piranha, or Kaprosuchus. `configured`
33. **River Run 3** — Kill 20 creatures in any combination: Otter, Carbonemys, Baryonyx, Sarco, or Piranha. `configured`

### Volcano Sweep

34. **Volcano Sweep 1** — Kill 20 creatures in any combination: Rex, Allosaurus, Carnotaurus, Argentavis, or Ankylosaurus. `configured`
35. **Volcano Sweep 2** — Kill 20 creatures in any combination: Doedicurus, Magmasaur, Rock Elemental, Wyvern, or Basilisk. `configured`
36. **Volcano Sweep 3** — Kill 20 creatures in any combination: Thorny Dragon, Pulmonoscorpius, Araneo, Mantis, or Arthropluera. `configured`

[Back to top](#top)

</details>

<a id="creature-hunts"></a>
<details>
<summary><strong>🦖 Creature hunts (25)</strong></summary>

37. **Small Game Sweep** — Kill 5 creatures in any combination: Dodo or Jerboa. `configured`
38. **Take Out the Trash** — Kill 10 Dung Beetles. `configured`
39. **Piranha Predator** — Kill 50 Piranhas. `configured`
40. **Exterminator Extraordinaire** — Kill 20 creatures in any combination: Meganeura, Titanomyrma, Mantis, Pulmonoscorpius, Araneo, Arthropluera, or Dung Beetle. `configured`
41. **Monster Hunt** — Kill 1 creature from this group: Tusoteuthis, Karkinos, Deinosuchus, or Spinosaurus. `configured`
42. **Predator Patrol** — Kill 10 Raptors. `configured`
43. **Big Game Cull** — Kill 5 creatures in any combination: Rex, Spinosaurus, or Carnotaurus. `configured`
44. **Cave Clearance** — Kill 20 creatures in any combination: Onyc, Araneo, or Arthropluera. `configured`
45. **Centipede Control** — Kill 25 Arthropluera. `configured`
46. **Predator Shutdown** — Kill 5 creatures in any combination: Managarmr, Ravager, or Carnotaurus. `configured`
47. **Swamp Jaws** — Kill 15 creatures in any combination: Sarco or Deinosuchus. `configured`
48. **Swamp Ambush** — Kill 15 creatures in any combination: Kaprosuchus, Sarco, or Deinosuchus. `configured`
49. **Predator Bounty** — Kill 12 creatures in any combination: Baryonyx or Carnotaurus. `configured`
50. **Big Game Pursuit** — Kill 5 creatures in any combination: Spinosaurus, Rex, or Carnotaurus. `configured`
51. **Fang and Claw** — Kill 15 creatures in any combination: Carnotaurus or Raptor. `configured`
52. **Carnivore Ambush** — Kill 12 creatures in any combination: Allosaurus or Carnotaurus. `configured`
53. **Feathered Fury** — Kill 20 creatures in any combination: Terror Bird or Raptor. `configured`
54. **Forest Threats** — Kill 10 creatures in any combination: Thylacoleo, Dire Bear, or Carnotaurus. `configured`
55. **Pack Breaker** — Kill 20 creatures in any combination: Direwolf or Raptor. `configured`
56. **Heavy Hitters** — Kill 10 creatures in any combination: Mammoth, Paraceratherium, Morellatops, or Carnotaurus. `configured`
57. **Winged Hunt** — Kill 15 creatures in any combination: Argentavis, Dimorphodon, or Yi Ling. `configured`
58. **Crawler Control** — Kill 15 creatures in any combination: Mantis or Arthropluera. `configured`
59. **Waterway Hunt** — Kill 10 creatures in any combination: Anglerfish, Piranha, or Electrophorus. `configured`
60. **Danger Below** — Kill 15 creatures in any combination: Megalodon, Piranha, or Electrophorus. `configured`
61. **Tough Targets** — Kill 1 creature from this group: Rock Elemental, Ankylosaurus, or Doedicurus. `configured`

[Back to top](#top)

</details>

<a id="creature-class-hunts"></a>
<details>
<summary><strong>🧬 Creature class hunts (15)</strong></summary>

62. **Apex Predator** — Kill 1 creature from this group: Giganotosaurus, Carcharodontosaurus, Reaper Queen, Rex, Spinosaurus, or Acrocanthosaurus. `configured`
63. **Large Carnivore Hunter** — Kill 5 creatures in any combination: Rex, Spinosaurus, Acrocanthosaurus, Deinosuchus, Wyvern, or Carnotaurus. `configured`
64. **Medium Carnivore Hunter** — Kill 10 creatures in any combination: Allosaurus, Baryonyx, Carnotaurus, or Ceratosaurus. `configured`
65. **Small Carnivore Hunter** — Kill 20 creatures in any combination: Raptor, Dilophosaur, Compy, Troodon, or Microraptor. `configured`
66. **Apex Herbivore Hunter** — Kill 2 creatures in any combination: Titanosaur, Brontosaurus, Diplodocus, or Paraceratherium. `configured`
67. **Large Herbivore Hunter** — Kill 6 creatures in any combination: Diplodocus, Paraceratherium, Mammoth, Morellatops, or Stegosaurus. `configured`
68. **Medium Herbivore Hunter** — Kill 15 creatures in any combination: Triceratops, Stegosaurus, Iguanodon, Bison, or Morellatops. `configured`
69. **Small Herbivore Hunter** — Kill 20 creatures in any combination: Dodo, Lystrosaurus, Moschops, Phiomia, Ovis, or Jerboa. `configured`
70. **Sky Hunter** — Kill 15 creatures in any combination: Argentavis, Pteranodon, Tapejara, Pelagornis, or Dimorphodon. `configured`
71. **Bug Exterminator** — Kill 20 creatures in any combination: Meganeura, Titanomyrma, Mantis, or Pulmonoscorpius. `configured`
72. **Aquatic Predator** — Kill 10 creatures in any combination: Megalodon, Anglerfish, Electrophorus, Xiphactinus, or Piranha. `configured`
73. **Coastal Forager** — Kill 20 creatures in any combination: Trilobite, Coelacanth, Hesperornis, or Piranha. `configured`
74. **Armoured Beasts** — Kill 10 creatures in any combination: Doedicurus, Ankylosaurus, Kentrosaurus, or Stegosaurus. `configured`
75. **Pack Hunters** — Kill 20 creatures in any combination: Raptor, Direwolf, Ravager, or Terror Bird. `configured`
76. **Creatures of the Dark** — Kill 10 creatures in any combination: Troodon, Onyc, Megalania, or Megalosaurus. `configured`

[Back to top](#top)

</details>

<a id="gathering"></a>
<details>
<summary><strong>⛏️ Gathering (20)</strong></summary>

77. **Miner’s Madness** — Gather 25,000 Metal Ore. `configured`
78. **Wood Run** — Gather 25,000 resources in any combination: Wood or Fungal Wood. `configured`
79. **Silica Expedition** — Gather 5,000 Silica Pearls. `configured`
80. **Timber Surge** — Gather 25,000 resources in any combination: Wood, Fungal Wood, Thatch, or Fibre. `configured`
81. **Ore Scout** — Gather 25,000 resources in any combination: Stone or Flint. `configured`
82. **Metal Rush** — Gather 25,000 resources in any combination: Metal Ore, Stone, or Flint. `configured`
83. **Stone Quarry** — Gather 25,000 Stone. `configured`
84. **Flint Run** — Gather 25,000 Flint. `configured`
85. **Thatch Gathering** — Gather 25,000 Thatch. `configured`
86. **Fibre Collection** — Gather 25,000 Fibre. `configured`
87. **Rare Mushroom Harvest** — Gather 3,000 Rare Mushrooms. `configured`
88. **Hide Drive** — Gather 25,000 Hide. `configured`
89. **Chitin Stockpile** — Gather 25,000 Chitin. `configured`
90. **Keratin Sweep** — Gather 25,000 Keratin. `configured`
91. **Crystal Run** — Gather 5,000 Crystal. `configured`
92. **Obsidian Stockpile** — Gather 5,000 Obsidian. `configured`
93. **Oil Reserves** — Gather 5,000 Oil. `configured`
94. **Organic Polymer Hunt** — Gather 3,000 Organic Polymer. `configured`
95. **Black Pearl Dive** — Gather 3,000 Black Pearls. `configured`
96. **Rare Flower Harvest** — Gather 5,000 Rare Flowers. `configured`

[Back to top](#top)

</details>

<a id="crafting"></a>
<details>
<summary><strong>🛠️ Crafting (15)</strong></summary>

97. **Chitin and Paste** — Gather 1,000 Chitin and craft 500 Cementing Paste. `configured`
98. **Arrow Assembly** — Craft 250 Stone Arrows. `configured`
99. **Tranq Supply** — Craft 100 Tranq Arrows. `configured`
100. **Narcotic Workshop** — Craft 250 Narcotics. `configured`
101. **Stimulant Reserve** — Craft 150 Stimulants. `configured`
102. **Medical Supply** — Craft 100 Medical Brews. `configured`
103. **Gunpowder Stock** — Craft 2,000 Gunpowder. `configured`
104. **Sparkpowder Stock** — Craft 3,000 Sparkpowder. `configured`
105. **Ammunition Run** — Craft 500 Advanced Rifle Bullets. `configured`
106. **Shotgun Stock** — Craft 250 Shotgun Shells. `configured`
107. **Paste Production** — Craft 1,000 Cementing Paste. `configured`
108. **Electronics Assembly** — Craft 500 Electronics. `configured`
109. **Polymer Workshop** — Craft 1,000 Polymer. `configured`
110. **Metal Ingot Batch** — Craft 5,000 Metal Ingots. `configured`
111. **Structural Sprint** — Craft 100 Stone Foundations. `configured`

[Back to top](#top)

</details>

<a id="special--mixed"></a>
<details>
<summary><strong>⚔️ Special &amp; mixed (10)</strong></summary>

112. **Bounty Hunt** — Kill 5 large predators (Rex, Spinosaurus, Acrocanthosaurus, Deinosuchus, or Carnotaurus) and 10 small predators (Raptor, Dilophosaur, or Troodon). Each group has its own shared total. `configured`
113. **Alpha Slayer** — Kill 3 eligible Alpha creatures in any combination. Includes EVO Alpha Rex and Tarbo, aquatic Alphas, and map-specific Alphas. `configured`
114. **Snowline Defense** — Kill 15 creatures in any combination: Direwolf, Yutyrannus, Purlovia, Carnotaurus, or Raptor. `configured`
115. **Cave Resource Strike** — Kill 5 total Onyc, Araneo or Arthropluera and gather 5,000 Crystal. `configured`
116. **River Menace** — Kill 15 creatures in any combination: Baryonyx, Sarco, Kaprosuchus, Piranha, Deinosuchus, or Spinosaurus. `configured`
117. **Coastal Security** — Kill 15 creatures in any combination: Dilophosaur, Raptor, Troodon, Parasaur, or Triceratops. `configured`
118. **Mountain Sweep** — Kill 10 creatures in any combination: Argentavis, Allosaurus, Rex, Ankylosaurus, Doedicurus, or Carnotaurus. `configured`
119. **Predator Control** — Kill 15 creatures in any combination: Carnotaurus, Raptor, Dilophosaur, Baryonyx, or Troodon. `configured`
120. **Ocean Depths** — Kill 10 creatures in any combination: Mosasaurus, Megalodon, Piranha, Electrophorus, Anglerfish, or Cnidaria. `configured`
121. **Alpha Interception** — Kill 1 Alpha Raptor, Alpha Rex, Alpha Basilisk, Alpha Karkinos, Alpha Fire Wyvern, Alpha Deathworm, or Alpha Surface Reaper King. EVO Alpha Rex and Tarbo count. `configured`

[Back to top](#top)

</details>


## Weekly quest list

**Every weekly below requires 1 daily completion and awards 25,000 Gold Nuggets.**

<a id="weekly-supplies-and-ammunition"></a>
<details>
<summary><strong>📦 Supplies and ammunition (30)</strong></summary>

Requires **1 daily completion** plus all listed objectives. **Reward: 25,000 Gold Nuggets each.**

1. **Supply Run** — Gather 50,000 resources in any combination: Wood, Fungal Wood, Stone, or Metal Ore; craft 1,000 items in any combination: Stone Arrows, Tranq Arrows, Advanced Rifle Bullets, or Shotgun Shells. `configured`
2. **Frontier Stockpile** — Gather 50,000 resources in any combination: Stone, Flint, or Metal Ore; craft 500 Narcotics; craft 250 Tranq Arrows. `configured`
3. **Arrow Reserve** — Gather 50,000 resources in any combination: Wood, Fungal Wood, Thatch, or Fibre; craft 1,000 Stone Arrows. `configured`
4. **Tranq Reserve** — Gather 50,000 resources in any combination: Fibre, Wood, Fungal Wood, Thatch, or Hide; craft 500 Tranq Arrows. `configured`
5. **Narcotic Reserve** — Gather 50,000 resources in any combination: Fibre, Wood, Fungal Wood, Thatch, or Hide; craft 1,000 Narcotics. `configured`
6. **Medical Reserve** — Gather 10,000 resources in any combination: Rare Flowers, or Rare Mushrooms; craft 100 Medical Brews. `configured`
7. **Stimulant Reserve** — Gather 50,000 resources in any combination: Hide, Fibre, Wood, or Fungal Wood; craft 500 Stimulants. `configured`
8. **Rifle Reserve** — Gather 50,000 resources in any combination: Stone, Flint, or Metal Ore; craft 1,000 Advanced Rifle Bullets. `configured`
9. **Shotgun Reserve** — Gather 50,000 resources in any combination: Stone, Flint, or Metal Ore; craft 250 Shotgun Shells. `configured`
10. **Sidearm Reserve** — Gather 50,000 resources in any combination: Metal Ore, Wood, Fungal Wood, or Hide; craft 300 Simple Bullets. `configured`
11. **Longneck Reserve** — Gather 50,000 resources in any combination: Metal Ore, Wood, Fungal Wood, or Hide; craft 250 Simple Rifle Ammo. `configured`
12. **Dart Reserve** — Gather 50,000 resources in any combination: Fibre, Wood, Fungal Wood, Thatch, or Hide; craft 100 Tranquilizer Darts. `configured`
13. **Compound Ammunition** — Gather 10,000 resources in any combination: Crystal, Obsidian, or Silica Pearls; craft 250 Metal Arrows. `configured`
14. **Sniper Reserve** — Gather 10,000 resources in any combination: Crystal, Obsidian, Oil, or Silica Pearls; craft 200 Advanced Sniper Bullets. `configured`
15. **Pistol Reserve** — Gather 50,000 resources in any combination: Stone, Flint, or Metal Ore; craft 500 Advanced Bullets. `configured`
16. **Balanced Medicine** — Gather 50,000 resources in any combination: Hide, Fibre, Wood, or Fungal Wood; craft 500 Narcotics; craft 250 Stimulants. `configured`
17. **Field Medicine** — Gather 50,000 resources in any combination: Hide, Fibre, Wood, or Fungal Wood; craft 100 Medical Brews; craft 250 Stimulants. `configured`
18. **Tamer Preparation** — Gather 50,000 resources in any combination: Fibre, Wood, Fungal Wood, Thatch, or Hide; craft 500 Narcotics; craft 50 Tranquilizer Darts. `configured`
19. **Arrow and Dart** — Gather 50,000 resources in any combination: Fibre, Wood, Fungal Wood, Thatch, or Hide; craft 250 Tranq Arrows; craft 50 Tranquilizer Darts. `configured`
20. **Mixed Firepower** — Gather 50,000 resources in any combination: Stone, Flint, or Metal Ore; craft 500 Advanced Rifle Bullets; craft 125 Shotgun Shells. `configured`
21. **Powder and Shot** — Gather 50,000 resources in any combination: Stone, Flint, or Metal Ore; craft 2,000 Gunpowder; craft 200 Simple Bullets. `configured`
22. **Rifle Workshop** — Gather 50,000 resources in any combination: Metal Ore, Wood, Fungal Wood, or Hide; craft 150 Simple Rifle Ammo; craft 500 Advanced Rifle Bullets. `configured`
23. **Dual Sidearms** — Gather 50,000 resources in any combination: Metal Ore, Wood, Fungal Wood, or Hide; craft 150 Simple Bullets; craft 250 Advanced Bullets. `configured`
24. **Bow Supplies** — Gather 50,000 resources in any combination: Wood, Fungal Wood, Thatch, or Fibre; craft 500 Stone Arrows; craft 250 Tranq Arrows. `configured`
25. **Precision Supplies** — Gather 10,000 resources in any combination: Crystal, Obsidian, or Silica Pearls; craft 150 Metal Arrows; craft 100 Advanced Sniper Bullets. `configured`
26. **Medic and Tamer** — Gather 10,000 resources in any combination: Rare Flowers, or Rare Mushrooms; craft 75 Medical Brews; craft 500 Narcotics. `configured`
27. **Steady Hands** — Gather 50,000 resources in any combination: Hide, Fibre, Wood, or Fungal Wood; craft 250 Stimulants; craft 50 Tranquilizer Darts. `configured`
28. **Field Restock** — Gather 50,000 resources in any combination: Wood, Fungal Wood, Stone, Fibre, Thatch, Flint, Metal Ore, or Hide; craft 500 Stone Arrows; craft 50 Medical Brews; craft 250 Narcotics. `configured`
29. **Range Supplies** — Gather 50,000 resources in any combination: Metal Ore, Wood, Fungal Wood, or Hide; craft 500 Advanced Rifle Bullets; craft 50 Medical Brews. `configured`
30. **Supply and Survive** — Gather 50,000 resources in any combination: Wood, Fungal Wood, Stone, Fibre, Thatch, Flint, Metal Ore, or Hide; craft 250 Tranq Arrows; craft 125 Shotgun Shells; craft 50 Medical Brews. `configured`

[Back to top](#top)

</details>

<a id="weekly-manufacturing"></a>
<details>
<summary><strong>⚙️ Manufacturing (20)</strong></summary>

Requires **1 daily completion** plus all listed objectives. **Reward: 25,000 Gold Nuggets each.**

31. **Sparkpowder Reserve** — Gather 50,000 resources in any combination: Stone, Flint, or Metal Ore; craft 10,000 Sparkpowder. `configured`
32. **Powder Works** — Gather 50,000 resources in any combination: Stone, Flint, or Metal Ore; craft 5,000 Gunpowder. `configured`
33. **Paste Batch** — Gather 10,000 resources in any combination: Chitin, or Keratin; craft 2,500 Cementing Paste. `configured`
34. **Circuit Batch** — Gather 10,000 resources in any combination: Crystal, Obsidian, or Silica Pearls; craft 500 Electronics. `configured`
35. **Polymer Batch** — Gather 10,000 resources in any combination: Crystal, Obsidian, Oil, or Silica Pearls; craft 500 Polymer. `configured`
36. **Powder Mill** — Gather 50,000 resources in any combination: Stone, Flint, or Metal Ore; craft 5,000 Sparkpowder; craft 2,500 Gunpowder. `configured`
37. **Fabricator Stock** — Gather 10,000 resources in any combination: Crystal, Obsidian, Oil, or Silica Pearls; craft 250 Electronics; craft 250 Polymer. `configured`
38. **Workshop Adhesives** — Gather 10,000 resources in any combination: Chitin, Keratin, or Organic Polymer; craft 1,500 Cementing Paste; craft 250 Polymer. `configured`
39. **Circuit Support** — Gather 10,000 resources in any combination: Crystal, Obsidian, or Silica Pearls; craft 250 Electronics; craft 1,000 Cementing Paste. `configured`
40. **Production Reserve** — Gather 50,000 resources in any combination: Wood, Fungal Wood, Stone, or Metal Ore; craft 5,000 Sparkpowder; craft 1,000 Cementing Paste. `configured`
41. **Gunshop Stock** — Gather 50,000 resources in any combination: Stone, Flint, or Metal Ore; craft 2,500 Gunpowder; craft 250 Electronics. `configured`
42. **Manufacturing Reserve** — Gather 50,000 resources in any combination: Wood, Fungal Wood, Stone, or Metal Ore; craft 5,000 Sparkpowder; craft 250 Polymer. `configured`
43. **Field Fabrication** — Gather 5,000 Black Pearls; craft 1,000 Cementing Paste; craft 250 Electronics; craft 250 Polymer. `configured`
44. **Taming Industry** — Gather 50,000 resources in any combination: Fibre, Wood, Fungal Wood, Thatch, or Hide; craft 500 Narcotics; craft 1,000 Cementing Paste. `configured`
45. **Medical Workshop** — Gather 10,000 resources in any combination: Rare Flowers, or Rare Mushrooms; craft 100 Medical Brews; craft 250 Stimulants; craft 500 Cementing Paste. `configured`
46. **Advanced Supply Line** — Gather 5,000 Element; craft 2,000 Gunpowder; craft 250 Polymer. `configured`
47. **Armoury Support** — Gather 5,000 Element; craft 250 Electronics; craft 2,000 Gunpowder; craft 500 Cementing Paste. `configured`
48. **Chemical Stores** — Gather 10,000 resources in any combination: Rare Flowers, or Rare Mushrooms; craft 5,000 Sparkpowder; craft 250 Stimulants. `configured`
49. **Sedation Works** — Gather 10,000 resources in any combination: Rare Flowers, or Rare Mushrooms; craft 5,000 Sparkpowder; craft 500 Narcotics. `configured`
50. **General Production** — Gather 5,000 Black Pearls; craft 1,000 Gunpowder; craft 1,000 Cementing Paste; craft 200 Electronics; craft 200 Polymer. `configured`

[Back to top](#top)

</details>

<a id="weekly-weapons-and-tools"></a>
<details>
<summary><strong>🛠️ Weapons and tools (15)</strong></summary>

Requires **1 daily completion** plus all listed objectives. **Reward: 25,000 Gold Nuggets each.**

51. **Bowstring Kit** — Gather 50,000 resources in any combination: Wood, Fungal Wood, Thatch, or Fibre; craft 2 Bows; craft 500 Stone Arrows. `configured`
52. **Crossbow Kit** — Gather 50,000 resources in any combination: Wood, Fungal Wood, Thatch, or Fibre; craft 1 Crossbow; craft 500 Stone Arrows. `configured`
53. **Tranquilizer Kit** — Gather 50,000 resources in any combination: Fibre, Wood, Fungal Wood, Thatch, or Hide; craft 1 Crossbow; craft 250 Tranq Arrows. `configured`
54. **Longneck Kit** — Gather 50,000 resources in any combination: Metal Ore, Wood, Fungal Wood, or Hide; craft 1 Longneck Rifle; craft 100 Tranquilizer Darts. `configured`
55. **Sidearm Kit** — Gather 50,000 resources in any combination: Metal Ore, Wood, Fungal Wood, or Hide; craft 1 Simple Pistol; craft 200 Simple Bullets. `configured`
56. **Shotgun Kit** — Gather 50,000 resources in any combination: Metal Ore, Wood, Fungal Wood, or Hide; craft 1 Shotgun; craft 150 Shotgun Shells. `configured`
57. **Pump-Action Kit** — Gather 50,000 resources in any combination: Metal Ore, Wood, Fungal Wood, or Hide; craft 1 Pump-Action Shotgun; craft 150 Shotgun Shells. `configured`
58. **Assault Kit** — Gather 10,000 resources in any combination: Crystal, Obsidian, Oil, or Silica Pearls; craft 1 Assault Rifle; craft 500 Advanced Rifle Bullets. `configured`
59. **Fabricated Sidearm** — Gather 10,000 resources in any combination: Crystal, Obsidian, or Silica Pearls; craft 1 Fabricated Pistol; craft 250 Advanced Bullets. `configured`
60. **Compound Kit** — Gather 10,000 resources in any combination: Crystal, Obsidian, or Silica Pearls; craft 1 Compound Bow; craft 150 Metal Arrows. `configured`
61. **Precision Kit** — Gather 10,000 resources in any combination: Crystal, Obsidian, Oil, or Silica Pearls; craft 1 Fabricated Sniper Rifle; craft 100 Advanced Sniper Bullets. `configured`
62. **Close Quarters** — Gather 50,000 resources in any combination: Hide, Fibre, Wood, or Fungal Wood; craft 1 Pike; craft 1 Sword; craft 50 Medical Brews. `configured`
63. **Harvesting Kit** — Gather 50,000 resources in any combination: Wood, Fungal Wood, Stone, or Metal Ore; craft 1 Metal Pick; craft 1 Metal Hatchet; craft 500 Cementing Paste. `configured`
64. **Fibre Kit** — Gather 50,000 resources in any combination: Hide, Fibre, Wood, or Fungal Wood; craft 1 Metal Sickle; craft 250 Stimulants. `configured`
65. **Field Bow Pair** — Gather 50,000 resources in any combination: Wood, Fungal Wood, Thatch, or Fibre; craft 1 Bow; craft 1 Crossbow; craft 500 Stone Arrows. `configured`

[Back to top](#top)

</details>

<a id="weekly-saddles"></a>
<details>
<summary><strong>🦕 Saddles (15)</strong></summary>

Requires **1 daily completion** plus all listed objectives. **Reward: 25,000 Gold Nuggets each.**

66. **Raptor Outfitter** — Gather 50,000 resources in any combination: Hide, Fibre, Wood, or Fungal Wood; craft 2 Raptor Saddles; craft 250 Tranq Arrows. `configured`
67. **Parasaur Outfitter** — Gather 50,000 resources in any combination: Hide, Fibre, Wood, or Fungal Wood; craft 2 Parasaur Saddles; craft 500 Narcotics. `configured`
68. **Trike Outfitter** — Gather 50,000 resources in any combination: Hide, Fibre, Wood, or Fungal Wood; craft 1 Trike Saddle; craft 500 Narcotics. `configured`
69. **Stego Outfitter** — Gather 50,000 resources in any combination: Hide, Fibre, Wood, or Fungal Wood; craft 1 Stego Saddle; craft 250 Tranq Arrows. `configured`
70. **Ankylo Outfitter** — Gather 50,000 resources in any combination: Wood, Fungal Wood, Stone, or Metal Ore; craft 1 Ankylo Saddle; craft 500 Cementing Paste. `configured`
71. **Doedicurus Outfitter** — Gather 10,000 resources in any combination: Chitin, or Keratin; craft 1 Doedicurus Saddle; craft 1,000 Sparkpowder. `configured`
72. **Castoroides Outfitter** — Gather 50,000 resources in any combination: Wood, Fungal Wood, Stone, or Metal Ore; craft 1 Castoroides Saddle; craft 500 Cementing Paste. `configured`
73. **Argentavis Outfitter** — Gather 50,000 resources in any combination: Hide, Fibre, Wood, or Fungal Wood; craft 1 Argentavis Saddle; craft 250 Tranq Arrows. `configured`
74. **Pteranodon Outfitter** — Gather 50,000 resources in any combination: Hide, Fibre, Wood, or Fungal Wood; craft 1 Pteranodon Saddle; craft 250 Narcotics. `configured`
75. **Rex Outfitter** — Gather 10,000 resources in any combination: Chitin, Keratin, or Organic Polymer; craft 1 Rex Saddle; craft 500 Narcotics. `configured`
76. **Therizinosaurus Outfitter** — Gather 10,000 resources in any combination: Chitin, Keratin, or Organic Polymer; craft 1 Therizinosaurus Saddle; craft 500 Narcotics. `configured`
77. **Iguanodon Outfitter** — Gather 50,000 resources in any combination: Hide, Fibre, Wood, or Fungal Wood; craft 2 Iguanodon Saddles; craft 250 Tranq Arrows. `configured`
78. **Baryonyx Outfitter** — Gather 50,000 resources in any combination: Hide, Fibre, Wood, or Fungal Wood; craft 1 Baryonyx Saddle; craft 100 Medical Brews. `configured`
79. **Sarco Outfitter** — Gather 50,000 resources in any combination: Hide, Fibre, Wood, or Fungal Wood; craft 1 Sarco Saddle; craft 100 Medical Brews. `configured`
80. **Utility Saddle Pair** — Gather 50,000 resources in any combination: Wood, Fungal Wood, Stone, or Metal Ore; craft 1 Ankylo Saddle; craft 1 Doedicurus Saddle; craft 500 Cementing Paste. `configured`

[Back to top](#top)

</details>

<a id="weekly-clothing"></a>
<details>
<summary><strong>🧵 Clothing (20)</strong></summary>

Requires **1 daily completion** plus all listed objectives. **Reward: 25,000 Gold Nuggets each.**

81. **Cloth Wardrobe** — Gather 50,000 resources in any combination: Hide, Fibre, Wood, or Fungal Wood; craft one full Cloth set: 1 headpiece, 1 chestpiece, 1 pair of gloves, 1 pair of leggings, and 1 pair of boots. `configured`
82. **Cloth Field Set** — Gather 50,000 resources in any combination: Hide, Fibre, Wood, or Fungal Wood; craft one full Cloth set: 1 headpiece, 1 chestpiece, 1 pair of gloves, 1 pair of leggings, and 1 pair of boots; craft 50 Medical Brews. `configured`
83. **Cloth Taming Set** — Gather 50,000 resources in any combination: Hide, Fibre, Wood, or Fungal Wood; craft one full Cloth set: 1 headpiece, 1 chestpiece, 1 pair of gloves, 1 pair of leggings, and 1 pair of boots; craft 250 Tranq Arrows. `configured`
84. **Cloth Workshop Set** — Gather 50,000 resources in any combination: Hide, Fibre, Wood, or Fungal Wood; craft one full Cloth set: 1 headpiece, 1 chestpiece, 1 pair of gloves, 1 pair of leggings, and 1 pair of boots; craft 500 Cementing Paste. `configured`
85. **Hide Wardrobe** — Gather 50,000 resources in any combination: Hide, Fibre, Wood, or Fungal Wood; craft one full Hide set: 1 headpiece, 1 chestpiece, 1 pair of gloves, 1 pair of leggings, and 1 pair of boots. `configured`
86. **Hide Field Set** — Gather 50,000 resources in any combination: Hide, Fibre, Wood, or Fungal Wood; craft one full Hide set: 1 headpiece, 1 chestpiece, 1 pair of gloves, 1 pair of leggings, and 1 pair of boots; craft 50 Medical Brews. `configured`
87. **Hide Taming Set** — Gather 50,000 resources in any combination: Hide, Fibre, Wood, or Fungal Wood; craft one full Hide set: 1 headpiece, 1 chestpiece, 1 pair of gloves, 1 pair of leggings, and 1 pair of boots; craft 250 Tranq Arrows. `configured`
88. **Hide Workshop Set** — Gather 50,000 resources in any combination: Hide, Fibre, Wood, or Fungal Wood; craft one full Hide set: 1 headpiece, 1 chestpiece, 1 pair of gloves, 1 pair of leggings, and 1 pair of boots; craft 500 Cementing Paste. `configured`
89. **Chitin Wardrobe** — Gather 10,000 resources in any combination: Chitin, or Keratin; craft one full Chitin set: 1 headpiece, 1 chestpiece, 1 pair of gloves, 1 pair of leggings, and 1 pair of boots. `configured`
90. **Chitin Field Set** — Gather 10,000 resources in any combination: Chitin, or Keratin; craft one full Chitin set: 1 headpiece, 1 chestpiece, 1 pair of gloves, 1 pair of leggings, and 1 pair of boots; craft 50 Medical Brews. `configured`
91. **Chitin Taming Set** — Gather 10,000 resources in any combination: Chitin, or Keratin; craft one full Chitin set: 1 headpiece, 1 chestpiece, 1 pair of gloves, 1 pair of leggings, and 1 pair of boots; craft 250 Tranq Arrows. `configured`
92. **Chitin Workshop Set** — Gather 10,000 resources in any combination: Chitin, or Keratin; craft one full Chitin set: 1 headpiece, 1 chestpiece, 1 pair of gloves, 1 pair of leggings, and 1 pair of boots; craft 500 Cementing Paste. `configured`
93. **Flak Wardrobe** — Gather 10,000 resources in any combination: Crystal, Obsidian, or Silica Pearls; craft one full Flak set: 1 headpiece, 1 chestpiece, 1 pair of gloves, 1 pair of leggings, and 1 pair of boots. `configured`
94. **Flak Field Set** — Gather 10,000 resources in any combination: Crystal, Obsidian, or Silica Pearls; craft one full Flak set: 1 headpiece, 1 chestpiece, 1 pair of gloves, 1 pair of leggings, and 1 pair of boots; craft 50 Medical Brews. `configured`
95. **Flak Taming Set** — Gather 10,000 resources in any combination: Crystal, Obsidian, or Silica Pearls; craft one full Flak set: 1 headpiece, 1 chestpiece, 1 pair of gloves, 1 pair of leggings, and 1 pair of boots; craft 250 Tranq Arrows. `configured`
96. **Flak Workshop Set** — Gather 10,000 resources in any combination: Crystal, Obsidian, or Silica Pearls; craft one full Flak set: 1 headpiece, 1 chestpiece, 1 pair of gloves, 1 pair of leggings, and 1 pair of boots; craft 500 Cementing Paste. `configured`
97. **Fur Wardrobe** — Gather 10,000 Pelt; craft one full Fur set: 1 headpiece, 1 chestpiece, 1 pair of gloves, 1 pair of leggings, and 1 pair of boots. `configured`
98. **Fur Field Set** — Gather 10,000 Pelt; craft one full Fur set: 1 headpiece, 1 chestpiece, 1 pair of gloves, 1 pair of leggings, and 1 pair of boots; craft 50 Medical Brews. `configured`
99. **Fur Taming Set** — Gather 10,000 Pelt; craft one full Fur set: 1 headpiece, 1 chestpiece, 1 pair of gloves, 1 pair of leggings, and 1 pair of boots; craft 250 Tranq Arrows. `configured`
100. **Fur Workshop Set** — Gather 10,000 Pelt; craft one full Fur set: 1 headpiece, 1 chestpiece, 1 pair of gloves, 1 pair of leggings, and 1 pair of boots; craft 500 Cementing Paste. `configured`

[Back to top](#top)

</details>
## Configuration checks

- All **347 current quests** have been checked for missing counter references, empty referenced target lists and malformed blueprint-reference syntax.
- All **100 weekly descriptions** match their configured gathering totals, crafting targets and amounts. Clothing slot requirements, gear limits, daily-completion requirements and rewards were checked.
- Grouped gathering counters have short labels; crafting counters name their items. The latest label pass changed only display names in the config.
- Missing legacy tame targets and malformed tracking references were repaired earlier in the rework. Permanent quest balancing remains pending.
- The daily pool and permanent quest definitions were preserved during the weekly rebuild. Weekly IDs from superseded pools were not reused for new objectives.
- These are **static configuration checks**, not proof of in-game completion or installed asset availability.

<a id="before-adding-these-to-the-live-rotation"></a>
## Testing and rollout

- [x] Configure all **121 dailies** and **100 progression weeklies**.
- [x] Set fixed rewards: **5,000 daily / 25,000 weekly**, with no extras.
- [x] Configure weekly resource tiers: **50,000 / 10,000 / 5,000**.
- [x] Require exactly **1 daily completion** on every weekly.
- [x] Exclude hunting and structures from weekly objectives.
- [x] Cap weekly equipment at 1–2 items and clothing at one full matching set.
- [x] Include the supplied EVO variants in the relevant daily groups.
- [x] Review counter labels and verify the current quest references.
- [x] Observe **Rifle Workshop** and **Supply and Survive** loading and displaying in-game.
- [x] Remove **Reset Dailies** from the prepared shop config.
- [ ] Verify daily-completion credit inside a weekly and progress across a daily reset.
- [ ] Verify grouped gathering and crafting credit through the actual vanilla and modded stations.
- [ ] Verify Medical Brew cooking, each clothing slot and weapon/saddle crafting.
- [ ] Verify actual Element and Black Pearl credit through the acquisition methods used on the servers. Loot, crafting/conversion, purchases and transfers must not be assumed to count as harvesting.
- [ ] Verify daily hunting, EVO variants and the repaired legacy objectives in-game.
- [ ] Confirm completed quests pay exactly **5,000 daily / 25,000 weekly**.
- [ ] Check actual creature spawns, resources, engrams and recipes on every cluster map.
- [ ] Review difficult daily targets, including **25,000 Keratin** and **3,000 Black Pearls**, based on observed completion time.
- [ ] Confirm **Reset Dailies** is removed from the live store.
- [ ] Confirm cluster-wide rollout and handling of existing assignments at the normal reset.
- [ ] Complete the permanent quest balance review, then revisit the wider economy if needed.

Changing objectives can interrupt active progress. Back up the quest database, announce pool changes and schedule them for the normal reset. The latest counter-label-only revision changes no quest IDs, tracking keys or requirements.

## Current status

**121 dailies and 100 weeklies are configured.** Two weekly quest screens have been observed in-game. Tracking, payouts, reset behaviour, map coverage and final balance still need validation. Cluster-wide live rollout remains unconfirmed.

---
## Credits

- **!azaleaa** — Quest planning, rework and coordination.
- **SammyWammyM8** — Quest feedback, creature selection and balancing suggestions.

<p align="center">
  <strong>Lusty Looters</strong><br>
  A harder, but rewarding Ark experience.
</p>
