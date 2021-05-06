Nouns
Nouns in the Turkana language are things.


Numerals
Numerals in the Turkana language are numbers.


Verbs
Verbs in the Turkana language are actions.



Prefixes
Prefixes in the Turkana language are bound to beginning of other words.



Adjectives
Adjectives in the Turkana language describe things.


Pronouns
Pronouns in the Turkana language are references to things.



# The Turkana morphophonological/twolc rules file 








# Rules


**Where ATR+ is possible**  

**Where ATR- is possible**  

**Disallow broken harmonies plus**  

**Disallow broken harmonies minus**  

**Require ATR+ No Low**  

**Require ATR- No Low**  

**Where ATR+ is required**  

**Where ATR- is required**  


**Itive suffix after +ATR**  

# Symbol affixes





Noun inflection
The Turkana language nouns inflect in cases.



Proper noun inflection
The Turkana language proper nouns inflect in the same cases as regular
nouns, but with a colon (':') as separator.



Verb inflection
The Turkana language verbs inflect in persons.











Adjective inflection
The Turkana language adjectives compare.




Morphology
This is a Turkana morphology for proof-of-concept demo of ATR harmony
among other things

 # Definitions for Multichar_Symbols

 * +Symbol = independent symbols in the text stream, like £, €, ©

## Analysis symbols
We've ignored analyses for this part of proof-of-concept


Morphophonology
The ATR harmony affects following set of vowels, the leftmost being the
initial (neutral) and others downward modified in clockwise order.

And following triggers to control the ATR dominant overrides and ATR
stuff

## Flag diacritics
We have manually optimised the structure of our lexicon using following
flag diacritics to restrict morhpological combinatorics - only allow compounds
with verbs if the verb is further derived into a noun again:
 |  @P.NeedNoun.ON@ | (Dis)allow compounds with verbs unless nominalised
 |  @D.NeedNoun.ON@ | (Dis)allow compounds with verbs unless nominalised
 |  @C.NeedNoun@ | (Dis)allow compounds with verbs unless nominalised

For languages that allow compounding, the following flag diacritics are needed
to control position-based compounding restrictions for nominals. Their use is
handled automatically if combined with +CmpN/xxx tags. If not used, they will
do no harm.
 |  @P.CmpFrst.FALSE@ | Require that words tagged as such only appear first
 |  @D.CmpPref.TRUE@ | Block such words from entering ENDLEX
 |  @P.CmpPref.FALSE@ | Block these words from making further compounds
 |  @D.CmpLast.TRUE@ | Block such words from entering R
 |  @D.CmpNone.TRUE@ | Combines with the next tag to prohibit compounding
 |  @U.CmpNone.FALSE@ | Combines with the prev tag to prohibit compounding
 |  @P.CmpOnly.TRUE@ | Sets a flag to indicate that the word has passed R
 |  @D.CmpOnly.FALSE@ | Disallow words coming directly from root.

Use the following flag diacritics to control downcasing of derived proper
nouns (e.g. Finnish Pariisi -> pariisilainen). See e.g. North Sámi for how to use
these flags. There exists a ready-made regex that will do the actual down-casing
given the proper use of these flags.
 |  @U.Cap.Obl@ | Allowing downcasing of derived names: deatnulasj.
 |  @U.Cap.Opt@ | Allowing downcasing of derived names: deatnulasj.

our examples are verbs, but this is prefixing language, so we'll start from
there.




We describe here how abbreviations are in Turkana are read out, e.g.
for text-to-speech systems.

For example:

 * s.:syntynyt # ;  
 * os.:omaa% sukua # ;  
 * v.:vuosi # ;  
 * v.:vuonna # ;  
 * esim.:esimerkki # ; 
 * esim.:esimerkiksi # ; 


















































% komma% :,      Root ;
% tjuohkkis% :%. Root ;
% kolon% :%:     Root ;
% sárggis% :%-   Root ; 
% násti% :%*     Root ; 

