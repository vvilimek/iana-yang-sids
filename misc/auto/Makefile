.PHONY: ietf-datastores ietf-constrained-yang-library all

all: ietf-datastores ietf-constrained-yang-library

ietf-datastores:
	pyang --sid-generate-file 71000:100 -p ../.. -p .. ../ietf-datastores.yang

ietf-constrained-yang-library:
	pyang --sid-generate-file 70000:100 -p ../.. -p .. ../ietf-constrained-yang-library.yang
