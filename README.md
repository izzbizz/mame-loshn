# mame-loshn מאמע-לשון

developing a system that can back-transliterate romanized yiddish to the alef-beys

## data

#### so far we have parallel data:

- 11.000 records (titles and author names) scraped from the yiddish book center's [digital yiddish library](https://www.yiddishbookcenter.org/collections/digital-yiddish-library)
- 8.000 records provided by the israeli [national library](https://www.nli.org.il)
- 8.000 place names from [yiddishland](https://yivo.org/yiddishland-topo)
- 7.000 records provided by the [brandeis university library](https://www.brandeis.edu/library/)
- 2700 nouns from the [multi-orthography parallel corpus of yiddish nouns](https://codeberg.org/jonne/yiddish-lrec-2020)
- 2400 words from [yidlid](http://yidlid.org/), a page with lyrics for yiddish songs
- 1500 records from the hessisches bibliotheksinformationssystem [hebis](https://www.hebis.de/)
- 1300 names from wikidata
- 300 proverbs from [yiddish wit](https://www.yiddishwit.com/List.html)
- parallel translation and transliteration of "le petit prince" to yiddish, courtesy of the translator shlomo lerman [דער קליינער פרינץ](http://www.petit-prince.at/pp-jidd.htm)

#### monolingual data (for pre-training a language model):

- 28,000 articles from the [yiddish wikipedia](https://yi.wikipedia.org/wiki/%D7%94%D7%95%D7%99%D7%A4%D7%98_%D7%96%D7%99%D7%99%D7%98)

## more yiddish resources on the internet

- refoyls yidish veb-bletl [link](https://www.cs.uky.edu/~raphael/yiddish.html)
- library of congress romanization rules [link](https://www.loc.gov/catdir/cpso/romanization/hebrew.pdf)
- list of words of hebrew (לשה"ק) origin [link](https://yi.wikipedia.org/wiki/%D7%9C%D7%99%D7%A1%D7%98%D7%A2_%D7%A4%D7%95%D7%9F_%D7%9C%D7%A9%D7%95%D7%9F-%D7%A7%D7%95%D7%93%D7%A9_%D7%95%D7%95%D7%A2%D7%A8%D7%98%D7%A2%D7%A8_%D7%90%D7%99%D7%9F_%D7%99%D7%99%D7%93%D7%99%D7%A9)
- yiddish alphabet with dialectal differences in pronunciation: [דער יידישער אלף-בית](https://tildeweb.au.dk/au132769/alefbeys.htm)

## literature

### yiddish orthographies

- bella hass weinberg: *ambiguities in the romanization of yiddish* [paper](https://ajlpublishing.org/index.php/jl/article/download/163/153/)
- steven a. jacobson: *a guide to the more common hebraic words in yiddish* [paper](https://www.yiddishbookcenter.org/collections/yiddish-books/spb-nybc203464/jacobson-steven-a-a-guide-to-the-more-common-hebraic-words-in-yiddish)
- tsuguya sasaki (tsvi sadan): *a morphological study of the hebrew-aramaic component in yiddish*
- tsuguya sasaki (tsvi sadan): *the hebrew component in yiddish: research possibilities* (both available on the author's [website](https://sites.google.com/view/tsvisadan/research/publications))

### yiddish nlp

- dmitriy genzel et al: *creating a high-quality machine translation system for a low-resource language: yiddish* [paper](https://research.google/pubs/pub35627/) [excerpt](excerpts/genzel-macherey-uszkoreit-2009)
- jonne sälevä: *a multi-orthography parallel corpus of yiddish nouns* [paper](https://www.aclweb.org/anthology/2020.lrec-1.119/) [excerpt](excerpts/sälevä-2020)

### neural machine transliteration (nmtr)

- mohamed seghir hadj ameur et al: *arabic machine transliteration using an attention-based encoder-decoder model* [paper](https://www.researchgate.net/publication/320972105_Arabic_Machine_Transliteration_using_an_Attention-based_Encoder-decoder_Model)
- thomas deselaers et al: *a deep learning approach to machine transliteration* [paper](https://dl.acm.org/doi/10.5555/1626431.1626476)
- andrew finch et al: *target-bidirectional neural models for machine transliteration* [paper](https://www.aclweb.org/anthology/W16-2711/)
- imane guellil et al: *arabizi transliteration of algerian arabic dialect into modern standard arabic* [paper](https://www.researchgate.net/publication/318755390_Arabizi_transliteration_of_Algerian_Arabic_dialect_into_Modern_Standard_Arabic)
- sarvnaz karimi et al: *machine transliteration survey* [paper](https://dl.acm.org/doi/10.1145/1922649.1922654) 
- anoop kunchukuttan et al: *leveraging orthographic similarity for multilingual neural transliteration* [paper](https://transacl.org/ojs/index.php/tacl/article/view/1248)
- soumyadeep kundu et al: *a deep learning based appraoch to transliteration* [paper](https://www.aclweb.org/anthology/W18-2411/)
- ngoc tan le, fatiha sadat: *low-resource machine transliteration using recurrent neural networks of asian languages* [paper](https://www.aclweb.org/anthology/W18-2414/)
- ngoc tan le, fatiha sadat et al: *low-resource machine transliteration using recurrent neural networks* [paper](https://dl.acm.org/doi/abs/10.1145/3265752)
- ngoc tan le, fatiha sadat: *improving the neural network-based machine transliteration for low-resourced language pair* [paper](https://www.aclweb.org/anthology/Y18-1038/)
- yuval merhav, stephen ash: *design challenges in named entity transliteration* [paper](https://www.aclweb.org/anthology/C18-1053/) [excerpt](excerpts/merhav-ash-2018)
- kanishka rao et al: *grapheme-to-phoneme conversion using long short-term memory recurrent neural networks* [paper](https://ieeexplore.ieee.org/document/7178767)
- mihaela rosca, thomas breuel: *sequence-to-sequence neural network models for transliteration* [paper](https://arxiv.org/abs/1610.09565)
- rico sennrich et al: *neural machine translation of rare words with subword units* [paper](https://www.aclweb.org/anthology/P16-1162/)
- yan shao, joakim nivre: *applying neural networks to english-chinese named entity transliteration* [paper](https://www.aclweb.org/anthology/W16-2710.pdf)
- shyam upadhyay et al: *bootstrapping transliteration with constrained discovery for low-resource languages* [paper](https://www.aclweb.org/anthology/D18-1046/)
- shijie wu et al: *applying the transformer to character-level transduction* [paper](https://arxiv.org/abs/2005.10213)
- kaisheng yao, geoffrey zweig: *sequence-to-sequence neural net models for grapheme-to-phoneme conversion* [paper](https://arxiv.org/abs/1506.00196)

### other interesting research on transl(iter)ation

- christos baziotis et al: *language model prior for low-resource neural machine translation* [paper](https://arxiv.org/abs/2004.14928)
