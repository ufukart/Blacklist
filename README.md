# Blacklist 🛡️

A comprehensive, regularly updated IP blacklist compiled from multiple trusted security sources for blocking malicious traffic.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Update Status](https://img.shields.io/badge/Status-Actively%20Maintained-green.svg)](https://github.com/ufukart/Blacklist)
[![Last Updated](https://img.shields.io/github/last-commit/ufukart/Blacklist)](https://github.com/ufukart/Blacklist/commits/main)
![Ips](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/ufukart/Blacklist/main/.badges/lines.json&cacheSeconds=3600)
![Blacklist File Size](https://img.shields.io/github/size/ufukart/Blacklist/blacklist.txt)
![Visitors](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Fufukart%2FBlacklist%2F&label=HITS&countColor=%23263759&style=flat)
[![Donate](https://img.shields.io/badge/Donate-PayPal-blue.svg)](https://www.paypal.com/donate/?business=53EHQKQ3T87J8&no_recurring=0&currency_code=USD)

## 📋 Description

This repository provides a curated IP blacklist aggregated from multiple reputable security sources. The list is automatically updated at regular intervals to ensure maximum protection against:

- **Malicious attackers** and botnet IPs
- **Brute force attempts** and dictionary attackers  
- **Spam sources** and compromised hosts
- **Tor exit nodes** (for services requiring blocking)
- **Known bad actors** from threat intelligence feeds

## 🚀 Quick Start

### Direct Download
```bash
# Download the latest blacklist
curl -O https://raw.githubusercontent.com/ufukart/Blacklist/main/blacklist.txt

# Or using wget
wget https://raw.githubusercontent.com/ufukart/Blacklist/main/blacklist.txt
```

## 📊 Statistics

- **Total IPs**: ~270,000+ (varies with updates)
- **Update Frequency**: Every 6 hours
- **Sources**: 11 trusted security feeds
- **Format**: Plain text, one IP per line
- **Duplicates**: Automatically removed
- **Private IPs**: Filtered out (RFC 1918)

## 🔍 Data Sources

This blacklist aggregates data from the following trusted sources:

| Source | Description | Type |
|--------|-------------|------|
| [Project Honey Pot](https://www.projecthoneypot.org/) | Directory of Dictionary Attacker IPs | Malicious IPs |
| [Tor Project](https://check.torproject.org/) | Tor Exit Nodes | Anonymity Network |
| [BruteForceBlocker](https://danger.rulez.sk/projects/bruteforceblocker/) | Brute Force Attack IPs | Attack Prevention |
| [Spamhaus DROP](https://www.spamhaus.org/drop/) | Don't Route Or Peer List | Network Security |
| [C.I. Army](https://cinsscore.com/) | Malicious IP Intelligence | Threat Intelligence |
| [blocklist.de](https://lists.blocklist.de/) | Attack IP Database | Security Feed |
| [GreenSnow](https://blocklist.greensnow.co/) | Malicious IP List | Threat Detection |
| [FireHOL Level 1](https://iplists.firehol.org/) | High Confidence Threats | Threat Intelligence |
| [StopForumSpam](https://www.stopforumspam.com/) | Forum Spam IPs | Anti-Spam |
| [AbuseIPDB](https://www.abuseipdb.com/) | Community Reported Abuse | Crowdsourced Security |
| [RTBH](https://list.rtbh.com.tr/) | Remote Triggered Black Hole | Flexible, Reliable, and Sustainable RTBH (Remote Triggered Black Hole) Service |

## 📁 File Format

```
# Each line contains one IP address or CIDR block
192.168.1.100
10.0.0.0/8
203.0.113.0/24
```

- **Plain text format** for maximum compatibility
- **One IP/CIDR per line** 
- **No comments or headers** in the main file
- **IPv4 only** (IPv6 support planned)

## ⚠️ Important Notes

### Filtering Applied
- **Private IP ranges** are automatically excluded (10.x.x.x, 192.168.x.x, 172.16-31.x.x)
- **Localhost addresses** are filtered out
- **Multicast ranges** are excluded (224-239.x.x.x)
- **Duplicate entries** are removed

### Recommendations
- **Test thoroughly** before implementing in production
- **Monitor false positives** and adjust as needed
- **Keep backups** of your original firewall rules
- **Update regularly** for maximum effectiveness

### Disclaimer
This blacklist is provided "as-is" for informational and security purposes. Users are responsible for testing and validating the impact on their specific environments. The maintainers are not liable for any issues arising from the use of this data.

## 🔄 Update Schedule

- **Automatic updates**: Every 6 hours
- **Manual verification**: Weekly
- **Source validation**: Monthly
- **Documentation updates**: As needed

## 🤝 Contributing

Contributions are welcome! Please:

1. **Report false positives** via [Issues](https://github.com/ufukart/Blacklist/issues)
2. **Suggest new sources** with proper documentation
3. **Submit improvements** via Pull Requests
4. **Follow** the existing format and style

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

```
MIT License

Copyright (c) 2025 [Your Name]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## 📞 Support

- **Issues**: [GitHub Issues](https://github.com/ufukart/Blacklist/issues)
- **Discussions**: [GitHub Discussions](https://github.com/ufukart/Blacklist/discussions)
- **Security**: Report security issues privately via email

---

### 🌟 Star this repository if you find it useful!

**Keywords**: `blacklist`, `security`, `firewall`, `iptables`, `malware`, `botnet`, `threat-intelligence`, `cybersecurity`, `ip-blocking`, `network-security`
