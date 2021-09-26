---
title: Computational Linguistics 2 (CL3.202)
subtitle: |
          | Monsoon 2021, IIIT Hyderabad
          | Assignment 2
header-includes:
- \newfontfamily\malayalamfont{MalayalamMN}
---

# Question 1
## Prototype
The prototype of a predicate is a typical member of the set of entities to which it may be applied. For example,  

* [കൊതുക്]{lang=ml} `koVwuk` (mosquito)  
    A prototype of this predicate can be a small, winged insect that tends to suck blood and cause itchy bites.

* [പുസ്തകം]{lang=ml} `puswakaM` (book)  
    A prototype of this predicate can be a collection of pages of paper bound together, containing text on some topic or domain.

* [സഞ്ചി]{lang=ml} `saFci` (bag)  
    A prototype of this predicate can be an object made of cloth, paper or polythene, in the rough shape of a container, capable of keeping things inside, and having handles to hold.

## Stereotype
The stereotype of a predicate is a list of the characteristic features of things to which it may be applied. For example,  

* [പേന]{lang=ml} `pena` (pen)  
    The stereotype of this predicate can be (i) long and thin, (ii) containing ink, (iii) capable of use for writing on some surface.

* [മേശ]{lang=ml} `meSa` (table)  
    The stereotype of this predicate can be (i) made of wood or plastic, (ii) having a flat surface, (iii) having 3 or more legs.

* [വാതിൽ]{lang=ml} `vAwil` (door)  
    The stereotype of this predicate can be (i) taller than it is wide, (ii) having hinges, (iii) forms the path between two rooms or between the inside and outside (of a cupboard or house), (iv) made of metal or wood.

## Paraphrase
Two propositions are called paraphrases of each other if they have the same set of entailments, or if they entail each other. For example,  

* [ഇത് ചെയ്യണം]{lang=ml} `iw ceVyyaNaM` (this has to be done) vs.  
    [ഇതാണ് ചെയ്യേണ്ടത്]{lang=ml} `iwAN ceVyyeNtaw` (this is what has to be done)

* [അവൻ നിശ്ശബ്ദനായി]{lang=ml} `avan niSSabxanAyi` (he became silent) vs.  
    [അവൻ ഒന്നും പറയാതായി]{lang=ml} `avan oVnnuM parYayAwAyi` (literally "he became not saying anything" = "he became silent")

* [ഞാൻ കാരണം അവൾ താമസിച്ചു]{lang=ml} `FAn kAraNaM avalY wAmasiccu` (because of me, she was late) vs.  
    [ഞാൻ അവളെ താമസിപ്പിച്ചു]{lang=ml} `FAn avalYeV wAmasippiccu` (I made her late)

## Entailment
A proposition $X$ is said to entail another proposition $Y$ if $Y$ must be true whenever $X$ is true. In other words, $X$ being true is a sufficient condition for $Y$ to be true. For example,  

* [നിങ്ങൾ ഇവനെ കൊന്നു]{lang=ml} `niffalY ivaneV koVnnu` (you (pl.) killed him) entails  
    [ഇവൻ മരിച്ചു]{lang=ml} `ivan mariccu` (he died)
    
* [എല്ലാ മനുഷ്യരും മരണമുള്ളവരാണ്]{lang=ml} `eVllA manuRyaruM maraNamulYlYavarAN` (all humans are mortal) entails  
    [സോക്രാറ്റീസ് മരണമുള്ളവനാണ്]{lang=ml} `sokrarYrYIs maraNamulYlYavanAN` (Socrates is mortal)

* [അവർ ദിവസേന കോളേജിലേക്ക് പോകാറുണ്ട്]{lang=ml} `avar xivasena kolYejilekk pokArYuNt` (they go to college every day) entails  
    [അവർ നാളെ കോളേജിലേക്ക് പോകും]{lang=ml} `avar nAlYeV kolYejilekk pokuM` (they will go to college tomorrow)

## Sense Properties of Sentences
We will consider examples of three sense properties: analyticity, syntheticity and contradiction.

### Analytic Sentences
An analytic sentence is one which must logically be always true, due to the relations among the senses of the predicates involved in it. For example,  

* [ആ അവിവാഹിതൻ കല്യാണം കഴിച്ചിട്ടില്ല]{lang=ml} `A avivAhiwan kalyANaM kalYYiccittilla` (that bachelor has not married)

* [പ്ലേറ്റോ അറിസ്റ്റോറ്റലിന്റെ അധ്യാപകനാണെങ്കിൽ അറിസ്റ്റോറ്റൽ പ്ലേറ്റോവിന്റെ ശിഷ്യനാണ്]{lang=ml} `plerYrYo arYisrYrYorYrYalinrYeV aXyApakanANeVfkil arYisrYrYorYrYal plerYrYovinrYeV SiRyanAN` (if Plato is Aristotle's teacher, then Aristotle is Plato's student)

* [നിരീശ്വരമതക്കാർക്ക് ഈശ്വരനിൽ വിശ്വാസമില്ല]{lang=ml} `nirISvaramawakkArkk ISvaranil viSvAsamilla` (atheists do not believe in God)

### Synthetic Sentences
A synthetic sentence is one which may or may not be true, depending on the circumstances. For example,  

* [സൂര്യൻ കിഴക്കുദിക്കിൽ ഉദിക്കും]{lang=ml} `sUryan kilYYakkuxikkil uxikkuM` (the Sun rises in the east)

* [മനുഷ്യർ മരണമുള്ളവരാണ്]{lang=ml} `manuRyar maraNamulYlYavarAN` (humans are mortal)

* [അദ്ധ്യാത്മരാമായണം എഴുതിയത് തുഞ്ചത്ത് എഴുത്തച്ഛനാണ്]{lang=ml} `axXyAwmarAmAyaNaM eVllYuwiyaw wuFcaww eVlYYuwwacCanAN` (Thunchath Ezhuthachan wrote the Adhyatma Ramayanam)

### Contradictions
A contradiction is a sentence which must necessarily be false, again due to the relations among the senses of the predicates involved in it. For example,  

* [ആ കഷണ്ടിയുടെ തലമുടി ചുവന്നതാണ്]{lang=ml} `A kaRaNtiyuteV walamuti cuvannawAN` (that bald person's hair is red)

* [എന്റെ ചങ്ങാതി എന്റെ ശത്രുവാണ്]{lang=ml} `eVnrYeV caffAwi eVnrYeV SawruvAN` (my friend is my enemy)

* [ഐമൂന്ന് പതിനേഴ്]{lang=ml} `EmUnn pawinelYY` (five times three is seventeen)

# Question 2
## Synonymy
Two predicates are said to be synonymous if they have the same senses. For example,  

* [പൂ]{lang=ml} `pU` and [പുഷ്പം]{lang=ml} `puRpaM` (flower)

* [കസേര]{lang=ml} `kasera` and [കസാല]{lang=ml} `kasAla` (chair)

* [പൊന്ന്]{lang=ml} `poVnn` and [തങ്കം]{lang=ml} `wafkaM` (gold)

* [അമ്പിളി]{lang=ml} `anpilYi` and [ചന്ദ്രൻ]{lang=ml} `candran` (moon)

* [പുസ്തകം]{lang=ml} `puswakaM` and [കിത്താബ്]{lang=ml} `kiwwAb` (book)

## Binary Antonyms
Binary antonyms are predicates which occur in pairs and cover all possibilities. For example,

* [ചൂട്]{lang=ml} `cUt` (heat) and [തണുപ്പ്]{lang=ml} `waNupp` (cold)

* [പഴയ]{lang=ml} `palYYaya` (old) and [പുതിയ]{lang=ml} `puwiya` (new)

* [രാത്രി]{lang=ml} `rAwri` (night) and [പകൽ]{lang=ml} `pakal` (daytime)

* [വലിയ]{lang=ml} `valiya` (big) and [ചെറിയ]{lang=ml} `ceVrYiya` (small)

* [അമ്മ]{lang=ml} `amma` (mother) and [അച്ഛൻ]{lang=ml} `acCan` (father)

## Converses
Converses are predicates which occur in pairs and describe the same relationship from different perspectives. For example,

* [മൂത്ത]{lang=ml} `mUwwa` (elder) and [ഇളയ]{lang=ml} `ilYaya` (younger)

* [അദ്ധ്യാപകൻ]{lang=ml} `axXyApakan` (teacher) and [ശിഷ്യൻ]{lang=ml} `SiRyan` (student)

* [രാജാവ്]{lang=ml} `rAjAv` (king) and [പ്രജ]{lang=ml} `praja` (subject)

* [അടുത്ത]{lang=ml} `atuwwa` (next) and [കഴിഞ്ഞ]{lang=ml} `kalYYiFFa` (previous)

* [മുകളിൽ]{lang=ml} `mukalYil` (above) and [താഴെ]{lang=ml} `wAlYYeV` (below)

## Multiple Compatibility
If a semantic system is divided into multiple fields, the predicates describing each of these fields exhibit multiple compatibility. For example,

* [വടക്ക്]{lang=ml} `vatakk` (north), [തെക്ക്]{lang=ml} `weVkk` (south), [കിഴക്ക്]{lang=ml} `kilYYakk` (east), [പടിഞ്ഞാറ്]{lang=ml} `patiFFArY` (west)

* [മേടം]{lang=ml} `metaM`, [ഇടവം]{lang=ml} `itavaM`, [മിഥുനം]{lang=ml} `miWunaM`, [കർക്കിടകം]{lang=ml} `karkkitakaM`, [ചിങ്ങം]{lang=ml} `ciffaM`, [കന്നി]{lang=ml} `kanni`, [തുലാം]{lang=ml} `wulAM`, [വൃശ്ചികം]{lang=ml} `vQScikaM`, [ധനു]{lang=ml} `Xanu`, [മകരം]{lang=ml} `makaraM`, [കുംഭം]{lang=ml} `kuMBaM`, [മീനം]{lang=ml} `mInaM` (months of the calendar)

* [പ്രതിപദം]{lang=ml} `prawipaxaM`, [ദ്വിതീയ]{lang=ml} `xvitIya`, [തൃതീയ]{lang=ml} `wQwIya`, [ചതുർത്ഥി]{lang=ml} `cawurwWi`, [പഞ്ചമി]{lang=ml} `paFcami`, [ഷഷ്ഠി]{lang=ml} `RaRWi`, [സപ്തമി]{lang=ml} `sapwami`, [അഷ്ടമി]{lang=ml} `aRtami`, [നവമി]{lang=ml} `navami`, [ദശമി]{lang=ml} `waSami`, [ഏകാദശി]{lang=ml} `ekAxaSi`, [ദ്വാദശി]{lang=ml} `xvAxaSi`, [ത്രയോദശി]{lang=ml} `wrayoxaSi`, [ചതുർദ്ദശി]{lang=ml} `cawurxxaSi`, [പൗർണ്ണമി]{lang=ml} `pOrNNami`, [അമാവാസി]{lang=ml} `amAvAsi` (days of the fortnight)

* [ഋഗ്വേദം]{lang=ml} `QgvexaM` (Rgveda), [സമവേദം]{lang=ml} `samavexaM` (Samaveda), [യജുർവ്വേദം]{lang=ml} `yajurvvexaM` (Yajurveda), [അഥർവ്വവേദം]{lang=ml} `aWarvvavexaM` (Atharvaveda)

* [പിതാവ്]{lang=ml} `piwAv` (The Father), [പുത്രൻ]{lang=ml} `puwran` (The Son), [പരിശുദ്ധാത്മാവ്]{lang=ml} `pariSuxXAwmAv` (The Holy Spirit)

## Hyponyms
Hyponyms are pairs of predicates such that one predicate's meaning is included in the other's. For example,

* [പശു]{lang=ml} `paSu` (cow) vs. [മൃഗം]{lang=ml} `mQgaM` (animal)

* [നോവൽ]{lang=ml} `noval` (novel) vs. [പുസ്തകം]{lang=ml} `puswakaM` (book)

* [റോജ]{lang=ml} `rYoja` (rose) vs. [പൂ]{lang=ml} `pU` (flower)

* [മലയാളി]{lang=ml} `malayAlYi` (Malayali) vs. [ഇന്ത്യക്കാരൻ]{lang=ml} `inwyakkAran` (Indian)

* [ഷർട്ട്]{lang=ml} `Rartt` (shirt) vs. [തുണി]{lang=ml} `wuNi` (cloth/item of clothing)

## Polysemy
Polysemy is the property of predicates which have more than one sense, but whose senses are all closely related. For example,

* [മണ്ണ്]{lang=ml} `maNN` (soil, Earth)

* [കമ്പി]{lang=ml} `kanpi` (wire, telegram)

* [വാക്ക്]{lang=ml} `vAkk` (word, promise)

* [സമ്മാനം]{lang=ml} `sammAnaM` (prize, gift)

* [കണക്ക്]{lang=ml} `kaNakk` (account, figure)

# Question 3
A referring expression is a predicate that is used with a particular referent in mind – one or more persons, objects or concepts.  

A deictic expression is any expression that takes some element of its meaning from the context of the utterance in which it is used.  

Consider the following 4 examples:

* [**നീ** വന്നത് നന്നായി]{lang=ml} `nI vannaw nannAyi` (it's good that **you** came)  
    In this sentence, [നീ]{lang=ml} `nI` (you (sg.)) is a referring expression (as it has definite referent, the addressee).  
    It is also a deictic expression (as the actual identity of the addressee depends on the context).
    
* [**൧൭൫൭-ലെ തിരുവിതാങ്കൂർ രാജാവ് അനിഴം തിരുനാൾ മാർത്താണ്ട വർമ്മ** ലോകപ്രിയർ ആയിരുന്നു]{lang=ml} `1757-leV wiruviwAfkUr rAjAv anilYYaM wirunAlY mArwwANta varmma lokapriyar Ayirunnu` (**The Maharaja of Travancore in 1757, Anizham Thirunal Marthanda Varma**, was popular)  
    In this sentence, [൧൭൫൭-ലെ തിരുവിതാങ്കൂർ രാജാവ് അനിഴം തിരുനാൾ മാർത്താണ്ട വർമ്മ]{lang=ml} (The Maharaja of Travancore in 1757, Anizham Thirunal Marthanda Varma) is a referring expression as it has a definite referent.  
    However, it is *not* a deictic expression. In any context, it would refer to the same person, Maharaja Anizham Thirunal Marthanda Varma.

* [**ഇന്ന്** എനിക്ക് ക്ലാസ്സ് ഇല്ല]{lang=ml} `inn eVnikk klAss illa` (**today** I don't have class)  
    Here, [ഇന്ന]{lang=ml} `inn` (today) is *not* a referring expression. Syntactically, it is an adverb and therefore has no referent.  
    It is, however, a deictic expression. It makes a statement about the day on which the utterance is made.  
    
* [കുപ്പി **ഏകദേശം** നിറഞ്ഞു]{lang=ml} `kuppi ekaxeSaM nirYaFFu` (the bottle is **almost** full)  
    In this sentence, [ഏകദേശം]{lang=ml} `ekaxeSaM` (almost) is *not* a referring expression. It has no referent in the real world (physical or virtual).  
    It is also *not* a deictic expression. In any utterance its meaning is independent of the context and makes the same modification to the meaning of the verb.
    
Thus, it is clear that referring expressions and deictic expressions are distinct and independent classifications which may or may not overlap.
