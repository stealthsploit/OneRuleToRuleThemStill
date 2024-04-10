# OneRuleToRuleThemStill

An revamped and optimised version of [OneRuleToRuleThemAll](https://github.com/stealthsploit/Optimised-hashcat-Rule).

OneRuleToRuleThemStill now has a ~~5%~~ ~6.9% reduction in rules (52,000 down to ~~49,465~~ 48,414) with 0% performance loss against the Lifeboat and LastFM data breaches.

Updates:
- De-duplication of resulting candidate generation (previously literal strings only)
- Added LastFM breach dataset (~21m unique hashes) for larger/better modelling
- Common non-matching rules removed (Lifeboat and LastFM)
- Ordered by frequency against LastFM

More detail can be found in the blog: https://in.security/2023/01/10/oneruletorulethemstill-new-and-improved/

<h2>Credits</h2>
As well as several default hashcat rules (including generated2 by https://github.com/evilmog), the following non-default rule sets were used in testing to create the original rule:

- https://github.com/praetorian-inc/Hob0Rules (d3adhob0.rule, hob064.rule)
- http://contest-2010.korelogic.com/rules-hashcat.html (KoreLogicRulesPrependRockYou50000)
- https://github.com/NSAKEY/nsa-rules (__NSAKEY.v2.dive.rule_)

The tool https://github.com/mhasbini/duprule assisted during development.

Many thanks to https://github.com/hashcat/hashcat and it's team for their continual great work.

<h2>License</h2>
Individual rules used will use their respective licenses if present. Additional custom rules are MIT licensed.
