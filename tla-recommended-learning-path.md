# Introduction to TLA+ in Onomy

TLA+ is a specification language created by Leslie Lamport in 1999. This is "formal" specification, based on
pure mathematics.

In Onomy we use TLA+ to formally define most critical parts of the infrastructure.

Currently, the following elements are specified with TLA+:

- the custom consensus protocol we use in Onomy Blockchain ("Equity")
- the mechanics of decentralized exchange ("Market")

This document serves as a guide for team members who want to learn TLA+. It reflects the most up-to-date
knowledge on the optimal path to learn TLA+.

# The reference path to learn TLA+

## Step 0: Mathematical prerequisites

TLA+ is based on:

1. First Order Logic (see [here](https://en.wikipedia.org/wiki/First-order_logic))
1. Zermelo-Fraenkel set theory (see [here](https://en.wikipedia.org/wiki/Zermelo%E2%80%93Fraenkel_set_theory))
3. Temporal Logic (see [here](https://en.wikipedia.org/wiki/Temporal_logic))

(1) and (2) are what is considered a "standard" notation in mainstream math for (at least) last 100 years.

Wikipedia gives a shallow intros to all these topics - nevertheless they are deep enough to grasp TLA+.

For a more detailed introduction to set theory, consider reading the paper "Fundamentals of Zermelo-Fraenkel
set theory" by Tony Lian (or some graduate-level handbooks for math students).

## Step 1: Read TLA entry in Ron Pressler's blog

Somehow it happened that it was not the inventor of TLA+ who gave best introduction to the language.

There are 4 blog entries, linked into a chain. This chain starts [here](https://pron.github.io/posts/tlaplus_part1).

## Step 2: Read "Specifying systems" book by Leslie Lamport

The book can be downloaded from [here](https://lamport.azurewebsites.net/tla/book.html?back-link=learning.html#download).

This book introduces TLA+ in examples-oriented way. This is a little convoluted, because the author is a mathematician,
so he definitely is a definition-oriented person - nevertheless he seems to believe that the path "define-than-use" is unnatural
to engineers. Following this (false) assumption he attempts to introduce TLA+ gradually with examples. This turns out to be
heavily confusing when used as the first intro to TLA+. It however turns into quite useful when read AFTER everything
is nicely explained in Ron's blog (see step 1 above).

## Step 3: Install TLA+ IDE

The "reference" IDE for TLA+ is called "Toolbox" and can be downloaded from [here](https://lamport.azurewebsites.net/tla/toolbox.html).

A developer used to the perfection of IDEs in 2021 will find this IDE rather rough. Nevertheless, it is useful. The biggest
issue is that this IDE is not smart enough to render TLA+ symbols. All you can do is to work with ASCII representation
of these symbols (which largely resembles working with LaTeX).

Alternatively, one can install Visual Studio Code, which supports a plugin for TLA+. There is also another plugin
which allows nice rendering of TLA+ symbols - see [here](https://www.gitmemory.com/issue/alygin/vscode-tlaplus/197/770464096).

### Step 4: Analyze some examples

- TLA+ main GitHub site: [here](https://github.com/tlaplus)
- Hillel Wayne blog: [here](https://www.hillelwayne.com/)
- Building a simple distributed system: [here](https://jack-vanlightly.com/blog/2019/1/25/building-a-simple-distributed-system-the-what)
- Alexander Niederbühl: [here](https://github.com/Alexander-N/tla-specs)

### Step 6: Read PlusCal book (by Hillel Wayne)

PlusCal is another specification language created by Leslie Lamport. It compiles to TLA+. It was a brave attempt to attract
these software developers, who are into "hacking" but who perceive pure math as "too scary to be useful". Hence, PlusCal attempts
to mimic programming language syntax.

Hillel Wayne - who is a TLA+ guru - published a book with a misleading title "Practical TLA+". Contrary to the title, this book
is exclusively devoted to PlusCal. It ignores TLA+ completely.

Nevertheless, it gives another interesting perspective on TLA+ in general.

## Step 7: Attempt writing a spec and analyze it

(under construction)

## Step 8: Play with proofs

(under construction)

