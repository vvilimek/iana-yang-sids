# `vvilimek`'s proposals for the IANA YANG SIDs registry

This directory follow same structure as the [parent](https://github.com/vvilimek/iana-yang-sids).

# Structure
 - `readable/` human-readable .sid files

# YANG Modules
 - [ietf-constrained-yang-library](ietf-constrained-yang-library.yang) revision 2019-03-28
 - [ietf-datastores](ietf-datastores.yang) revision 2018-02-14

# Tracked modules
 | YANG Module                                       | revision   | Entry point | Size  | IANA .sid file | PYANG .sid file | optimized .sid file | source |
 | -----------                                       | --------   | ----------- | ----- | -------------- | --------------- | ------------------- | ------ |
 | [ietf-constrained-yang-library](ietf-constrained-yang-library.yang)  | 2019-03-28 | 70000 | 100 | `N/A` | [ietf-constrained-yang-library.sid](auto/ietf-constrained-yang-library.sid)   | [ietf-constrained-yang-library.sid](optimal/ietf-constrained-yang-library.sid) | [draft-ietf-constrained-yang-library](https://datatracker.ietf.org/doc/html/draft-ietf-core-yang-library/) |
 | [ietf-datastores](ietf-datastores.yang)               | 2018-02-14 | 71000 | 100 | `N/A` | [ietf-datastores.sid](auto/ietf-datastores.sid)   | Not needed, `identity` only module | [RFC8342](https://datatracker.ietf.org/doc/html/rfc8342) [YangModels/Yang/ietf-datastores.yang](https://github.com/YangModels/yang/blob/main/standard/ietf/RFC/ietf-datastores%402018-02-14.yang) |


