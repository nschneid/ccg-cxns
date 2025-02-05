---
layout: entry
title: Multiword Expressions
---

## Pages

<ul>
{% for p in site.mwe %}
  {% if p.title != page.title %}<li><a href="{{ site.baseurl }}{{ p.url }}" class="doclabel">{{ p.title }}</a></li>{% endif %}
{% endfor %}
</ul>

## Definition

## General issues to consider

1. Which of the (lexicalized) words is the _syntactic_ head, i.e., it takes all the other lexicalized words 
as dependents in the derivation and bears inflections?

2. Which of the words is the _semantic_ head, i.e., it specifies any idiosyncratic aspects of the meaning?

3. How to treat the semantics of lexicalized words other than the semantic head? 
Do they have null semantics?

4. How to assign categories such that the idosyncratic lexical entries are limited to instances of the MWE?

## References

* Baldwin & Kim 2010, [Multiword Expressions](http://ww2.cs.mu.oz.au/~tim/pubs/handbook2009.pdf). In N. Indurkhya and F. J. Damerau (eds.), _Handbook of Natural Language Processing, Second Edition_.
* Ch. 3 of [Nathan's disseration](http://www.cs.cmu.edu/~nschneid/thesis/)

### MWEs in CCG

* Bozşahin 2022 [Referentiality and configurationality in the idiom and the phrasal verb](https://doi.org/10.1007/s10849-022-09381-y)
* Bozşahin & Guven 2018 [Paracompositionality, MWEs and argument substitution](http://arxiv.org/abs/1805.08438)
* Lancioni & Boella 2012, [Idiomatic MWEs and Machine Translation: A Retrieval and Representation Model: The AraMWE Project](http://mt-archive.info/AMTA-2012-Lancioni.pdf). _Proc. of the Fourth Workshop on Computational Approaches to Arabic Script-based Languages._
  - §3.2 describes a proof-of-concept grammar of 18 English and 18 Arabic verbal MWEs, including _kick the bucket_. See figures 1, 3, and 4. Apparently, their solution assigns no semantics to the direct object NP and the idiomatic verb has no constraint on which direct objects it licenses.
* de Lhoneux 2014. CCG Parsing and Multiword Expressions. MS Thesis, Edinburgh [supervised by Mark and Omri].
* de Lhoneux et al. 2019. [Investigating the effect of automatic MWE recognition on CCG parsing](http://langsci-press.org/catalog/view/202/2027/1553-1)
