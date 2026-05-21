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
 - auto
 - optimal
 - misc
 - `*.yang`

## Detailed description

[^auto]
Directory [auto](auto) has `Makefile` and generated .sid files for all tracked modules.
See the `Makefile` for how the .sid files are genereted.

[^optimal]
Directory [optimal](optimal) contains optimized .sid files after the analysis. If the .sid file is missing
there, it has not been (most likely) analyzed yet.

[^misc]
In the [misc](misc) directory, you can find modules not tracked by referenced IANA registry
but I think they should be part of the registry.

# Tracked modules
 - [iana-crypt-hash](ietf-crypt-hash.yang)           revision 2014-08-06
 - [iana-if-type](iana-if-type.yang)                 revision 2014-05-08
 - [ietf-coreconf](eitf-coreconf.yang)               revision 2026-03-02
 - [ietf-inet-types](ietf-inet-types.yang)           revision 2025-12-22
 - [ietf-interfaces](ietf-interfaces.yang)           revision 2018-02-20
 - [ietf-ip](ietf-ip.yang)                           revision 2018-02-22
 - [ietf-netconf-acm](ietf-netconf-acm.yang)         revision 2018-02-14
 - [ietf-schc](ietf-schc.yang)                       revision 2023-03-01
 - [ietf-sid-file](ietf-sid-file.yang)               revision 2024-07-31
 - [ietf-system](ietf-system.yang)                   revision 2014-08-06
 - [ietf-voucher-request](ietf-voucher-request.yang) revision 2021-05-20
 - [ietf-voucher](ietf-voucher.yang)                 revision 2018-05-09
 - [ietf-yang-types](ietf-yang-types.yang)           revision 2025-12-22

# Tooling
TODO
