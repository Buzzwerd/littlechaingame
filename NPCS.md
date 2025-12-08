# NPCs - Chain Game v0.47

Complete guide to all NPCs in the game, their locations, and what they offer.

## NPC Interaction
- Walk near an NPC to start dialogue
- Navigate dialogue with Left/Right arrows
- Accept/decline offers with Up (yes) / Down (no)
- Some NPCs require coins - pay by depositing coins while they're collecting

---

## Starting Area NPCs

### Tim
**Location:** (150, 150) - Southeast of post
**Type:** Tutorial / Work Tools Provider

Tim is the first NPC you'll encounter. He teaches you the drop mechanic and gives your first ability.

| Offers | Cost | Effect |
|--------|------|--------|
| Small Bag +1 Capacity | Free | +1 carry capacity |
| Work Tools | Free* | Required for jobs |

*Work Tools given when you return after accepting a job from Wheaton or Weadon.

**Key Dialogue:** "Press Left and Right arrows at the same time to drop the last item you picked up."

---

### Gary
**Location:** (-150, 200) - Southwest of post
**Type:** Lore NPC

Gary doesn't offer any items - he just complains about dropping his coins. Purely for world-building.

---

### Wes
**Location:** (150, -250) - Northeast of post
**Type:** Diamond Giver

| Offers | Cost | Effect |
|--------|------|--------|
| Diamond | Free | Heavy item worth more |

**Choice Required:** Up for yes, Down for no

---

### Chris
**Location:** (350, 250) - East of post
**Type:** Ability Giver

| Offers | Cost | Effect |
|--------|------|--------|
| Carry Capacity +10 | Free | +10 carry capacity |

---

## Mid-Range NPCs

### Sam
**Location:** (-300, -450) - Northwest
**Type:** Ability Seller

| Offers | Cost | Effect |
|--------|------|--------|
| Speed Boost | 3 coins | +40% movement speed |

**Choice Required:** Up for yes, Down for no

---

### Zoe
**Location:** (-500, 500) - Southwest
**Type:** Ability Seller

| Offers | Cost | Effect |
|--------|------|--------|
| Zoom Out 20% | 3 coins | +20% zoom out |

**Choice Required:** Up for yes, Down for no

---

### Ron
**Location:** (-600, -350) - West-Northwest
**Type:** Ability Seller

| Offers | Cost | Effect |
|--------|------|--------|
| Turbo Speed +50% | 5 coins | +50% movement speed |

**Personality:** Very enthusiastic about SPEED!

**Choice Required:** Up for yes, Down for no

---

### Bob
**Location:** (4, 550) - South of post
**Type:** Ability Seller

| Offers | Cost | Effect |
|--------|------|--------|
| Carry Penalty -50% | 3 coins | -50% carry speed penalty |

**Choice Required:** Up for yes, Down for no

---

### Eddie
**Location:** (550, -200) - East
**Type:** Ability Seller

| Offers | Cost | Effect |
|--------|------|--------|
| Carry Speed Bonus +30% | 6 coins | +30% speed when carrying |

**Tip:** Eddie tells you that the game saves whenever you deposit something.

**Choice Required:** Up for yes, Down for no

---

### Hank
**Location:** (700, -850) - Far Northeast
**Type:** Ability Giver

| Offers | Cost | Effect |
|--------|------|--------|
| Carry Capacity +15 | Free | +15 carry capacity |

**Personality:** Former hoarder who's "downsizing."

---

## Music Disk NPCs

### George
**Location:** (0, -1000) - North
**Type:** Music Disk Giver

| Offers | Cost | Tracks |
|--------|------|--------|
| Chill Tune Disk | Free | 1 track |

**Tip:** Teaches you can hold Up+Down to change disks.

---

### Fritz
**Location:** (2000, 100) - Far East
**Type:** Music Disk Seller

| Offers | Cost | Tracks |
|--------|------|--------|
| Going Places | 3 coins | 2 tracks (suncity, highlife) |

**Choice Required:** Up for yes, Down for no

---

### Jawn
**Location:** (-2000, -600) - Far West
**Type:** Music Disk Seller

| Offers | Cost | Tracks |
|--------|------|--------|
| GAMBLIN MAN | 3 coins | 1 track |

**Choice Required:** Up for yes, Down for no

---

### Klaus
**Location:** (4500, -60) - Very Far East
**Type:** Music Disk Giver (Conditional)

| Offers | Cost | Tracks |
|--------|------|--------|
| Cache Full Disk | Free* | 9 tracks |

*Requires helping Pin first. Klaus won't give you the disk until Pin has made progress on their chain.

---

### Noodles
**Location:** (-4500, -4060) - Very Far Southwest
**Type:** Music Disk Giver (Conditional)

| Offers | Cost | Tracks |
|--------|------|--------|
| BUDSbeats | Free* | 12 tracks |

*Requires a very long chain. Noodles won't give you the disk until your chain is "getting ready to come off."

**Personality:** Sarcastic, but respects dedication.

---

## Special NPCs

### Straum
**Location:** (1000, 1000) - Southeast
**Type:** Coin/Diamond Giver

Straum has collected 99 coins from someone who dropped them. He'll give you coins up to your carry capacity each time you visit.

| Offers | Cost | Effect |
|--------|------|--------|
| Coins (up to capacity) | Free | Multiple coins per visit |
| Diamond | Free | After coins run out |

**Note:** Straum notices if you've dropped coins yourself.

**Choice Required:** Up for yes, Down for no

---

### Pin
**Location:** (3033, -49) - Far East
**Type:** Chained NPC

Pin is unique - they have their own chain attached to their own post. Pin's post has no nearby coins, so they need help.

**Mechanic:** Drop coins near Pin's post, and Pin will collect them to grow their chain.

| Pin's Chain Length | Dialogue |
|-------------------|----------|
| 10 links | "Look how long my chain is getting!" |
| 20 links | "I can't believe I'll finally get out into the world." |
| 50 links | "At this rate, I'll be as long as you soon!" |
| 100 links | Gives you a diamond |

**Unlocks:** Helping Pin unlocks Klaus's disk.

---

### Brot
**Location:** (-4600, 3400) - Very Far Southwest
**Type:** Chained NPC (Animal Collector)

Brot has a massive 500-link chain but is tired of collecting coins. He just wants pets. His post is located at (2400, -2600), so you can see his chain stretching across the map.

**Mechanic:** Lead animals from the farm into Brot's 800px zone (marked by dense grass). Once animals enter the zone, they stay permanently and wander around Brot.

| Animals Brought | Dialogue |
|-----------------|----------|
| 1 animal | "Wait... is that... an animal?!" (Joyous) |
| 5 animals | "Five little friends!" |
| 10 animals | "Ten animals! TEN!" |
| 25 animals | "Twenty-five?! You're kidding me." (Disbelief) |
| 50 animals | Gives you the **Golden Fleece** |

**Golden Fleece:** A heavy item worth 100 coins (weighs 100).

**After Quest:** Brot resumes collecting dropped coins like Pin.

**Note:** Animals entering Brot's zone take priority over Wheaton's animal retrieval job.

---

### Clint
**Location:** (5000, 400) - Very Far East
**Type:** Follower NPC

Clint is lonely and existentially distressed. If you accept, he follows you around.

| Offers | Cost | Effect |
|--------|------|--------|
| Companionship | Free | Clint follows you |

**Personality:** Melancholic, grateful if accepted.

**Choice Required:** Up for yes, Down for no

---

## Job NPCs

### Chaff
**Location:** (200, -2500) - Far North
**Type:** Information NPC

Chaff explains the job system and points you to the two job locations:
- **West:** Farm (Wheaton) - Animal Retrieval
- **East:** Courier Depot (Weadon) - Deliveries

---

### Wheaton
**Location:** (-2000, -2500) - Far Northwest
**Type:** Job Giver - Animal Retrieval

Offers the Animal Retriever job. Requires Work Tools from Tim.

**Job Details:**
- Retrieve scattered farm animals
- Animals follow you when you get close
- Bring them back to Wheaton
- New animals spawn at 18:00 daily
- Coins rewarded on delivery

**Choice Required:** Up for yes, Down for no

---

### Weadon
**Location:** (2100, -2400) - Far Northeast
**Type:** Job Giver - Courier

Offers the Courier job. Requires Work Tools from Tim.

**Job Details:**
- Receive packages to deliver
- Deliver to specified NPCs
- 3 deliveries per day maximum
- Time limit per delivery
- Coins rewarded on delivery

**Choice Required:** Up for yes, Down for no

---

## Far Outskirts NPCs

### Quincy
**Location:** (-2599, -2129) - Far West
**Type:** Ability Seller

| Offers | Cost | Effect |
|--------|------|--------|
| Max Fulfillment Coin | 15 coins | Speed boost when carrying 10+ weight |

**Personality:** Lonely, feels forgotten in the void.

**Choice Required:** Up for yes, Down for no

---

### Moe
**Location:** (3500, 3200) - Far Southeast
**Type:** Ability Seller

| Offers | Cost | Effect |
|--------|------|--------|
| Zoom Out 20% | 6 coins | +20% zoom out |

**Personality:** Philosophical about more and less.

**Choice Required:** Up for yes, Down for no

---

### Don
**Location:** (-3800, -3400) - Very Far West
**Type:** Ability Seller

| Offers | Cost | Effect |
|--------|------|--------|
| Turbo Speed +50% | 10 coins | +50% movement speed |

**Note:** Same effect as Ron's ability but costs twice as much. Don claims it's "premium."

**Choice Required:** Up for yes, Down for no

---

### Rob
**Location:** (-3200, 3800) - Far Southwest
**Type:** Ability Seller

| Offers | Cost | Effect |
|--------|------|--------|
| Carry Penalty -50% | 6 coins | -50% carry speed penalty |

**Note:** Same effect as Bob's ability but costs twice as much.

**Choice Required:** Up for yes, Down for no

---

## NPC Quick Reference Map

```
                     North
                       |
     Noodles          Chaff         Weadon
    (-4500,-4060)   (200,-2500)   (2100,-2400)
                       |
         Don        Wheaton      Brot's Post
      (-3800,-3400) (-2000,-2500) (2400,-2600)
                       |
       Quincy                      Hank
     (-2599,-2129)               (700,-850)
           |                        |
         Jawn        George       Eddie    Klaus      Pin      Clint
      (-2000,-600)   (0,-1000)  (550,-200) (4500,-60)(3033,-49)(5000,400)
           |            |           |         |
          Ron          Wes        Chris     Fritz
       (-600,-350)  (150,-250)  (350,250) (2000,100)
           |            |           |
         Gary         Tim          Bob      Straum
       (-150,200)   (150,150)    (4,550)  (1000,1000)
           |            |
          Zoe          |          Moe
       (-500,500)    POST       (3500,3200)
           |         (0,0)
          Rob                     Brot
      (-3200,3800)            (-4600,3400)
                       |
                     South
```

---

## Tips

1. **Start with Tim** - Get the drop mechanic tutorial and first capacity upgrade
2. **Visit free NPCs first** - Chris, Hank, George, and Wes give items for free
3. **Help Pin early** - Unlocks Klaus's 9-track disk
4. **Get Work Tools before jobs** - Accept a job, then visit Tim for tools
5. **Straum is a coin farm** - Visit repeatedly to get coins up to your capacity
6. **Check both sellers** - Some abilities are sold by multiple NPCs at different prices
7. **Help Brot for Golden Fleece** - Lead 50 animals to Brot's zone for a 100-coin reward
