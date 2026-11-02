<a id="top"></a>

<p align="center">
  <img src="https://i.imgur.com/hSLVhdU.png" alt="Lusty Looters logo" width="180">
</p>

<h1 align="center">Lusty Looters — Daily Quest Rework</h1>

<p align="center">
  Daily quests are the first step in a wider quest and economy review. Weekly and permanent quests will be reviewed next, and shop pricing and the wider Gold Nugget economy may be adjusted afterwards.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Total%20Quests-121-8b5cf6?style=for-the-badge" alt="121 total quests">
  <img src="https://img.shields.io/badge/Configured-121-22c55e?style=for-the-badge" alt="121 quests configured">
  <img src="https://img.shields.io/badge/Status-Awaiting%20Server%20Testing-f59e0b?style=for-the-badge" alt="awaiting server testing">
  <img src="https://img.shields.io/badge/Live%20Rollout-Unconfirmed-3b82f6?style=for-the-badge" alt="live rollout unconfirmed">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Daily%20Quest%20Reward-5%2C000%20Gold%20Nuggets-eab308?style=for-the-badge" alt="5000 Gold Nuggets per quest">
</p>

> [!IMPORTANT]
> **All 121 daily quests are now configured. Live rollout has not been confirmed.** Every daily is set to pay **5,000 Gold Nuggets**, with no additional item rewards. The config has passed static reference checks, but in-game tracking, payouts and availability on every map still need testing. **Weekly and permanent quest balancing remains a later phase**, followed by a possible review of shop prices and the wider Gold Nugget economy. The 5,000-Nugget daily reward is not a final economy balance.

> [!NOTE]
> The goal with this rework is simple: make dailies feel better, cover more playstyles, and be **doable on any map without needing to transfer**.

> [!WARNING]
> The creature groups are configured for the intended cross-map design, but they have **not been verified against the live spawn tables** on every Lusty Looters map. A valid blueprint reference does not prove that a qualifying creature spawns on a particular map.

## Quick links

- [Overview](#overview)
- [Rewards and store changes](#rewards-and-store-changes)
- [Variant support](#variant-support)
- [Configuration fixes](#configuration-fixes)
- [Quest list](#quest-list)
  - [Biome hunts](#biome-hunts)
  - [Creature hunts](#creature-hunts)
  - [Creature class hunts](#creature-class-hunts)
  - [Gathering](#gathering)
  - [Crafting](#crafting)
  - [Special & mixed](#special--mixed)
- [Before adding these to the live rotation](#before-adding-these-to-the-live-rotation)
- [Credits](#credits)

## Overview

### Progress

Updated **2 November 2026**.

| Configuration status | Count |
| :-- | --: |
| Existing dailies retained or reworked | 18 |
| New dailies added | 103 |
| **Daily quests configured** | **121** |

The previous pool contained 31 dailies: 18 were retained or reworked, 13 were retired, and 103 new quests were added. The 18 retained quests include the 11 planned objective reworks and 7 quests whose objectives were kept. Every daily now uses the same 5,000-Nugget reward.

### Status tags

- `configured` — included in the prepared JSON, with its required counters and reward set.
- Configured does **not** mean tested in-game or confirmed live. Server validation and rollout are tracked below.

### How grouped kills work

Alternative creatures within one objective share **one kill counter**. Mixed quests that require two objectives keep separate counters for each required group or activity.

Example:

- `20 kills: Sarco, Kaprosuchus or Piranha`
- This means **20 kills total**, in any combination.

### Rewards and store changes

> [!TIP]
> **Every daily is configured to award 5,000 Gold Nuggets.** The reward is the same regardless of its category or requirements, and previous extra item rewards have been removed from the daily pool.

- **Daily quest reward:** 5,000 Gold Nuggets each.
- **Store:** The **Reset Dailies** product has been removed from the prepared shop config. Its removal from the live store still needs confirming.
- **Other shop settings:** Existing prices, previous product removals and the reduced Red Gem selling rule are unchanged by this quest update.
- **Next up:** Weekly quests, followed by permanent quests. Their requirements and rewards have not been rebalanced in this phase.
- **Later:** Shop pricing and the wider economy may be adjusted after those reviews. No wider economy changes are confirmed here.
- **Rollout:** Configuration work is complete; deployment and in-game results are not confirmed.

### Variant support

The supplied **12 EVO blueprint paths** have been added to the matching daily hunt groups. Supported catalogue and map variants are included where they match the objective.

| EVO group | Included variants |
| :-- | :-- |
| Rex / Tarbo | Tarbo, Paleo Rex, Legacy Rex, Volcano Rex and Tek Rex |
| Alpha Rex / Tarbo | Alpha Tarbo, Alpha Rex and Alpha Legacy Rex |
| Giganotosaurus | EVO Giga, Paleo Giga, Volcano Giga and Wasteland Giga |

- Ordinary Rex hunts also accept the configured Alpha Rex/Tarbo variants.
- Alpha objectives count qualifying Alphas; ordinary Rex or Giga variants do not satisfy an Alpha objective.
- Variants in a grouped objective contribute to the same required total. They are not separate kill requirements.
- Actual spawning and kill credit for these classes still need checking on the live servers.

### Configuration fixes

- Added separate daily tracking groups so changing the daily pool does not redefine the existing weekly or permanent counters.
- Standardised wording, punctuation, number formatting and stat labels across old and new quests while retaining their existing names and themes.
- Filled the missing targets for **Astrocetus Tamer**, **Megachelon Tamer** and **Parrot Tamer**.
- Corrected malformed references used by **Surface Reaper Vanquisher**, **Electronics Batch**, **Bullet Barrage**, **Maeguana Tamer**, **System Shutdown** and **Wrath of the Boar Kings**.
- Cleaned up matching quote errors and duplicate references elsewhere in the tracking lists.
- All **264 current quests** pass static checks for missing trackers, empty referenced targets and malformed blueprint-reference syntax. This is not an in-game completion test.
- Legacy fixes preserve quest IDs, required amounts, rewards, permissions and progression links. Weekly and permanent balance reviews are still pending.

### Daily quest rules

- No taming objectives.
- Biome hunts use **20 kills each**.
- Grouped quests include the configured eligible variants for their targets.
- The main aim is **playable on every map**, not perfect biome realism.

## Quest list

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

## Before adding these to the live rotation

- [x] Build all **121 daily quests** in the JSON.
- [x] Set every daily reward to exactly **5,000 Gold Nuggets**, with no extra items.
- [x] Configure shared counters for grouped alternatives and separate counters for mixed requirements.
- [x] Add the **12 supplied EVO paths** to the relevant daily groups.
- [x] Repair the identified legacy tracker defects and validate the current quest references.
- [x] Apply consistent wording and stat labels across old and new quests.
- [x] Remove **Reset Dailies** from the prepared shop config.
- [ ] Load the config on a test server and restart the map for the new custom tracking stats.
- [ ] Check kill, gather and craft credit in-game, including Fungal Wood, mixed resource groups and normal/remapped crafting stations.
- [ ] Check EVO Rex, Giga and Alpha kill credit, the three repaired taming objectives, and the corrected legacy boss objectives.
- [ ] Confirm that completing a daily pays exactly **5,000 Gold Nuggets**.
- [ ] Check every creature group against the **actual live spawn tables** on each cluster map.
- [ ] Confirm qualifying Alpha availability on every map; revise or restrict objectives where necessary.
- [ ] Revisit grind-heavy requirements such as **25,000 Keratin** and **3,000 Black Pearls**.
- [ ] Confirm **Reset Dailies** is removed from the live store.
- [ ] Confirm the updated pool is deployed and old daily assignments are handled at the daily reset or through the supported reassignment process.
- [ ] Review weekly quests, then permanent quests, as separate balance phases.
- [ ] Reassess shop prices and the wider economy afterwards if needed.

## Current status

This page now describes the **prepared 121-quest configuration**. Every listed daily is configured, and the supporting reference checks are complete. In-game behaviour, map coverage, economy balance and live rollout remain unconfirmed until the checks above are completed.

---

## Credits

- **!azaleaa** — Quest planning, rework and coordination.
- **SammyWammyM8** — Quest feedback, creature selection and balancing suggestions.

<p align="center">
  <strong>Lusty Looters</strong><br>
  A harder, but rewarding Ark experience.
</p>
