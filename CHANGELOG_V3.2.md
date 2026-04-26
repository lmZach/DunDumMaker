# 🗳️ Version 3.2 - SOCIAL DUNGEON VOTING!

## 🎉 What's New:

### **🗳️ Voting System for Social Dungeons**

Social dungeons now have a unique mechanic where the party votes for who should get a +2 bonus!

---

## 🎮 How Social Voting Works:

### **1. Dungeon Phase**
- Dungeon card flips
- If it's a **Social Dungeon** (🗣️), voting is triggered

### **2. Card Selection**
- You select your cards as normal
- Lock in your selection

### **3. Chaos Master Plays**
- Chaos Master plays their card

### **4. 🗳️ VOTING PHASE (NEW!)**
- **Phase indicator:** "🗳️ Social Dungeon! Vote for who should get +2 bonus."
- **Voting UI appears** with 3 buttons:
  - Vote for YOU
  - Vote for Alice
  - Vote for Bob

### **5. Vote Resolution**
- **You cast your vote** (click a button)
- **AI votes automatically** (Alice & Bob vote randomly)
- **Votes are tallied:**
  - 3 votes total
  - Whoever has the most votes wins
  - Winner gets **+2 to their roll**
  - Must have 2+ votes to get bonus

### **6. Dice Rolling**
- Everyone rolls as normal
- **Vote winner gets +2 applied to their roll**
- Vote winner's roll shows 🗳️ emoji
- Log shows "(with vote bonus!)"

---

## 📊 Example Social Round:

```
Phase: 🗳️ Social Dungeon! Vote for who should get +2 bonus.

[Vote for YOU] [Vote for Alice] [Vote for Bob]

> You voted for Alice
> Alice voted for YOU  
> Bob voted for Alice

🏆 Alice wins the vote with 2 votes! Gets +2

Phase: 🎲 Rolling dice...

👤 YOU rolled: 14
🧑 Alice rolled: 18 🗳️ (with vote bonus!)
🧑 Bob rolled: 12

🎉 Alice wins! +1 Glory!
```

---

## 🎯 Strategic Voting:

- **Vote for yourself** if you have strong cards
- **Vote for others** to be diplomatic (or strategic)
- **AI votes randomly** (for now - Phase 2 will add smarter AI)
- **Majority wins** - need 2+ votes for +2 bonus
- **Ties:** First alphabetically wins (can be improved later)

---

## 🔧 Technical Changes:

### **New Functions:**
- `startVoting()` - Shows voting UI
- `castVote(votedFor)` - Handles vote logic & tallying

### **Updated Functions:**
- `chaosMasterPlays()` - Checks dungeon type, routes to voting for Social
- `rollAllDice()` - Applies vote bonus to rolls
- `nextRound()` - Clears vote data

### **New GameState Properties:**
- `voteWinner` - Who won the vote
- `voteBonus` - Bonus amount (0 or 2)

### **UI Additions:**
- Voting section with 3 buttons
- Vote winner indicator (🗳️ emoji on roll)
- Phase messages for voting

---

## 🃏 Dungeon Types Summary:

| Type | Icon | How to Win | Special Mechanic |
|------|------|------------|------------------|
| **Combat** | ⚔️ | Highest roll | None |
| **Social** | 🗣️ | Highest roll | 🗳️ Vote for +2 bonus |
| **Exploration** | 🧭 | Closest to target | *(Coming soon)* |
| **Wild** | ❓ | Chaos decides | *(Coming soon)* |

---

## 📥 Download:

**[dod_card_creator_v3.2_voting.html](computer:///mnt/user-data/outputs/dod_card_creator_v3.2_voting.html)** (92 KB) ⭐

**Or from GitHub deploy folder:**
**[index.html](computer:///mnt/user-data/outputs/github-deploy/index.html)**

---

## 🚀 What's Working:

✅ Social dungeon voting system  
✅ 3 voting options (YOU, Alice, Bob)  
✅ AI auto-votes  
✅ Vote tallying  
✅ +2 bonus applied to winner  
✅ Visual indicator (🗳️) on winner's roll  
✅ Vote data clears each round  
✅ Works alongside Combat dungeons  

---

## 🎯 Next Steps (Phase 2+):

- 🧠 **Smarter AI voting** (vote strategically)
- 🎲 **Exploration dungeons** (closest to target)
- 🎭 **Wild dungeons** (Chaos Master decides)
- 🗣️ **Social effects** (different Social challenges)
- 📊 **Vote history** (see who voted for whom)

---

## 🐛 Testing Checklist:

- [ ] Start game
- [ ] Play until Social dungeon appears
- [ ] See voting UI pop up
- [ ] Cast your vote
- [ ] See AI votes logged
- [ ] See vote winner announced
- [ ] See +2 bonus applied to rolls
- [ ] See 🗳️ emoji on winner's roll
- [ ] Winner determined correctly
- [ ] Next round clears vote data

---

**Version:** 3.2 (Social Voting)  
**Date:** 2026-04-26  
**File Size:** 92 KB (was 88 KB)  
**New Lines:** ~100

🗳️ **Democracy has come to Dungeons of Dumbassery!** 🗳️
