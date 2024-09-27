# ANCVIVC---Advanced-Network-Configuration-of-several-Virtual-ISPs-and-Virtual-Companie

![TopologiaProjeto](https://github.com/user-attachments/assets/555a7b88-bba4-47c3-a411-437777bba9b0)

---
## Badges
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)

## Table of Contents
  - [Description](#description)
  - [Technologies used in this work](#technologies-used-in-this-work)
  - [Contributing](#contributing)
  - [License](#license)

## Description

ANCVIVC (Advanced Network Configuration of several Virtual ISPs and Virtual Companies) is a project that was developed for the Advanced Network Topics curricular unit of Computer Engineering course at the Polytechnic of Leiria. The final grade for this project was 16 (sixteen, on a scale of 0 to 20). The main aim of this project was to plan, design, configure and document a network scenario with several interconnected ISPs and provide connectivity to a business customer. The tasks of designing and configuring the ISP network were carried out using the GNS3 application.

Some of the requirements implemented to achieve the objectives were:

- **IPv4 addressing optimised according to the needs of the ISPs**

- **IPv6 addressing optimised in all networks and correctly configured with GUA and Link-Local addresses**

- **Tier 1 was configured with OSPFv3 multi-area and the following areas were used:**
    - *Area 0 - Backbone*
    - *Area 1 - Standard*
    - *Area 2 - Stub*
    - *Area 3 - Totaly Stubby*
    - *Area 4 - NSSA*
    - *Area 5 - Totaly NSSA*
    - *Area 6 - Virtual Link*
- **Tier 2A, 3A, 3B were configured with OSPFv3 single-area**

- **Tier 2B has been configured with RIP and RIPng**

- **All Tiers were configured with BGP and iBGP, and Tier 1 used confederations due to its size**

- **Tier 3 traffic has always had a preference for going via Tier 2A and only Tier 2B in the event of a Tier 2A failure.**

- **The connections between Tier 3 and Tier 2 contained redundancy and parallel use of links**

- **The following features have been implemented in the corporate network:**
    - *NAT implementation*
    - *IPv4 addressing only*
    - *L3 VPN configuration over MPLS technology between the company's head office and one of its branches*

## Technologies used in this work
- **GNS3**
- **BGP and iBGP**
- **OSPFv3 with single-area and multi-area**
- **RIP and RIPng**
- **L3 VPN over MPLS**
- **NAT**

## Contributing
This project was developed by:
  - Duarte Bento Batista

## License
[GPL-3.0 license](../LICENSE)
