---
title: Vectorisation and Memories
subtitle: Using vectorisation to deal with painful memories
date: 2022-02-28T09:57:11.856Z
draft: false
featured: false
image:
  filename: featured
  focal_point: Smart
  preview_only: false
---
When I was taking the classes of Dr. Ng on Machine Learning *(to which an adequate reference and detail already exists in a post called [Update] (<update>))* I was occasionally struck by how much I was learning on the subject. It occurred to me that I had spent so many many years mentally idling around while this resource which was already about ten years old on the internet existed. I was baffled at my self, how much time I wasted doing stuff that did not hold any interest for me whereas I was only thinking of how to earn money from them. Yet this thing was there all the time. I was just struck dumb.

Being that my primary temperament is a melancholy one, it is very easy for me to slide down into the cycle of reminiscing, regretting and mental self-battery. Incidentally I have had a good many lessons from M. Coué that it wouldn't do to go back that road regardless. Also, a good dose of mental prayer and meditation helps one to see some of these faults in good light. Good light does not mean that the faults are good; no, not at all. It means that I can see them more clearly as they are with their origins and effects. And so I learnt to not berate myself for those failings but then what am I to do when in the middle of my work they start to line up and walk past my screen when I am cracking my head to figure out how best to write a code so that it not only calculates properly but it is able to pass all tests.

This is important to me because more than 70 percent of the lost years was spent solely on mental regurgitation: revisiting past mistakes, magnifying them and feeling bad about them, and thinking how they have made it impossible for me to move ahead. If only this, if only that! etc... So at this time, in addition to autosuggestion and meditation, was there any thing I could also do that would make it possible and feasible for me to deal with this thing a little more easily? At this time it was not as bad as it was even a month ago. With each passing day that I poured myself out into my studies and work while also doig the A&Ms I do, the memories were receding. Their power was waning. But you know, if you've seen the darks, you start to loathe even shadows. I didn't want them to hang over my life anymore. I have a future to figure out, and a lot of catching up to do.

That was about the time I was solving problems and writing codes using vectorisation. To summarise what vectorisation is for the non-initiated, it's a way to deal with matrices as though they were vectors. A matrix is an mXn array of numbers or values where the number of rows m and the number of columns n are real numbers greater than 1. A vector on the other hand is either an mX1 or a 1Xm array. I hope array is the right word.

In other words rather than dealing with the mXn matrix which could be 240X500 for example as a matrix in which you have to go through 120000 values on 240 rows and 500 columns one after the other, you look at it as though it were a 120000 X 1 vector. You are just going through all the numbers once. Vectorization makes it really fast and easy to operate on large matrices. So you can add, subtract, multiply or divide the matrices as easily as though they were just vectors or plain numbers.

One question you might ask is, "What would be the alternative to an unvectorised operation?" Well, the simple answer I found out at this time which also happened to the approach I was using at first was the use of loops, especially for-loops. Write something like:

```octave
for i = 1:end;
    for j = 1:end;
        A(i,j) = V(i,j) * Example(i,j);
    endfor
endfor;
```

Now this is only a simple multiplication but imagine that you had to do a division and exponent too. Regardless of the package you were using, the larger the matrices, the longer your code would start to take to run. Now what would the vectorised version look like? Don't be shocked.

```
A = V * Example;
```

That's all. And V and Example can be as large as they want. They can have *m >= 1000*, *n >= 1000*, and your code would run in Octave without skipping a beat. It was awesome. Of course you have to bear in mind that as part of Linear Algebra some operations require matrix transposition and others require that the matrices have similar dimensions. Other than that, as long as you have that sorted, your vectorisation will make your code run like a breeze. Really cool and neat stuff huh! Of course.

Well, I took it a little step further and used it to deal with my annoying, painful, repetitive and intrusive memories. That's the real subject of this article anyway so why not get to it at once. How did I or how am I doing it?

I should explain that I have a predominantly melancholy temperament which means that it is as easy for me to brood over past hurts whether real or imagined as it is for some people to make friends and laugh with everyone they meet. So I categorised these memories into two distinct groups: the sins (the wrongs I did mostly deliberately) and the faults (wrongs that were inadvertent and not deliberate).

The deliberate ones are called sins in Christian parlance because you know they are bad and you do them anyway without caring for the consequences (which sometimes we don't really appreciate the magnitude of). The faults are things that we do wrong because of our temperament, our nature or plain ignorance. They can be really bad, but not as bad as the deliberate sins. Sometimes faults we refuse to acknowledge can go from being just a shortcoming to  becoming a strong magnet to the worst kinds of sins.

In any case, like every human being I have my share of both. The painful part was that when I remembered them they made me real sad. And the faults sometimes hurt more than the sins. This is because as Catholics you confess the sins to the priest and he absolves you and the sins go away, effaced. But we forget or sometimes don't consider the faults as worth confessing so they stay and they attract the sins again. Plus faults can be really embarrassing and hurt our pride while also assuming different shapes in the mind.

At this point I was done being exhausted and mentally distracted. So I decided to apply vectorisation. In my memory, there were lots of wrongs, mostly confessed. And there were lots of faults big and small. Rather than go through them one by one and either pray about them or think about how to forget them one at a time, I created vectors of both.

```octave

faults =  m * n;  # matrix of the faults
evils = m * n; # matrix of the moral wrongs 
memories = faults * evils;

```

Now all I need to do is each time I remember one or the other, I place it in the appropriate vector, multiply them and just stash it a way as a matrix of memories. I don't need to bother about what is inside. And I just pray for it all as one vector of memories.

It doesn't bother me anymore as it used to and I can move forward with my life. At the same time, it is also easy for me to make the distinction between sins and faults because I have to manually add each one to the vector where it belongs without caring about what was already there. The more I correct the faults, the less I have sins to add to the sin vector in my memory. And I can learn to confess the faults so that they too lose their power. That way my head is clearer and I can focus on what I need to do to get my work done.
