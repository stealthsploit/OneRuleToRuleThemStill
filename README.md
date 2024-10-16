# OneRuleToRuleThemStill

An revamped and optimised version of [OneRuleToRuleThemAll](https://github.com/stealthsploit/Optimised-hashcat-Rule).

OneRuleToRuleThemStill now has a ~~5%~~ ~6.9% reduction in rules (52,000 down to ~~49,465~~ 48,414) with 0% performance loss against the Lifeboat and LastFM data breaches.

Updates:
- De-duplication of resulting candidate generation (previously literal strings only)
- Added LastFM breach dataset (~21m unique hashes) for larger/better modelling
- Common non-matching rules removed (Lifeboat and LastFM)
- Ordered by frequency against LastFM

More detail can be found in the blog: https://in.security/2023/01/10/oneruletorulethemstill-new-and-improved/

<br>
<h2>Free Training</h2>

[![alt text](https://in.security/wp-content/uploads/2024/10/pw101logo.jpg)](https://in.security/technical-training/password-cracking/)

I developed **Password Cracking 101+1**, freely available on our website at https://in.security/technical-training/password-cracking/ 
- 4 hours of video content split into 15 parts with hands-on challenges
- Covers basic/traditional attack techniques as well as deeper, more creative attacks (such as delimited passphrases, foreign language, emojis, non-determinstic attacks etc)
- VM to download pre-built with training challenges and answers (VirtualBox OVA format)
- Password Cracking 101+1 training channel in our Discord server to chat
  
[![Discord Banner 3](https://discord.com/api/guilds/752813804491898910/widget.png?style=banner2)](https://discord.gg/5VpwE9YJ9R)

<br>
<h2>Credits</h2>
As well as several default hashcat rules (including generated2 by https://github.com/evilmog), the following non-default rule sets were used in testing to create the original rule:

- https://github.com/praetorian-inc/Hob0Rules (d3adhob0.rule, hob064.rule)
- http://contest-2010.korelogic.com/rules-hashcat.html (KoreLogicRulesPrependRockYou50000)
- https://github.com/NSAKEY/nsa-rules (__NSAKEY.v2.dive.rule_)

The tool https://github.com/mhasbini/duprule assisted during development.

Many thanks to https://github.com/hashcat/hashcat and it's team for their continual great work.

<h2>License</h2>
Individual rules used will use their respective licenses if present. Additional custom rules are MIT licensed.
