---
title: Obsessed with terminology
author: Ghassen Faidi
pubDatetime: 2026-2-24T04:06:31Z
slug: terminology
featured: true
draft: false
tags:
  - terminology
description:
  sharing my thoughts about terminology

---

<figure>
  <img
    src="/images/terminology/thistle-dither-annotated.png"
    alt="TODO"
  />
  <figcaption class="text-center">
    Golden Thistles, April 2025
  </figcaption>
</figure>


Last year, I started to learn more about the flora in my surroundings, the names of plants and flowers. What amazed me is how, once I knew their names, I couldn't stop seeing them, observing how plants grow and wither, how they change from season to season. It made walking around much more fun.
When you know the names of things, it builds some kind of a bond with them. You start to see things differently.
It reminded me of Anne of Green Gables and how, as a kid, she would give cool names to things, trees, and places she visited.

> They should call it—let me see—the White Way of Delight. Isn't that a nice imaginative name? -- Anne of Green Gables



The same thing happened to me with programming.
I still remember when I finally understood the term "abstraction" (which has a specific meaning in computer science). I was so excited because it explains a LOT of things: gates abstract transistors, ICs abstract logic gates, the OS is just a huge abstraction, TCP abstracts IP, functional abstraction, parametric abstraction, syntactic abstraction (macros), etc.
I found myself using the term "abstraction" so much: *this abstracts that, this is a leaky abstraction, this is a nice abstraction.* 😅

Sometimes the value of a term isn't obvious at first; I still remember hearing the term "binding" for the first time.
Something like *foo is bound to 10* for `foo = 10`.

I didn't get it; why on earth not just call it "assignment"!
Later I learned that binding is a much broader idea; it's just the abstract idea of associating a "name" to a "value." For example, the name of the function is bound to the function (could be some object, perhaps a closure); when you import something from a module or library, you are creating a binding too. Binding is in a different level of abstraction. 
And even the terms "name" and "value" are actually super interesting.
For instance, I felt so happy after learning this definition of a *value*:

> a value is an expression that evaluates to itself.

It's one of the most simple and elegant definitions I have seen, and it's powerful as a tool for thinking. It made me realize [I didn't actually understand C](https://stackoverflow.com/questions/79537353/how-does-the-left-hand-side-lhs-of-an-assignment-evaluate-in-c).
Good fundamental terms guide us to ask the right questions and show you the gaps in understanding.

That's one of the benefits of studying functional programming (and computer science in general): it leaves you with an arsenal of mental models and sharp terms that assist your reasoning and communication.


But as an excited young computer science student, I didn't like it when people misused terminology; it's a problem that needed fixing, I used to think.

Then I slowly started to notice that most programmers, including people far more experienced and wiser than me, don't care much about terms at all and use whatever crosses their mind first. On top of that, I saw that the way people invent terms is often arbitrary.
Why is entropy called "entropy" in information theory? Well, it's pretty much a joke.

> I thought of calling it "information", but the word was overly used, so I decided to call it "uncertainty". [...] Von Neumann told me: you should call it entropy, for two reasons. In the first place your uncertainty function has been used in statistical mechanics under that name, so it already has a name. In the second place, and more important, nobody knows what entropy really is, so in a debate you will always have the advantage. -- [Wikipedia](https://en.wikipedia.org/wiki/Entropy?useskin=vector#Information_theory)

Why is it called a lambda function?

> It may seem perverse to use lambda to introduce a procedure/function. The notation goes back to Alonzo Church, who in the 1930's started with a "hat" symbol; he wrote the square function as "ŷ . y × y". But frustrated typographers moved the hat to the left of the parameter and changed it to a capital lambda: "Λy . y × y"; 
from there the capital lambda was changed to lowercase, and now we see "λy . y × y" in math books and (lambda (y) (* y y)) in Lisp. -- [Peter Norvig](norvig.com/lispy2.html)

But the person who really changed my perspective on the importance of terminology was Professor Dan Grossman. I was studying his [online course](https://www.coursera.org/learn/programming-languages) on programming languages. While he was explaining the difference between "higher-order functions" and "first-class functions," he said, "People often confuse these terms and use them interchangeably, so we won't care so much either." 
That hit me. If someone with a PhD in programming languages doesn't care, why do I? Is precision a tool, or is it an end in itself?

I loosened up; I stopped correcting people when not necessary. I also started to dislike courses and books that are full of unimaginative jargon, one example I won't forget is "ideation", [which is another word for "thinking"](https://web.archive.org/web/20190207015323/https://hbr.org/2008/08/why-jargon-feeds-on-lazy-minds.html).


I also started to appreciate it in books and in courses when the teacher shows that they are aware of jargon and terms that sound way too fancy, as in [Crafting Interpreters](https://craftinginterpreters.com/a-map-of-the-territory.html#scanning):

> The first step is scanning, also known as lexing, or (if you’re trying to impress someone) lexical analysis. They all mean pretty much the same thing. 


I like it because it sounds human.

## When misusing terms causes misunderstanding

I remember a professor saying "JavaScript is an interpreted language", and started explaining the drawbacks of being interpreted.

Now, later when I studied programming languages, I realized how what he said actually distorted my understanding.
Being interpreted or compiled is not a matter of the language; it's a property of the implementation. Without that understanding, one starts to confuse dynamic typing with interpreting and static typing with compiling. A language can be implemented using a compiler, interpreter or even both.
Once I got it, I started to see languages with more clarity, and was able to recognize the characteristics that matter and the ones that don't in programming languages.

If understanding is distorted by misusing terms, leading to wrong thinking, perhaps it's worth being careful.

So, overall, I think we should take it easy; most misuse of terms is harmless, and people are good at understanding each other. But in some cases, it's worth being precise.

---

## Side notes

Recently I've been reading the novel Orwell's 1984 for the first time. One idea really struck me, creating a new language (Newspeak) with a vocabulary deliberately small to limit how people think and feel. You'd walk past flowers, but perhaps you'd never see them.