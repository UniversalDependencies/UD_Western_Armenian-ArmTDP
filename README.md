# Summary

The Western Armenian UD treebank is based on the Western Armenian section of the Armenian Dependency Treebank (Հայերէնի Ծառադարան), developed for UD originally by the ArmTDP team led by Marat M. Yavrumyan at the Yerevan State University.

# Introduction

The UD_Western_Armenian-ArmTDP treebank is based on the Հայերէնի Ծառադարան dataset (version 1.0), a mix of texts sampled from different sources and representing different genres and domains, released in several formats (local on-line newspaper and journal articles, fiction dated between 1895 and 2020). The treebank consists 1780 sentences (~36K tokens).

The annotation scheme was developed in according to the UD guidelines. The original data was manually annotated by the ArmTDP team. The tokenization and POS-tagging process was carried out through alternating steps of automatic scripting and manual revision in the YerevaNN research lab (led by Hrant H. Khachatrian). The treebank is so far the only manual verificated corpus of Western Armenian supplied with comprehensive morphological annotation and syntactic annotation in the form of a complete dependency tree provided for every sentence.

# Acknowledgments

This work became possible in part by a research grant from the Calouste Gulbenkian Foundation («Գալուստ Կիւլպէնկեան» Հիմնարկութիւն) based in Lisbon, Portugal.

The team behind the UD_Western_Armenian-ArmTDP: Marat M. Yavrumyan, Hrant H. Khachatrian, Anna S. Danielyan, Setrag H.M. Hovsepian, Liana G. Minasyan.

## References

* Marat M. Yavrumyan. “Universal Dependencies for Armenian.” International Conference on Digital Armenian, Abstracts. Inalco, Paris, October 3-5, 2019.

## Format

UD_Armenian-ArmTDP data conforms to [CoNLL-U](http://universaldependencies.org/format.html) format with the following specifics:
* Sentence-level comments:
  * Document titles are present as `# doc_title = Սիլիհտարի պարտէզները`.
  * Document boundaries are present as `# newdoc id = fiction/news-xxxx`.
  * Sentence-level paragraph boundaries are present as `# newpar id = newdoc-xxxx`.
  * Sentence boundaries are present as `# sent_id = newdoc-newparxxxx`.
* XPOSTAG column is currently unused.
* No enhanced dependencies or empty nodes present in DEPS column.
* MISC column:
  * `SpaceAfter=No` markers are present.
  * Form (`Translit`) and lemma (`LTranslit`) transliterations are present (based on ISO 9985:1996).
* Document, paragraph, sentence, and token ids are 4-character base-32 numbers. They survive treebank updates.

# Changelog

* 2021-05-15 v2.8
  * Initial release in Universal Dependencies.


<pre>
=== Machine-readable metadata (DO NOT REMOVE!) ================================
Data available since: UD v2.8
License: CC BY-SA 4.0
Includes text: yes
Genre: fiction nonfiction
Lemmas: manual native
UPOS: manual native
XPOS: not available
Features: manual native
Relations: manual native
Contributors: Yavrumyan, Marat M.
Contributing: elsewhere
Contact: myavrum@ysu.am
===============================================================================
Documentation contributors: Yavrumyan, Marat M.; Danielyan, Anna S.
https://github.com/armtreebank
</pre>
