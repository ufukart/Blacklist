# Blacklist 🛡️

A comprehensive, automatically maintained IP blacklist compiled from multiple trusted threat intelligence sources to help protect servers, firewalls, and network infrastructure against malicious traffic.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Last Updated](https://img.shields.io/github/last-commit/ufukart/Blacklist)](https://github.com/ufukart/Blacklist/commits/main)
![IPs](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/ufukart/Blacklist/main/.badges/lines.json&cacheSeconds=3600)
![Blacklist File Size](https://img.shields.io/github/size/ufukart/Blacklist/blacklist.txt)
![Visitors](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Fufukart%2FBlacklist%2F&label=HITS&countColor=%23263759&style=flat)
[![Donate](https://img.shields.io/badge/Donate-PayPal-blue.svg)](https://www.paypal.com/donate/?business=53EHQKQ3T87J8&no_recurring=0&currency_code=USD)

---

## 🚫 Live Statistics

| Metric | Value |
| --------- | ------: |
| **Blocked IP Addresses** | **<!--IP_COUNT-->243778<!--/IP_COUNT-->** |
| **Update Frequency** | Every 6 hours |
| **Security Sources** | 11 |
| **Duplicates** | Automatically Removed |
| **Private IPs** | Filtered Out |
| **Format** | Plain Text |

> 🔥 The blacklist currently contains **<!--IP_COUNT-->243778<!--/IP_COUNT-->** unique malicious IP addresses, aggregated from 11 trusted security feeds and refreshed every 6 hours.

---

## 📥 Quick Download

```bash
curl -O https://raw.githubusercontent.com/ufukart/Blacklist/main/blacklist.txt
```

or

```bash
wget https://raw.githubusercontent.com/ufukart/Blacklist/main/blacklist.txt
```

---

## 📖 Description

This repository provides a continuously updated blacklist of malicious IPv4 addresses aggregated from multiple reputable threat intelligence providers.

**At a glance:**

- **Total IPs**: **<!--IP_COUNT-->243778<!--/IP_COUNT-->** (varies with updates)
- **Update Frequency**: Every 6 hours
- **Sources**: 11 trusted security feeds
- **Format**: Plain text, one IP per line
- **Duplicates**: Automatically removed
- **Private IPs**: Filtered out (RFC 1918)

The blacklist is designed for use with:

- Firewalls
- Intrusion Prevention Systems (IPS)
- Intrusion Detection Systems (IDS)
- Web Application Firewalls (WAF)
- Reverse Proxies
- Security Appliances
- Custom Security Scripts

The list includes addresses associated with:

- Malicious bots
- Brute-force attacks
- Spam sources
- Tor exit nodes
- Known attackers
- Threat intelligence feeds

---

## ✅ Compatible With

- iptables
- ipset
- nftables
- Fail2Ban
- CSF
- UFW
- pfSense
- OPNsense
- MikroTik

## 📂 File Format

```ipformats
1.2.3.4
8.8.8.8
203.0.113.0/24
...
```

- Plain text
- One IP/CIDR per line
- UTF-8
- IPv4 only
- No comments
- Ready for automation

---

## 📊 Data Sources

| Source | Description |
| -------- | ------------- |
| Project Honey Pot | Dictionary attacker IPs |
| Tor Project | Tor Exit Nodes |
| BruteForceBlocker | Brute-force attackers |
| Spamhaus DROP | High-risk networks |
| C.I. Army | Threat intelligence |
| blocklist.de | Attack database |
| GreenSnow | Malicious IP feed |
| FireHOL Level 1 | High-confidence threats |
| StopForumSpam | Spam IP database |
| AbuseIPDB | Community abuse reports |
| RTBH | Remote Triggered Black Hole |

---

## Why Blacklist?

✔ Multiple trusted sources

✔ Duplicate removal

✔ Private IP filtering

✔ Ready for production

✔ Free forever

✔ Updated every 6 hours

---

## 🔄 Update Schedule

The blacklist is automatically regenerated every **6 hours**.

Each update performs the following:

- Downloads all source lists
- Removes duplicates
- Filters private IP ranges
- Removes localhost addresses
- Removes invalid entries
- Generates the final blacklist

---

## ⚠️ Filtering Rules

The following entries are automatically excluded:

- RFC1918 Private Networks
- Localhost
- Link-local addresses
- Multicast ranges
- Duplicate entries
- Invalid records

---

## 💡 Usage Example

### iptables

```bash
while read ip; do
    iptables -A INPUT -s "$ip" -j DROP
done < blacklist.txt
```

### nftables

```bash
while read ip; do
    nft add element inet blacklist blocked_ips { $ip }
done < blacklist.txt
```

---

## 🤝 Contributing

Contributions are welcome.

You can help by:

- Reporting false positives
- Suggesting new security feeds
- Improving documentation
- Submitting pull requests

---

## 📄 License

Released under the MIT License.

---

## ❤️ Support

If this project helps protect your infrastructure, consider:

- ⭐ Starring the repository
- 🍴 Forking the project
- 💙 Supporting via PayPal

---

## Keywords

`blacklist` `ip-blacklist` `iptables` `firewall` `security` `malware` `botnet` `threat-intelligence` `cybersecurity` `network-security`
