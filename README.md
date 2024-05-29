# Spam Blocklist

This repository contains curated lists of IP addresses that are known for spam activities. The lists are dynamically updated using Cloudflare Workers.

## Files in the Repository

1. **merged-list.txt**
   - This file contains a merged list of IP addresses from both the `nixspam-ip.txt` and `sslipblacklist-ips.txt` files.
   
2. **nixspam-ip.txt**
   - This file contains IP addresses from the Nixspam iX spam protection feed.

3. **sslipblacklist-ips.txt**
   - This file contains IP addresses from the SSBL SSL botnet IPs feed.

## Dynamic Cloudflare Workers

The following Cloudflare Workers are used to dynamically curate and update the lists:

- Nixspam IP List: [https://ip-blacklist.corale.workers.dev/nixspam-ip.txt](https://ip-blacklist.corale.workers.dev/nixspam-ip.txt)

- SSBL IP List: [https://ip-blacklist.corale.workers.dev/sslipblacklist-ips.txt](https://ip-blacklist.corale.workers.dev/sslipblacklist-ips.txt)

- Merged IP List: [https://ip-blacklist.corale.workers.dev/merged-list.txt](https://ip-blacklist.corale.workers.dev/merged-list.txt)


These workers ensure that the lists are always up-to-date with the latest data.

## How to Use

You can use these lists to block known spam IP addresses in your firewall or security settings to enhance your protection against spam and botnet activities.

Feel free to contribute by submitting pull requests or opening issues for any suggestions or improvements.
