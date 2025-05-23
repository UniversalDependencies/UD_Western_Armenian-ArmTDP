# Summary

A Universal Dependencies treebank for Western Armenian was developed for UD originally by the ArmTDP team led by Marat M. Yavrumyan at the Yerevan State University.

# Introduction

The UD_Western_Armenian-ArmTDP treebank is based on the Western Armenian part of the Հայերէնի Ծառադարան (ArmTDP v2.0) - a representative corpus of written Modern Standard Armenian covering a wide range of genres. The treebank consists of 6656 sentences (~122K tokens).

The annotation scheme was developed under the UD guidelines. The original data was manually annotated by the ArmTDP team. The tokenization and POS-tagging process involved alternating glossary-based automatic scripting and manual revision steps. The treebank is the only manually verified corpus of Western Armenian, supplied with comprehensive morphological and syntactic annotation in the form of a complete dependency tree for every sentence.

# Acknowledgments

This work became possible through a research grant from the Calouste Gulbenkian Foundation («Գալուստ Կիւլպէնկեան» Հիմնարկութիւն) based in Lisbon, Portugal.

The team behind the UD_Western_Armenian-ArmTDP: Marat M. Yavrumyan, Hrant H. Khachatrian, Anna S. Danielyan, Setrag H.M. Hovsepian, Liana G. Minasyan.

## References

* Marat M. Yavrumyan. “Universal Dependencies for Armenian.” International Conference on Digital Armenian, Abstracts. Inalco, Paris, October 3-5, 2019.
* Marat M. Yavrumyan, Anna S. Danielyan, “Universal Dependencies and the Armenian Treebank.” Herald of the Social Sciences (2): 231-244, 2020. (in Armenian)

## Format

UD_Western_Armenian-ArmTDP data conforms to [CoNLL-U](http://universaldependencies.org/format.html) format with the following specifics:
* Sentence-level comments:
  * Document titles are present as `# doc_title = Սիլիհտարի պարտէզները`.
  * Document boundaries are present as `# newdoc id = blog/fiction/news/nonfiction-xxxx`.
  * Sentence-level paragraph boundaries are present as `# newpar id = newdoc-xxxx`.
  * Sentence boundaries are present as `# sent_id = newdoc-newparxxxx`.
* XPOSTAG column is currently unused.
* No enhanced dependencies or empty nodes present in DEPS column.
* MISC column:
  * `SpaceAfter=No` markers are present.
  * Form (`Translit`) and lemma (`LTranslit`) transliterations are present (based on ISO 9985:1996).
* Document, paragraph, sentence, and token ids are 4-character base-32 numbers. They survive treebank updates.

# Changelog

* 2023-11-15 v2.13
   * Fixed annotation errors and inconsistencies.

* 2022-05-15 v2.10
  * Fixed annotation errors and inconsistencies, added new texts: 93K→122K (reviews, social, spoken, web and wiki).
  * Resplitted train/dev/test.
  * Fixed some validation errors.

* 2021-11-15 v2.9
  * Fixed annotation errors and inconsistencies, added new texts: 36K→93K (mostly blog and news).
  * Introduced `flat:dist`, `flat:range`, `flat:frac`.
  * Specified `advcl:relcl`.
  * Resplitted train/dev/test.
  * Fixed some validation errors.

* 2021-05-15 v2.8
  * Initial release in Universal Dependencies.

<pre>
=== Machine-readable metadata (DO NOT REMOVE!) ================================
Data available since: UD v2.8
License: CC BY-SA 4.0
Includes text: yes
Genre: blog fiction news nonfiction reviews social spoken web wiki
Lemmas: manual native
UPOS: manual native
XPOS: not available
Features: manual native
Relations: manual native
Contributors: Yavrumyan, Marat M.
Contributing: elsewhere
Contact: marat.yavrumyan@plus.ac.at
===============================================================================
Documentation contributors: Marat M. Yavrumyan, Anna S. Danielyan, Setrag H.M. Hovsepian
https://github.com/armtreebank
</pre>
