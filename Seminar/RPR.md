# Abstract
* two approaches
    - naive – traverse parse tree
    - semantic analysis system

# Introduction
## -
* importance
* two approaches
    - naive
    - total semantic analysis system
* analytic

## Review of the Natural Language Processing Literature
* syntactic constraints on (non-)coreferentiality
* Winograd (1972) like first one
* Rieger (1974) properties of entities
* Charniak (1972) bruh
* Wilks (1974) partial solution

# The Syntactic Approach: The Naive Algorithm
## The Algorithm
* surface parse tree = structure (CFG, X-bar)
* traversal looking for NP with correct GN
    - begin at dominating NP
    - go up to first NP/S [path p, node X]
    - traverse branches to the left of p, L-R, breadth first. propose any NP with NP/S between it and X.
    - if X is the highest S node, traverse previous sentences in order in the same way, proposing similarly. else move on
    - from X, go up the tree to the first NP/S [p and X]
    - if X is an NP and p did not pass through the N-bar dominated by X, propose X
    - traverse all branches to the left of p, L-R, breadth first. propose any NP
    - if X is S, traverse all branches to the right of p, L-R, breadth first. stop at NP/S nodes. propose any NP
    - goto 4

* 2-3 reflexive
* 5-9 cycle
* 4 prev sentences

* additional selectional constraints: dates, places, large fixed objects can't move

* good
    - collects selectionally compatible entities for "they"
    - conjunction of plurals > either one
    - recovers syntactically recoverable material, records coreference

* bad
    - no sentence pronominalisation

## Relation of the Algorithm to Results from the Generative Transformational Tradition
* non-coreferentiality conditions
* not the same as identifying antec from remaining
* mechanism with these conds acts as filter
* conds
    - non-reflexive pronoun and antec cannot occur in the same simplex sent
    - antec must precede/command pronoun (neither dominates and S that dominates former doesnt *immediately* (but does) dominate latter)

## Stastical Results
* 88.3%
* with selec constraints, 91.7%
* lies lmao
* Klapholz and Lockman (1975) n
    - Charniak (1972) n = 5

# The Semantic Approach
## A System for Semantic Analysis of English Texts
* assume world knowldge is available as predicate calculus axioms
* semantic operations draw inferences from axioms
* inferences interpret words, determine relations, resolve anaphora
* text -> syntactically analysed with (non-)coreference constraints
* logical notation:
    - set of entities
    - kernel statements = properties of entities
    - which statement is asserted and which is subordinate
        `on (X1|boy(X1), X2|roof(X2,X3|building(X3)))`
        = `on(X1,X2), boy(X1), roof(X2,X3), building(X3)`
- lexicon contains axioms
- inferences are drawn forward/backward as needed
- axioms grouped by salience according to anticipated relevance

## The Semantic Operations and Pronoun Resolution
* 4 semantic ops
    - detecting intersentence connectives
        - common patterns
        - inference from two sentences
    - predicate interpretation
        - definition = inferences to be drawn + modification of them
    - knitting
        - redundancy is expected
        - same statements merged
    - identifying entities
        - hierarchy according to degree of specification
* expensive search op
* bidirectional search (Pohl 1971) from naive antecedent and from pronoun
* shallow check for propert compatibility
* among many possibilities, candidate which maximised redundancy simplest

# Examples of the Semantic Approach to Pronoun Resolution
## -
## -
## -
## -

# Summary
* three steps
    - intersentence relation operation with knitting
    - predicate interpretation together with knitting
    - bidirectional search
* we can add
    - competition among entities of correct GN
    - apply naive (always gives answer)
* usually accomplished by first two steps
