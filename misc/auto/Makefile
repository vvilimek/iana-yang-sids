.PHONY: ietf-datastores ietf-constrained-yang-library \
	all clean

all: ietf-datastores ietf-constrained-yang-library

REV_PATTERN=@[0-9][0-9][0-9][0-9]-[0-9][0-9]-[0-9][0-9]

ietf-datastores:
	pyang --sid-generate-file 71000:100 -p ../.. -p .. ../ietf-datastores.yang
	mv ietf-datastores${REV_PATTERN}.sid ietf-datastores.sid

ietf-constrained-yang-library:
	pyang --sid-generate-file 70000:100 -p ../.. -p .. ../ietf-constrained-yang-library.yang
	mv ietf-constrained-yang-library${REV_PATTERN}.sid ietf-constrained-yang-library.sid

clean:
	rm -f *.sid
