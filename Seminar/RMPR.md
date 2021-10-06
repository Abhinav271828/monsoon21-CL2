# Abstract
* text has info to resolve ambiguities

# Introduction
* syntactic-based heuristic rule for almost 90%
* world knowledge for > 90%
* uses intersentential information, extracted by algo
* e.g. collocation patterms (= case frames),
    word frequency (= topic/focus)

# Three Factors for Evaluating Salience in Candidates
* collect NPs and select most preferable candidate by filtering and attaching preferences
* types
    - grammatical constraints: filter
    - salience rules: attach preference

## Collocation Patterns within a Source Text
* semantic constraints need knowledge
* collocation patterns = modifer-modifiee relationships
* word sense unified in discourse
* statements repeated
* case role persistence, syntactic parallelism

## Frequency of Repetition in Preceding Sentences
* object in focus is likely to be pronominalised
* frequency = focus

## Syntactic Position
* subjects > objects in Hobbs
* advantage is it assigns ranking for all NPs
* provides default value

# Implementation
* extraction of candidates
* selection of antecedent

## Extraction of Candidates
* GNP constraints in same sentence
* back until candidates in 2 sentences
* also filter modifiees of pronoun and args (non-reflexive)

## Selection of an Antecedent
### Preference According to the Existence of Identical Collocation Patterns in the Text
* constant value 3 for candidate that has identical pattern
* online synonym dictionary

### Preference According to the Frequency of Repetition in Preceding Sentences
* for each appearance of an NP with the same lemma, sum over 1/((number of sentences)+1)
* larger for closer and more freq occurrences

### Preference According to Syntactic Position
* closer sentence or nearer to beginning of same sentence
* L2R order, negative preference for distance
* similar to Hobbs' naïve one

## Example

# Results
* excluded pronominalised sentences
* identical pronouns have same antecedent
* avg number of candidates = 4.1
* 93.8%
* 82.7% with only syntactic position
* 60.7% with only frequncy
* 26.2% with only collocation but no wrong candidates

# Conclusion
* info in source text
* practical
