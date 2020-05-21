# barge
All aboard the triage barge!

# Initial thoughts
1. I get bored reading online articles, so I'm tryinmg to figure out a way to make it quicker to absorb the bloggosphere's intel. Perhaps a prioritised list of articles.

2. It is a sad fact (but a fact nonetheless) that headlines drive security operations. At least to some degree. In order to make sure you don't miss any obvious signals, it would be good if that list of articles reflected what most people were talking about.

3. Point `2` isn't as dumb as you might think...report volume and "known-known" reporting can imply an inverse of knowledge gaps. If we think of article references (to attack patterns, threat actors, etc) as sources of intel, albeit secondary/tertiary reporting, this can add signal to our threat knowledge base to direct inbtel operations / prioritise.

# So how about...

* Pull in 2 or more open source report feeds. Nothing crazy, bleepingcomputer, elreg, something...
* Capture sufficient provenance to understand sourcing, referenced articles, etc, in order to identifiy circular reporting, primary/secondary/tertiary/etc...
* Tokenize article contents using basic concordance / word bag theory
* Make use of some off-the-shelf NLP courtesy of google/amazon/someone. Local library (like sklearn) as a last resort
* Map the outputs to Mitre ATT&CK or similar, perhaps using sightingsDB, to grow the intel graph.

2 main outputs would be:
1. A prioritised article list for busy readers (most talked about, weak signals, potentially unique insight based on provenance, etc). Mostly already done, but not with the provenance approach, perhaps?
2. A growing intelligence graph that can show what threats everyone is currently talking about, helping make sure you aren't missing the key threats, but also identifying blindspots (map to your own vulnerabilities to recognise where you should invest lots of research!!)