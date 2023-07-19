# Blocklists - with proper mastodon headers
Blocklist data but with proper mastodon headers in format

The headers are `#domain,#severity,#reject_media,#reject_reports,#public_comment,#obfuscate`
# Guide to the lists
Each list blocks more unwanted domains, but ANY list will block Meta's Threads by default.
* `fedinuke-mastodon.csv` - Seirdy's `FediNuke.txt` list in importable CSV format. Could be considered as a likely "default" blocklist. (174 entries)
* `blocked_domains_threadsonly.csv` - A domain blocking list only containing Meta's Threads.
* `blocked_domains_origmain_mastodon.csv` - The original "main" list that was compiled by looking up the list of intances for Mastodon, Misskey and Calckey. (73 entries)
* `blocked_domains_mainandfedinuke-mastodon.csv` - The "main" list and the Fedinuke list merged into one list. (240 entries)
* `blocked_domains_mainandfedinuke_100pct-mastodon.csv` - The "main" list, Fedinuke, and Oliphant's 100 percent list merged into one list. (258 entries)
* `blocked_domains_mainandfedinuke_100pct_gardenfence-mastodon.csv` - The "main" list, Fedinuke, and Oliphant's 100 percent, and Gardenfence list merged into one list. (332 entries)
* `blocked_domains_mainandfedinuke_100pct_gardenfence_pleromaenvs-mastodon.csv` - The "main" list, Seirdy's Fedinuke, BirdsiteLive, a portion of the `pleroma.envs.net` list, and Oliphant's 100 percent, Gardenfence list merged into one list. (1333 entries)

# Methodology used to construct the "main" list:
Some of the URLs were trivially easy to classify for reasons such as
* Being inherently based on a NSFW term
* The presence of the `crypto` word and related terms in URL
* Political terms present in URL
* Innuendo in URL
But, some of them were chosen because:
* It's someone's private speech bubble only open to their relatives or it's a single-user instance.
* It's a shitposting instance, and provides no real value to discussion.   
