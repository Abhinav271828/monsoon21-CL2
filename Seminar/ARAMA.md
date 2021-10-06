# Abstract
* multiple strategies from diff knowledg sources
* cognitive plausibility

# Introduction – The Complexity of Anaphora Resolution
* syntactic info plays central role in intrasentential anaphora
* semantic and pragmatic in intersentential anaphora
* integrates case frame semantics, global dialogue coherence structures

# The Problem – Semantics and Pragmatics Dominate
* 2 examples: cake and robot
* limited-domain anaphora : Hayes
* intrasentential anaphora : Webber
* multiple strategies: correspond to human judgments

# Multiple Resolution Strategies
* sentential syntax, case frame semantics, dialogue structure, general world knowledge

## Local Anaphor Constraints
* GNP

## Case-Role Semantic Constraints
* if case role filled by an anaphor, referent must satisfy constraints
* soft constraints are fine, if no hard

## Precondition/Postcondition Constraints
* action between referent and anaphor invalidates coreference

## Case-Role Persistence Preference
* corresponding semantic case role in earlier utterance
* generalised case-role (semantic) parallelism
* preference, not constraint
* semantic over syntactic (to susan = her), preference is stronger if they coincide

## Semantic Alignment Preference
* general form of above
* same "underlying action"
* pragmatic parallelism

## Syntactic Parallelism Preference
* like above two

## Syntactic Topicalisation Preference
* topicalised structures searched first
* preferential not categorical

## Intersentential Recency Preference
* search sentences in reverse chronological order

# Integrating the Strategies
* distinction between constraints and preferences
* apply constraints first, preferences to remaining
* if diff preferences suggest diff referents, ambiguity

# A Practical Implementation
* operates post facto on syntactic trees and semantic case frames of UP's output
* derive candidates by extracting NPs
* can change number of sentences

* preferences use voting method
* weight is given to each strategy
* case-role and local anaphor can be both constraining and preferring

* most preferred is unified with referent

* can resolve partially specified definite NPs
    - head noun same/hyponym
    - agreement
    - other slots unifiable or missing
