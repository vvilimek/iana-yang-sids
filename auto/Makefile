.PHONY: iana-crypt-hash iana-if-type ietf-coreconf ietf-inet-types ietf-interfaces \
	ietf-ip ietf-netconf-acm ietf-schc ietf-sid-file ietf-system \
	ietf-voucher-request ietf-voucher ietf-yang-types \
	all clean

all: iana-crypt-hash iana-if-type ietf-coreconf ietf-inet-types ietf-interfaces \
	ietf-ip ietf-netconf-acm ietf-schc ietf-sid-file ietf-system \
	ietf-voucher-request ietf-voucher ietf-yang-types

iana-crypt-hash:
	pyang --sid-generate-file 1200:50 -p .. ../iana-crypt-hash.yang
	mv -f iana-crypt-hash*.sid iana-crypt-hash.sid

iana-if-type:
	pyang --sid-generate-file 1800:400 -p .. ../iana-if-type.yang
	mv -f iana-if-type*.sid iana-if-type.sid

ietf-coreconf:
	pyang --sid-generate-file 1000:100 -p .. ../ietf-coreconf.yang
	mv -f ietf-coreconf*.sid ietf-coreconf.sid

ietf-inet-types:
	pyang --sid-generate-file 1150:40 -p .. ../ietf-inet-types.yang
	mv -f ietf-inet-types*.sid ietf-inet-types.sid

ietf-interfaces:
	pyang --sid-generate-file 1500:100 -p .. ../ietf-interfaces.yang
	mv -f ietf-interfaces*.sid ietf-interfaces.sid

ietf-ip:
	pyang --sid-generate-file 1600:100 -p .. ../ietf-ip.yang
	mv -f ietf-ip*.sid ietf-ip.sid

ietf-netconf-acm:
	pyang --sid-generate-file 1250:50 -p .. ../ietf-netconf-acm.yang
	mv -f ietf-netconf-acm*.sid ietf-netconf-acm.sid

ietf-schc:
	pyang --sid-generate-file 2550:400 -p .. ../ietf-schc.yang
	mv -f ietf-schc*.sid ietf-schc.sid

ietf-sid-file:
	pyang --sid-generate-file 1300:50 -p .. ../ietf-sid-file.yang
	mv -f ietf-sid-file*.sid ietf-sid-file.sid

ietf-system:
	pyang --sid-generate-file 1700:100 -p .. ../ietf-system.yang
	mv -f ietf-system*.sid ietf-system.sid

ietf-voucher:
	pyang --sid-generate-file 2450:50 -p .. ../ietf-voucher.yang
	mv -f ietf-voucher@*.sid ietf-voucher.sid
	
ietf-voucher-request:
	pyang --sid-generate-file 2500:50 -p .. ../ietf-voucher-request.yang
	mv -f ietf-voucher-request@*.sid ietf-voucher-request.sid

ietf-yang-types:
	pyang --sid-generate-file 1100:50 -p .. ../ietf-yang-types.yang
	mv -f ietf-yang-types*.sid ietf-yang-types.sid

clean:
	rm -f *sid
