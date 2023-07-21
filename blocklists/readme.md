# Blocklists main folder

This folder contains the files that can be uploaded using the Import function of a Mastodon instance.

To import, use Preferences -> Import and export -> Import, Select option "Domain Blocking list" and select the CSV file to be imported.

If you're unsure whether to merge or overwrite, export your current blocking list (for backup) and proceed with merging.

For a better, properly headered version of these lists, check out the `mastodon` folder.
# Guide to the lists
Each list blocks more unwanted domains, but ANY list will block Meta's Threads by default.
* `blocked_domains_threadsonly.csv` - A domain blocking list only containing Meta's Threads.
*  `100.percent.csv` - Oliphant's 100 percent CSV file (70 entries) 
* `blocked_domains_origmain.csv` - The original "main" list that was compiled by looking up the list of instances for Mastodon, Misskey and Firefish (formerly Calckey). (73 entries)
* `fedinuke.csv` - Seirdy's `FediNuke.txt` list in importable CSV format. Could be considered as a likely "default" blocklist. (174 entries)
* `gardenfence.csv` - Oliphant's Gardenfence CSV file. (176 entries)
* `blocked_domains_mainandfedinuke.csv` - The "main" list and the Fedinuke list merged into one list. (240 entries)
* `blocked_domains_mainv2andfedinuke_100pct.csv` - The "main" list, Fedinuke, and Oliphant's 100 percent list merged into one list. (258 entries)
* `blocked_domains_main_fedinuke_100pct_gardenfence.csv` - The "main" list, Fedinuke, and Oliphant's 100 percent, and Gardenfence list merged into one list. (332 entries)
* `blocked_domains_mainv2andfedinuke_100pct_gardenfence_pleromaenvs.csv` - The "main" list, Seirdy's Fedinuke, BirdsiteLive, a portion of the `pleroma.envs.net` list, and Oliphant's 100 percent, Gardenfence list merged into one list. (1333 entries)
* `blocked_domains_mainandfedinuke_100pct_gardenfence_pleromaenvs_new_upl.csv` The largest list, updated with some new instances (1504 entries)

# Methodology used to construct the "main" list:
Some of the URLs were trivially easy to classify for reasons such as
* Being inherently based on a NSFW term
* The presence of the `crypto` word and related terms in URL
* Political terms present in URL
* Innuendo in URL
  
But, some of them were chosen because:
* It's someone's private speech bubble only open to their relatives / friends or it's a single-user instance.
* It's a shitposting instance, and provides no real value to discussion.
