# IANA YANG SIDs Registry YANG Modules

This repostory contains YANG Modules tracked by IANA YANG SIDs registry.
All of these modules have been allocated SID ranges but none of them
has a (even experimental) .sid file created/proposed.

I want to:
  - generate the .sid files based on RFC9595 recommendation (using PYANG)
  - analyze the generated outputs
  - try to come up with even better, partially hand-written, .sid files optimalized
    for message sizes.

# Repository structure
 - `auto/`
 - `optimal/`
 - `misc/`
 - `*.yang`


## Detailed description

Directory [`auto/`](auto) has `Makefile` and generated .sid files for all tracked modules.
See the `Makefile` for how the .sid files are genereted.

Directory [`optimal/`](optimal) contains optimized .sid files after the analysis. If the .sid file is missing
there, it has not been (most likely) analyzed yet.

In the [`misc/`](misc) directory, you can find modules not tracked by referenced IANA registry
but I think they should be part of the registry.

# Tracked modules
 | YANG Module                                       | revision   | Entry point | Size  | IANA .sid file | PYANG .sid file | optimized .sid file | source |
 | -----------                                       | --------   | ----------- | ----- | -------------- | --------------- | ------------------- | ------ |
 | [ietf-coreconf](ietf-coreconf.yang)               | 2026-03-02 | 1000 | 100 | `N/A` | [ietf-coreconf.sid](auto/ietf-coreconf.sid)               | `N/A` | [draft-ietf-core-comi](https://datatracker.ietf.org/doc/html/draft-ietf-core-comi/) |
 | [ietf-yang-types](ietf-yang-types.yang)           | 2025-12-22 | 1100 | 50 | `N/A` | [ietf-yang-types.sid](auto/ietf-yang-types.sid)           | `N/A` | [RFC9911](https://datatracker.ietf.org/doc/html/rfc9911) [YangModels/Yang/ietf-yang-types.yang](https://github.com/YangModels/yang/blob/main/standard/ietf/RFC/ietf-yang-types%402025-12-22.yang) |
 | [ietf-inet-types](ietf-inet-types.yang)           | 2025-12-22 | 1150 | 50 | `N/A` | [ietf-inet-types.sid](auto/ietf-inet-types.sid)           | `N/A` | [RFC9911](https://datatracker.ietf.org/doc/html/rfc9911) [YangModels/Yang/ietf-inet-types.yang](https://github.com/YangModels/yang/blob/main/standard/ietf/RFC/ietf-inet-types%402025-12-22.yang) |
 | [iana-crypt-hash](iana-crypt-hash.yang)           | 2014-08-06 | 1200 | 50 | `N/A` | [iana-crypt-hash.sid](auto/iana-crypt-hash.sid) | `N/A` | [RFC7317](https://datatracker.ietf.org/doc/html/rfc7317) [YangModels/Yang/iana-crypt-hash.yang](https://github.com/YangModels/yang/blob/main/standard/ietf/RFC/iana-crypt-hash%402014-08-06.yang) |
 | [ietf-netconf-acm](ietf-netconf-acm.yang)         | 2018-02-14 | 1250 | 50 | `N/A` | [ietf-netconf-acm.sid](auto/ietf-netconf-acm.sid)         | `N/A` | [RFC8341](https://datatracker.ietf.org/doc/html/rfc8341) [YangModels/Yang/ietf-netconf-acm.yang](https://github.com/YangModels/yang/blob/main/standard/ietf/RFC/ietf-netconf-acm%402018-02-14.yang) |
 | [ietf-sid-file](ietf-sid-file.yang)               | 2024-07-31 | 1300 | 50 | `N/A` | [ietf-sid-file.sid](auto/ietf-sid-file.sid)               | `N/A` | [RFC9595](https://datatracker.ietf.org/doc/html/rfc9595) [YangModels/Yang/ietf-sid-file.yang](https://github.com/YangModels/yang/blob/main/standard/ietf/RFC/ietf-sid-file%402024-07-31.yang) |
 | [ietf-interfaces](ietf-interfaces.yang)           | 2018-02-20 | 1500 | 100 | `N/A` | [ietf-interfaces.sid](auto/ietf-interfaces.sid)           | `N/A` | [RFC8343](https://datatracker.ietf.org/doc/html/rfc8343) [YangModels/Yang/ietf-inetfaces.yang](https://github.com/YangModels/yang/blob/main/standard/ietf/RFC/ietf-inetfaces%402018-02-20.yang) |
 | [ietf-ip](ietf-ip.yang)                           | 2018-02-22 | 1600 | 100 | `N/A` | [ietf-ip.sid](auto/ietf-ip.sid)                           | `N/A` | [RFC8344](https://datatracker.ietf.org/doc/html/rfc8344) [YangModels/Yang/ietf-ip.yang](https://github.com/YangModels/yang/blob/main/standard/ietf/RFC/ietf-ip%402018-02-22.yang) |
 | [ietf-system](ietf-system.yang)                   | 2014-08-06 | 1700 | 100 | `N/A` | [ietf-system.sid](auto/ietf-system.sid)                   | `N/A` | [RFC7317](https://datatracker.ietf.org/doc/html/rfc7317) [YangModels/Yang/ietf-system.yang](https://github.com/YangModels/yang/blob/main/standard/ietf/RFC/ietf-system%402014-08-06.yang) |
 | [iana-if-type](iana-if-type.yang)                 | 2014-05-08 | 1800 | 400 | `N/A` | [iana-if-type.sid](auto/iana-if-type.sid)                 | `N/A` | [RFC7224](https://datatracker.ietf.org/doc/html/rfc7224) [YangModels/Yang/iana-if-type.yang](https://github.com/YangModels/yang/blob/main/standard/ietf/RFC/iana-if-types%402014-05-08.yang) |
 | [ietf-voucher](ietf-voucher.yang)                 | 2018-05-09 | 2450 | 50 | `N/A` | [ietf-voucher.sid](auto/ietf-voucher.sid)                 | `N/A` | [draft-ietf-anima-rfc8366bis](https://datatracker.ietf.org/doc/draft-ietf-anima-rfc8366bis/) |
 | [ietf-voucher-request](ietf-voucher-request.yang) | 2021-05-20 | 2500 | 50 | `N/A` | [ietf-voucher-request.sid](auto/ietf-voucher-request.sid) | `N/A` | [draft-ietf-anima-rfc8366bis](https://datatracker.ietf.org/doc/draft-ietf-anima-rfc8366bis/) |
 | [ietf-schc](ietf-schc.yang)                       | 2023-03-01 | 2550 | 400 | `N/A` | [ietf-schc.sid](auto/ietf-schc.sid)                       | `N/A` | [RFC9363](https://datatracker.ietf.org/doc/html/rfc9363) [YangModels/Yang/ietf-schc.yang](https://github.com/YangModels/yang/blob/main/standard/ietf/RFC/ietf-schc%402023-03-01.yang) |

# Tooling
TODO
