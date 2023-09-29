---
title: "Text Analysis Overview"
date: 2022-02-15T17:23:12+10:00
draft: false
---

### Understanding Text as Data

Many definitions of _data_ include an element such as _individual items of information_. If we consider _text_ to include any sort of language in use, covering different modalities (spoken, written signed) and different extents (from individual sounds to multi-volume books), then fitting text to this definition requires some abstraction. We have to define some unit or units of analysis and we can then treat each of those units as an individual item of information. Examples of such units include documents, sentences and words. But _word_ is not as simple a unit as you may think.

### What's in a word?

The term _word_ is problematic. It is well-known to linguists that phonological words (defined by sound patterns), syntactic words (defined by combinatorial possibilities) and orthographic words (defined by the conventions of a writing system) do not always coincide. And even when we are only looking at written material, there are problems. How many words are there in this sentence?

_The cat sat on the mat_

One answer is that there are six words; that is, there are six groups of characters which are separated according to typographical convention. But there is another answer: There are five words, that is five distinct sequences of characters and one of those sequences (_the_) occurs twice. The terms standardly used to make this distinction are **type** and **token**. **Tokens** are instances of **types**, therefore if we count tokens, we count without considering repetition, while if we count types, we do consider repetition. In our example, there are five types (_the, cat, sat, on, mat_) but six tokens, because there are two tokens of one of the types (_the_).

There is a further distinction we may need to make which we can see if we consider another question:

<center>Are <i>cat</i> and <i>cats</i> the same word?</center>

They are distinct types, and therefore must also be distinct as tokens. But we have an intuition that at some level they are related, that there is some more abstract item which underlies both of them. This concept is usually referred to as a **lemma** (there is more about this concept on the [Data Preparation](../data_prep) page).

### Text Analysis Workflow

This brief introduction to text analysis divides the process into three parts. In the first stage, the text is made into data. It is divided into the units appropriate for the analysis to be carried out and shaped to a format which our analytic tools can work with. The second stage is the analysis proper, including its interpretation. A wide range of analytic methods can be used, and we give a survey of some of the commonly used possibilities. Finally, our data, methods and results can be documented and packaged as a **research object** which can be stored and reused.

[Data Preparation](../data-prep/) &emsp;&emsp; [Useful Methods](../methods) &emsp;&emsp; [Research Objects](../research-objects)
