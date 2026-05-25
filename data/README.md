# Name Data

`first-names.json` contains names derived from Social Security Administration baby-name data. The official SSA download was blocked from this environment, so this file was generated from the `atleast500.txt` processed mirror at:

https://github.com/hackerb9/ssa-baby-names

`last-names.json` contains the top 10,000 surnames from the U.S. Census Bureau 2010 surname data:

https://www2.census.gov/topics/genealogy/2010surnames/names.zip

`email-words.json` is a hand-curated local word list for generating synthetic email addresses.

`email-domains.json` is a hand-curated list of common consumer email domains. It intentionally avoids workplace/company domains.

`score-chase-feedback.json` contains Score Chase feedback thresholds and message pools. The app uses the first category where the last 10-item correct count is at or below `maxCorrect`, then picks one message from that category at random.

The app loads these files locally so the practice tool does not depend on the internet at runtime when served from this folder.
