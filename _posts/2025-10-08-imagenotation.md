---
layout: post
title: Image Notation: A New Mnemonic Code for Chess Moves
permalink: /imagenotation
---

*Note 8 October 2025: I drafted this article fairly quickly. In future I may expand it with diagrams and more explanation. The technique is also subject to change as my thinking develops -- [feedback welcome](/contact).*

Since I published [The Chess Memory Palace](https://amzn.to/4k7nXBO) in late 2022, I have received some great feedback. One reader has memorised over 1000 variations and almost 3000 unique move-pairs. An Amazon reviewer with fading eyesight says it has transformed her chess memory and helps with teaching classes. And two of the first three Amazon reviews even called it life changing![^2]

[^2]: 'Life changing' sounds over the top, but I suppose if you spend a significant amount of your time reviewing chess openings, then a more fun and effective method could indeed be life changing.

However, I have also heard some people struggle with [the original Picture Notation](/chessmemorypalace/chapter1), and would prefer a system that more closely matches algebraic notation. To this end, I have been working[^1] on a new mnemonic code, **Image Notation**, which keeps 1 word = 1 move (for the most part), but matches algebraic notation more closely. This article explains how it works.

Please [see here for a complete set of Image Notation picture words](/chessmemorypalace/picturewords), to use when building your memory palaces at home.

[^1]: Many thanks to Stephen Hensley, whose correspondence has sharpened my thinking on Image Notation, and has gone further with The Chess Memory Palace than anyone else I know, making fascinating developments in the practice of branching memory palaces.

### Identifying the piece

Every chess move is shown in one word (a 'picture word').
- If the picture word starts with an **s** sound (not *sh*), we have a **queen** move.
- If the picture word starts with a **b/p** sound, we have a **king** move.
- Otherwise, if the picture word has **1 syllable** (and doesn't start with s/b/p), we have a **pawn** move.
- If the picture word has **2 syllables** (and doesn't start with s/b/p), we have a **knight** move.
- If the picture word has **3 syllables** (and doesn't start with s/b/p), we have a **bishop** move.
- If the picture word has **4 syllables** (and doesn't start with s/b/p), we have a **rook** move.

### Identifying the target square
The **first consonant sound** of the picture word identifies the **file** of the target square. The **second consonant sound** of the picture word identifies the **rank** of the target square. Use the following conversion table:
 
| Consonant Sound         | If First (File) | If Second (Rank) |
|--------------------------|-----------------|------------------|
| d / t / th              | a-file          | 1st rank         |
| n                       | b-file          | 2nd rank         |
| m                       | c-file          | 3rd rank         |
| r                       | d-file          | 4th rank         |
| l                       | e-file          | 5th rank         |
| ch / j / tch / sh       | f-file          | 6th rank         |
| hard c / g / k / x      | g-file          | 7th rank         |
| f / v                   | h-file          | 8th rank         |
| soft c / s / z / b / p / h / w / y | *(no meaning, ignore)* | *(no meaning, ignore)* |


### Putting it together
So, every picture word identifies the piece to move, and the target square, just like algebraic notation.

Here are some easy examples:
- **shell** = Pf5. (I will use P to mean a pawn move.) The picture word doesn't start with an s/b/p sound, so we count the syllables. 1 syllable is a pawn move. First consonant sound is *sh*, giving the f-file, second consonant sound is *l*, giving the 5th rank.
- **leech** is Pe6. The picture word doesn't start with an s/b/p sound, so we count the syllables. 1 syllable is a pawn move. The first consonant sound is *l*, giving the e-file, second consonant sound is *ch*, giving the 6th rank.

Or in short:
- **dragon** = Na4 — 2 syllables → knight; d = a-file, r = 4th rank.
- **bottle** = Ka5 — starts with b → king; t = a-file, l = 5th rank.
- **daffodil** = Ba8 — 3 syllables → bishop; d = a-file, f = 8th rank.
- **saloon** = Qe2 — starts with s → queen; l = e-file, n = 2nd rank.
- **cheetah** = Nf1 — 2 syllables → knight; ch = f-file, t = 1st rank.
 
Here are some slightly trickier examples (but it should still be fairly easy):
- **cereal** is Qd5. The picture word starts with a soft c, which makes an *s* sound, so this is a queen move. The first two relevant consonant sounds are *r* and *l*, which mean the d-file and 5th rank, respectively.
- **chameleon** is Rg3. The picture word starts with a /k/ sound (despite being spelled 'ch'), so we count the number of syllables to identify the piece. There are 4 syllables, so this is a rook move. The first two consonant sounds are *k* and *m*, which gives the g-file and the 3rd rank, respectively.
 
Remember, we use sounds, not spelling. This is easier to do in your head at the board.

### Castling
There is no special notation for castling: it is just Kg1, Kc1, Kg8 or Kc8. e.g. **baguette** gives O-O (or Kg1). (Picture word starts with *b* = king move, first relevant consonant sound *g* = g-file, second relevant consonant sound *t* = 1st rank.)

### Captures, checks and promotions (no special notation)
There is no special notation for check, checkmate (or stalemate), or captures. e.g. Ne5+, Ne5# and Nxe5 are all notated **lily**. (2 syllable picture word = knight move, first consonant sound *l* = e-file, second consonant sound *l* = 5th rank.)

There is no special notation for promotion to a queen: it is just a pawn move to the 8th/1st rank. There *is* a special notation for underpromotion, but it will almost never come up, so I will not describe it here. Read [Chapter 1 of the original Picture Notation](/chessmemorypalace/chapter1) if you really want to know.

### Disambiguations -- simple solution
What if more than one of the same piece can move to the target square? This can happen when you have two knights or two rooks. It can also happen with two pawns, for a capture.

Barring promotions, which we won't worry about, it cannot happen with bishops (because they have opposite colours), nor kings and queens (because you only have one).

Algebraic notation deals with disambiguations by identifying the starting file of the piece to move, e.g. Rag1, or the starting rank if both pieces are on the same file, e.g. R1h7.

In Image Notation, we identify a 'piece 1' and a 'piece 2', starting from the back rank and breaking ties starting from the queenside. **For piece 1, the picture word does not change. For piece 2, we transform the image by imagining the picture word on fire.**

For example, if you have knights on g1 and c3 (so that e2 is the mutual target square), then the knight on g1 is 'piece 1' (because it's further back) and the knight on c3 is 'piece 2'. In this case, **lantern** is Nge2, as normal. (2 syllable picture word is a knight move, *l* is the e-file, *n* is the 2nd rank.) **Lantern on fire** is Nce2.

If you have rooks on a1 and a8, with nothing in between, then the rook on a1 is piece 1 and the rook on h1 is piece 2. (Because they are both on the same rank, so we break ties starting from the queenside.) **Caterpillar** is Rag1 (4 syllable word is a rook move, *c* gives the g-file, *t* gives the 1st rank). **Caterpillar on fire** is Rhg1.

### Disambiguations -- advanced solution
If you don't like transforming the images and instead want to keep 1 move = 1 picture word, it is possible. I plan to describe more fully in future. In short, notice there is a maximum of 14 moves you would ever need to disambiguate in a given position (2 knight moves, 6 rook moves, 6 pawn captures).

Label these using unique picture words 1-14 that don't already have a meaning, e.g. apple, bee, cow, dew, egg, eff, guy, hat, imp, jay, kip, owl, amp, nose. So e.g. *apple* always means 'move the second knight to the first mutual target square' (Ncd2 in the example above); *cow* always means 'move the second rook to the first mutual target square' (Rhb1 in the example above).

### Okay I understand Image Notation! Now what?
Convert your opening repertoire into picture words ([using this word list](/chessmemorypalace/picturewords)), combine them into composite images of picture word 1 + picture word 2 + location, then memorise them along a branching memory palace. This is all taught in [The Chess Memory Palace](https://amzn.to/4k7nXBO). Enjoy recalling your openings perfectly at the board!

### Comparing the original Picture Notation and the new Image Notation
Both the original Picture Notation and the new Image Notation work perfectly as mnemonic codes, generally keeping 1 picture word = 1 move, with no ambiguity.

The advantage of the original Picture Notation is that it uses a slightly smaller vocabulary set. This means that if you want to convert from move to picture word while at the board, which can be useful to help use your memory palace, there is slightly less to learn.

The advantage of Image Notation is that it follows algebraic notation closely, which makes it more intuitive and easier to use. This also makes it easier to review a few moves ahead while at the board. (And also means you can scan across your memory palaces for every instance of a move, e.g. Qd4, if for some reason you wanted to do that.)

The difference is small: choose whichever mnemonic system you prefer.
