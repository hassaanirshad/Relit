# Deriving SemanticCheckers from Tests to Detect Silent Failures in Production Distributed Systems

## Abstract
Production distributed systems provide rich features, but vari-
ousdefectscancauseasystemtosilentlyviolateitssemantics
without explicit errors. Such failures cause serious conse-
quences. Yet, they are extremely challenging to detect, as
it requires deep domain knowledge and substantial manual
effortsto write goodcheckers.
Inthispaper,weexplorea novelapproachthat directly de-
rivessemanticcheckersfromsystemtestcode.Wefirstpresent
a large-scale study on existing system test cases. Guided by
the study findings, we develop T2C, a framework that uses
static and dynamic analysis to transform and generalize a test
intoaruntimechecker.WeapplyT2C onfourlarge,popular
distributedsystemsandsuccessfullyderivetenstohundredsof
checkers.Thesecheckersdetect15outof20real-world silent
failures we reproduce andincursmall runtimeoverhead.

## People

