---
layout: post
title: A Theory of Mnemonics
permalink: /theoryofmnemonics

---

This is an extract from The Chess Memory Palace (Chapter 7).

{% include chess-memory-header.html %}


## Chapter Contents
- [Fundamentals of mnemonic systems](#fundamentals-of-mnemonic-systems)
- [Non-linear memory palaces](#non-linear-memory-palaces)
- [Mnemonic codes](#mnemonic-codes)
- [Mnemonic code for chess moves: the specifications](#mnemonic-code-for-chess-moves-the-specifications)
- [How Image Notation meets these specifications, and why alternatives do not](#how-image-notation-meets-these-specifications-and-why-alternatives-do-not)
- [Error detection and redundancy](#error-detection-and-redundancy)
- [Analysis paralysis](#analysis-paralysis)


> *I’ve done the analysis with my engine, and I’ve organised everything, and I understand it and I get it -- I just can’t remember it.*  
> — GM Patrick Wolff

Memory palaces are a powerful tool to expand your memory. However, it's not always obvious how to apply them. One of the common questions is, "I have [some complicated dataset]. How do I memorise it?"

In this chapter I share my thoughts on how to approach this question. In the process I explain the design choices behind Image Notation and the Chess Memory Palace system, so that you understand why it is designed the way it is, and what you should consider if you want to modify it for your own preferences.

## Fundamentals of mnemonic systems

Building a mnemonic system requires two steps: (1) work out the structure of your system of pegs, then (2) build a reliable code to convert non-memorable data into memorable data.

*All mnemonics are about mapping something that you don't know onto something that you do know.* For example, you might not know the order of the planets, but you do know a series of landmarks in your street. You can then imagine the planets (or something that reminds you of the planets, e.g. a red warlike figure for Mars) in order along your street, creating visualisations (little stories) to associate one planet with one location, in order.

The "things that you do know" are often called "pegs". Traditionally pegs are locations, hence the names "memory palace", "method of loci" or "journey method", but pegs don't have to be locations; they can be anything you know well, such as song lyrics, film scenes, or football players in order of shirt number. The pegs structure the images, so that you have a way of navigating through your entire dataset. To continue the example above, you can mentally walk along your street from landmark to landmark, and recall the planet attached to each.

Mnemonist Joe Reddington, in his book *Advanced Memory Palaces*, notes that the method of loci can be thought of as just "an array that is indexed by physical locations", and that the term is shorthand for "using physical locations as a source of keywords for an array". This is correct, although my vague understanding of the science is that there *is* something special about using locations rather than objects for pegs. Our brains remember the place where we learned a piece of information, and our neurons that store locations trigger slightly before we have the conscious knowledge of remembering the information.



## Non-linear memory palaces

Usually designing Step 1, the system of pegs, is not too difficult. The vast majority of memory palaces that I have read about are linear, so one can use any linear journey of landmarks, film scenes, song lyrics et cetera.

How about memorising *tabular* data (that has rows and columns)? One method is to use a series of similarly-structured pegs (for the table rows) where you can attach the different data points in a consistent way.

For example, use five shops in a high street for five rows of data. Attach the data in column 1 to the doors, the data in column 2 to the windows, the data in column 3 to the counter, and so on. This, alongside Karnaugh maps (like Venn diagrams) and binary trees, is discussed in *Advanced Memory Palaces*. Joshua Foer's famous book *Moonwalking with Einstein* discusses a similar approach for remembering details about several individuals, for a memory competition.

For chess, there is a challenge: chess openings take a *branching tree structure* (technically a *directed graph* when there are transpositions involved), so it is natural for the system of pegs to also take a branching tree structure.

As a side note, the system of pegs does not necessarily have to take the same structure as your original data, as Joe Reddington pointed out to me in correspondence. For example, you may be able to memorise a simple lookup table that will enable you to navigate through the branches of tree-shaped data. This does not work for chess, because you do not always respond to the same move from your opponent in the same way -- it depends on the board position. Another approach to tree-shaped data is to use computer science techniques to convert the data into a linear shape, but I could not find a satisfactory way to do this for an unbalanced tree like a chess opening.

So, for chess we need a branching system of pegs, to match the structure of the branching chess moves we want to memorise. How can we build a branching system of pegs? One correspondent told me he maps chess moves to branching family trees. This is ingenious but limited; it is much more versatile to use geographical settings with branching paths.

Arguably this is actually a more natural way to use locations than a linear memory palace. In our experience of the world, most of our locational knowledge is as a network of places. For example, if I want to find a plate in my flat, I would enter the flat, go straight on to the kitchen, then turn right to the cupboard. If I wanted to use the oven, I would enter the flat, go straight on to the kitchen, then turn left to the oven. If I wanted to access the bookshelves, I would enter the flat, turn left to the living room, then go to the far side of the room for the books. My experience of my flat isn't a linear journey hugging the edge of each room; it is more like a network of nodes. The same is true of my workplace, university campus, local town centre, and so on.

Using a network of locations, you can design memory palaces to store branching data (or graphs with loops, or flowcharts). It does make less "efficient'' use of space than a linear memory palace, because it is difficult to fit lots of locations in a room without the branching paths getting confused. But in practice I haven't needed to worry about running out of settings. If you need more settings, you can always go and explore a new town, or play a new video game!

Whatever system of pegs you use, make sure you have a systematic method to walk through the entire set of images (assuming your goal is to be able to reproduce all the information without external prompting). Despite what I have said above about trees, if possible I do think it is best to convert your data into a simple linear array. So, for example, never try to memorise an unordered set. Turn your data into a list with an order, even if the order is arbitrary.

Before we move to Step 2, we need to ask: does the design of pegs create any constraints on the mnemonic code? In the case of chess, the answer is yes. We want the memory palace to be able to branch after any pair of moves. Therefore each location (peg) can hold a maximum of one pair of moves.



## Mnemonic codes

Step 2 is about converting non-memorable data into memorable data. Memorable data is anything that is easy to visualise, animate, and describe in stories: typically people and animals and emotive objects. Often we need to design a code to convert non-memorable data into memorable data.

In the easiest cases, you don't need a code at all, you can just visualise your target information directly. The classic example is memorising a shopping list. To memorise a shopping list, you can simply visualise the items themselves, with a little bit of exaggeration, such as eggs cracking, broccoli growing through the floor like trees, orange juice spilling over the shelves, and so on.

In other cases, you can memorise a more memorable image in place of a less memorable word, but you don't need a systematic mnemonic code. For example, for *courage*, imagine Mars or Achilles (suggested in the Dialexeis fragment, c.~400 BC); for *the Earl of Balfour*, imagine a "ball 4'' pool ball (suggested by mnemonist Ed Cooke), for *Buchanan*, imagine a cannon firing (part of my exam preparation a decade ago, which I have never forgotten).

The most difficult cases are truly abstract data, when you will need to design a systematic mnemonic code (and rote memorise it). The best known example is the *major system* for memorising numbers. The digits 0-9 are coded onto consonant sounds, so that you can memorise words instead of numbers. For example, *turtle bench lime* encodes the first nine decimal places of pi (141592653). Image Notation is a modified form of the major system, so if you understand Image Notation then you should be able to understand the major system quite easily. Early versions of the major system date back to the 16th century. The practice of converting numerals to sounds for memorisation dates back at least as far as the Kaṭapayādi system in India, around 600 AD.

Memory world records have been slashed in the last 20 years. A lot of this has been due to the development of more efficient mnemonic codes. For example, using a version of the major system, you could memorise a deck of playing cards in 52 pictures, by encoding one picture per card. Ben Pridmore's *Ben system* was revolutionary, as he created a way to memorise a pair of cards in a single picture, so now mnemonists could memorise a deck of cards in 26 pictures -- at the cost of needing to prepare pictures upfront for 2704 possible combinations. A further development noticed that one can use the pegs to encode information: for example by using the same peg twice if a pair of cards starts with a red card, but moving to a new peg if the pair of cards starts with a black card. This halved the number of pictures to memorise upfront, to 1352.

A very popular mnemonic code for random digits is known as PAO: Person Action Object. In a "2-digit system'', one would memorise 100 people, each with an action and an object. For example, 15 might be Albert Einstein writing on a blackboard, and 36 might be Michael Jackson moonwalking with a white glove. Then each set of 6 random digits can be converted into an image; for example, 15-36-15 might be Albert Einstein moonwalking with a blackboard -- hence the title of Foer's book, *Moonwalking with Einstein*.

In a 3-digit system, one would memorise 1000 people, each with an action and object. This is very powerful, as a mnemonist can memorise 9 digits in a single composite image of 3 picture elements -- but it carries the high upfront cost of preparing and memorising pictures of 1000 people, actions and objects. Some people use 1000 people and objects but only 100 actions, to code 8 digits at a time.



## Mnemonic code for chess moves: the specifications

How does this apply to chess? The first point to note is that *fewer images is better*. If you can memorise 9 digits in a single composite image, that is more efficient than memorising 6 digits in a composite image. For chess, we have seen from the peg structure that we want to memorise a maximum of one pair of moves (for example *e4 e5*) in a single image, because the palace may need to branch after any pair of moves. So, ideally, we want to memorise a pair of moves in a single composite image.

The second point to note is that memory competitors need to do lots of work to memorise their images upfront, because they need to convert data to pictures in their heads. For example, when they see the number 15, they need to immediately know that 15 is coded as Albert Einstein, so that they can quickly memorise it under memory tournament conditions. In other words, they need their mnemonic system to be "bidirectional''.

In chess this is different: we can memorise our opening repertoires at leisure at home. I don't need to convert, for example, *Nf3* from a chess move into a mnemonic picture in my head: I can just look up the picture word in the Appendix. All I need to do at the board is convert a mnemonic picture back into a chess move. So, we need a system that is easy to convert a picture to a chess move, but it does not need to be easy to convert a chess move into a picture in our heads. So, we don't need to make compromises in order to minimise the number of picture words in the system.

There is a third point to note. Memory competitors are memorising uniformly distributed random data. Each of their image combinations will come up with roughly equal frequency. Joe Reddington has noted that "PAO works at its best when the information to memorise is uniformly distributed[.] When the same Ps, As, or Os turn up a lot, you get very likely to make mistakes ('Einstein is moonwalking with a banana, now Einstein is moonwalking with a Lego, now Trump is moonwalking with a banana') [...] In general, I’d go as far as to say that PAO is a poor choice for *any* structured data." It would be interesting to see a memory competition where the random digits are not uniformly distributed, but were heavily weighted towards certain digits -- would competitors need to adapt their techniques?



## How Image Notation meets these specifications, and why alternatives do not

Image Notation codes almost every chess move in a single picture word. This means any pair of moves can be shown in a single composite image of two picture words (plus location). This is the most efficient way to encode a pair of moves.

The most obvious alternative solution is to encode both the starting and target square of each move, for example *1.e4 Nf6* becomes 5254 7866 (i.e. International Correspondence Chess Federation numeric notation), which you would then convert into images and memorise. But introducing an extra image to memorise the starting square is unnecessary, doubling the amount of memory work.

The second obvious solution is not to bother memorising the piece that moves. This is the most common solution I have seen proposed online. For example, if you memorise the target squares e4 e5 f3 c6, any chess player will recognise that the moves are *1.e4 e5 2.Nf3 Nc6*. I have seen this justified as "you don't *need* to memorise which piece moves'' (not quoting anyone in particular).

The drawback of this, of course, is that it leaves ambiguities. The piece to move is not always obvious. And the justification is a misunderstanding. *If* you had to memorise a more complicated image in order to identify the piece, I would agree it might be worth memorising the target square only. But, *we are not trying to minimise the total information memorised: we are trying to minimise the total number of images (and elements within the images)*.

Image Notation uses the number of syllables within the picture word to identify the piece, so it does not increase the number of images to memorise. Identifying the candidate piece with syllables is costless in terms of memory space.

When faced with a new challenge, many mnemonists habitually want to apply PAO. This hides a couple of difficulties. First, how exactly PAO, a digit system, will unambiguously code chess moves. It is possible to use PAO to code a pair of chess moves –- but to my mind, this is 50\% worse than using Image Notation, because Image Notation needs only two elements in each composite image, not three. In addition, Image Notation can easily be decoded (from image to chess move) one half-move at a time, which is simpler at the board than decoding both P and A, then A and O, to recover the two half-moves.

Second, with chess openings, the data (chess moves) is not at all randomly or uniformly distributed, which inherently makes PAO a questionable choice. There are many more moves to the central squares than the squares round the edge of the board, and pawns and knights move more in the opening than rooks and kings. If one attempts to memorise Algebraic Notation directly (using PAO or any other code), e.g. by having a set image for Knight and a set image for e5, then sticking them together to memorise *Ne5*, the resulting set of images will see extremely high frequency of certain pieces and squares, which is likely to cause confusion. Image Notation has two improvements: (1) by having a unique image for each *move* (not piece or square), there is much less repetition; and (2) Image Notation offers a lot of flexibility in the interactions between the two picture words. This is unlike PAO, where the action that glues the person and object together is itself target information.

There are probably lots of ways to design a mnemonic code for chess that keep a correspondence of one picture for each move, so it is possible to come up with mnemonic codes that are equally as good as Image Notation, but I do not believe it is possible to create a mnemonic code that is better.

One alternative would be to count letters rather than syllables, but this requires you to spell words accurately in your head, which is harder.

A second alternative is to first identify the target square with consonant sounds, then identify the piece using syllables and a priority system. Earlier versions of this book used this system, which I called "Picture Notation''. Compared to Image Notation, Picture Notation had the advantage that it never needed an image transformation for disambiguations, and therefore was slightly more efficient in terms of memory space. However, it was less intuitive for people to understand because it was so different to Algebraic Notation, and it was harder to use because the picture words could not be interpreted without reference to a board position.

So, I believe the only way to improve Image Notation would be to make cleverer use of picture words, but these all add complexity and constraints. For example, you could have two different sets of vocabulary for white and black moves, avoiding the need to memorise the order of moves within each composite image. You would then also need an additional rule to recognise which picture words are for white and which picture words are for black.

It might be possible to improve Image Notation by finding a way to encode a move pair in a single picture word -- but this would require six items of information in a single picture word (two pieces, two target files, two target ranks), which would be difficult. Even if possible, it would not necessarily be an improvement, because at the board it can be easier to decode one player's move (from picture to chess move) at a time, rather than decoding both players' moves together.

Finally, in a kind of "compression'' technique, if you recognise common picture word pairs, you could invent a single image to replace them. For example, always memorise a snowman instead of "*Bigfoot baguette*''. However this is a small gain and requires more upfront memory work to learn the compressions.



## Error detection and redundancy

Finally, a note on error detection and correction. Some mnemonists, when memorising data for the medium to long term, will memorise some of the digits twice. For example, five-time US Memory Champion Nelson Dellis, in at least one case, memorised 1000 digits in groups of five. For each group of five, he memorised the first three digits as a person and the last three digits as an object: by memorising the middle digit twice, he could give himself a hint, if he recalled only the person or the object but not both.

You could also come up with checksums (like the last digit of a credit card) if you do not expect to be under time pressure during recall, or if you are able to do the calculation rapidly in your head. If you ever memorise something critical such as a Bitcoin address, you should definitely include lots of extra error correction images, or just memorise the crucial data twice with a different image set. One of the interesting but rarely applicable properties of mnemonics, compared with rote-learning raw facts, is that it makes "memorise it twice" possible as a concept.

Similarly, one piece of advice recommended since ancient times is to have a door or window every five or ten locations along your memory palace. This is excellent advice if you are designing a traditional linear memory palace, as it chunks your memories into digestible groups of five, and acts as a safety mechanism to alert you if you forget a location. However I have chosen not to advise this for a Chess Memory Palace, for four reasons.

First, it is less necessary for chess, because the board position itself will validate or invalidate your picture words. If you misremember an image, or accidentally skip a location, the resulting pair of chess moves will almost always be impossible or nonsensical. In other words, the board position will alert you to any mistakes in your recollection of your palace, so you do not need an additional check of grouping locations in fives.

Second, because of the branching nature of a repertoire, placing a window or door every five moves does not neatly chunk your locations into groups of five; depending on the repertoire this might force you to store many more than five locations inside a single room.

Third, the biggest challenge in creating a branching memory palace, compared to a traditional linear memory palace, is fitting the tree diagram to a setting. Requiring a window or door at regular intervals is an annoying additional constraint.

Fourth, some positions can be reached by different numbers of moves, due to transpositions, so it is not possible to maintain the "every five locations'' rule in a strict sense. For example the mainline Sicilian Sveshnikov can be reached by *1.e4 c5 2.Nf3 Nc6 3.d4 cxd4 4.Nxd4 Nf6 5.Nc3 e5 6.Ndb5 d6 7.Bg5*, or by *5...e6 6.Ndb5 d6 7.Bf4 e5 8.Bg5*.

Back in Diagram, I discussed how to create a robust composite image. The ideas are not new; they are based on techniques memory competitors use to store two pictures together in a location without getting the order confused. But formalising it like this helped me memorise images more consistently. Recall that I recommended visualising all three interactions, not just two, and that we have dual indicators of picture word order: active versus passive roles and higher versus lower position. These are forms of *redundancy* (a term from *Advanced Memory Palaces*).

In theory, you would only need to visualise two of the three interactions to be able to recover both picture words, and in theory you only need a single rule to remind you which picture word is first and which is second. But this makes your memory less robust: if you have any lapse in memory, the information is lost. By having redundancy, you should still be able to recover 100\% of the information, even if you start to forget details, e.g. you forget one of the three interactions, or you remember which picture word is higher but forget which is doing the action to the other.

When designing rules to store data in a memory palace, there is a trade-off between writing strict rules with added redundancy, versus leaving room for creative images. There is also a trade-off between spending time visualising detailed images in the first place, versus spending time reviewing and rebuilding broken links later. In general, the more you want to memorise, and the longer the time period over which you want to retain the memories, the more you should come down on the first side of both of these trade-offs. The Chess Memory Palace needs to work for large quantities of chess moves over a long playing career, hence I advise detailed images and lots of redundancy.

When designing your own mnemonic systems, consider where you want to land on these trade-offs. Do you want special markers every five/ten pegs, strict rules for the images, and extra images for error detection and correction, or is it not worth it?



## Analysis paralysis

There is a lot to consider when designing a mnemonic system, but my final piece of advice is to not overthink it. Sometimes you just need to start, and you will work out the problems as you go along.

My early versions of Picture Notation and Image Notation used transformations, vowel sounds and a complicated piece-priority system to choose the candidate piece. I only simplified it over time, and particularly when writing the book, as explaining a system forces you to iron out any unnecessary complications. This also meant that I had a collection of old chess memory palaces in my mind that used outdated technology, which I have gradually let decay, apart from a few annoyingly persistent images.

So, it's worth designing the best system you can upfront, and I hope this chapter will be helpful in that endeavour, while also giving confidence that the Chess Memory Palace follows sound mnemonic principles. But don't get too bogged down: as always, the best system is the system you will actually use.
