# `nic.in` subdomain tracker

The repository contains list of subdomains/web applications maintained by National Informatics Centre (NIC) under Govt. of India. As this tool uses a DNS protocol level technique to enumerate the subdomains, the coverage is 100% i.e.the file contains all the valid and active subdomains under `nic.in` for a given date.

- `all_subdomains_{time_stamp}.txt` contains list of subdomains under `nic.in` domain for a given day.
- `changes_on_{time_stamp}.txt` contains list of deleted and added subdomains on a given day compared to previous day.


## How is this data gathered?

Nothing fancy. Once a day, a Python script runs on my machine that - 

1. Uses a specific DNS enumeration technique to gather all the subdomains
2. Pushes the file with the list of subdomains for that day to this git repo

## Future plans

1. ~~Diff files of today/previous day to get a list of newly added subdomains for the day~~
2. Create a Twitter bot to notify when there is a new subdomain

## Frequently Asked Questions (FAQs)

### Why aggregate subdomains/web applications by NIC?

> National Informatics Centre (NIC) provides infrastructure to help support the delivery of Indian government IT services and the delivery of some of the initiatives of Digital India.

As per my knowledge, unlike [other](https://github.com/GSA/govt-urls) [government agencies](https://www.gov.uk/government/publications/list-of-gov-uk-domain-names), NIC doesn't maintain a directory of all the subdomains/web applications.

Having a list of subdomains/web applications maintained by NIC will help research organisations/think tanks that perform studies on those domains/websites such as verify their privacy protection using scoring tools like [Webbkoll](https://webbkoll.dataskydd.net) etc.
