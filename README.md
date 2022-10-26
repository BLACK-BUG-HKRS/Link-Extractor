# All-Website-Links-Extractor
Extract all website links using this python script

to use this:

- `pip install -r requirements.txt`

```
python link_extractor.py --help
```

output: 

```
usage: link_extractor.py [-h] [-m MAX_URLS] url

Link Extractor Tool with Python

positional arguments:
  url                   The URL to extract links from.

options:
  -h, --help            show this help message and exit
  -m MAX_URLS, --max-urls MAX_URLS
                        Number of max URLs to crawl, default is 30.
```

For instance, to extract all links from 2 first URLs appeared in github.com:

```
python link_extractor.py https://github.com -m 2
```

This will result in a large list, here is random chosen links:

```
...
[*] Internal link: https://github.com/about/diversity
[*] Internal link: https://socialimpact.github.com/
[*] Internal link: https://shop.github.com
[!] External link: https://twitter.com/github
[!] External link: https://www.facebook.com/GitHub
[!] External link: https://www.linkedin.com/company/github
[!] External link: https://www.youtube.com/github
[!] External link: https://www.twitch.tv/github
[!] External link: https://www.tiktok.com/@github
[*] Internal link: https://github.com/github
[*] Internal link: https://docs.github.com/en/github/site-policy/github-terms-of-service
[*] Internal link: https://docs.github.com/en/github/site-policy/github-privacy-statement
[*] Internal link: https://github.com/github/site-policy/pull/582
[*] Internal link: https://github.com/site-map
[*] Internal link: https://github.com/git-guides
[*] Crawling: https://resources.github.com/devops/fundamentals/devsecops/
[*] Internal link: https://github.com/enterprise/trial
...
```

This will also save these URLs in `github.com_external_links.txt` for external links and `github.com_internal_links.txt` for internal links.
