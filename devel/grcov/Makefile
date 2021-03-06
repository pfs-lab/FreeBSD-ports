# $FreeBSD$

PORTNAME=	grcov
DISTVERSIONPREFIX=	v
DISTVERSION=	0.6.1
CATEGORIES=	devel

MAINTAINER=	yuri@FreeBSD.org
COMMENT=	Code coverage information aggregator

LICENSE=	MPL20
LICENSE_FILE=	${WRKSRC}/LICENSE-MPL-2.0

USES=		cargo

USE_GITHUB=	yes
GH_ACCOUNT=	mozilla

CARGO_CRATES=	\
		addr2line-0.14.0 \
		adler-0.2.3 \
		adler32-1.2.0 \
		aho-corasick-0.7.15 \
		ansi_term-0.11.0 \
		anyhow-1.0.34 \
		arrayref-0.3.6 \
		arrayvec-0.5.2 \
		atty-0.2.14 \
		autocfg-1.0.1 \
		backtrace-0.3.55 \
		base64-0.12.3 \
		bitflags-1.2.1 \
		blake2b_simd-0.5.11 \
		block-buffer-0.9.0 \
		bstr-0.2.14 \
		byteorder-1.3.4 \
		cargo-binutils-0.3.3 \
		cargo_metadata-0.11.4 \
		cc-1.0.65 \
		cfg-if-0.1.10 \
		cfg-if-1.0.0 \
		chrono-0.4.19 \
		clap-2.33.3 \
		const_fn-0.4.3 \
		constant_time_eq-0.1.5 \
		crc32fast-1.2.1 \
		crossbeam-0.8.0 \
		crossbeam-channel-0.5.0 \
		crossbeam-deque-0.8.0 \
		crossbeam-epoch-0.9.0 \
		crossbeam-queue-0.3.0 \
		crossbeam-utils-0.7.2 \
		crossbeam-utils-0.8.0 \
		digest-0.9.0 \
		dirs-2.0.2 \
		dirs-sys-0.3.5 \
		either-1.6.1 \
		failure-0.1.8 \
		failure_derive-0.1.8 \
		flate2-1.0.14 \
		fnv-1.0.7 \
		fomat-macros-0.3.1 \
		generic-array-0.14.4 \
		getrandom-0.1.15 \
		gimli-0.23.0 \
		globset-0.4.6 \
		hermit-abi-0.1.17 \
		is_executable-0.1.2 \
		itoa-0.4.6 \
		lazy_static-1.4.0 \
		libc-0.2.80 \
		libz-sys-1.1.2 \
		log-0.4.11 \
		md-5-0.9.1 \
		memchr-2.3.4 \
		memoffset-0.5.6 \
		miniz_oxide-0.3.7 \
		miniz_oxide-0.4.3 \
		num-integer-0.1.44 \
		num-traits-0.2.14 \
		num_cpus-1.13.0 \
		object-0.22.0 \
		opaque-debug-0.3.0 \
		pest-2.1.3 \
		pkg-config-0.3.19 \
		ppv-lite86-0.2.10 \
		proc-macro2-1.0.24 \
		quick-xml-0.20.0 \
		quote-1.0.7 \
		rand-0.7.3 \
		rand_chacha-0.2.2 \
		rand_core-0.5.1 \
		rand_hc-0.2.0 \
		rayon-1.5.0 \
		rayon-core-1.9.0 \
		redox_syscall-0.1.57 \
		redox_users-0.3.5 \
		regex-1.4.2 \
		regex-syntax-0.6.21 \
		remove_dir_all-0.5.3 \
		rust-argon2-0.8.2 \
		rustc-cfg-0.4.0 \
		rustc-demangle-0.1.18 \
		rustc-hash-1.1.0 \
		rustc_version-0.2.3 \
		ryu-1.0.5 \
		same-file-1.0.6 \
		scopeguard-1.1.0 \
		semver-0.9.0 \
		semver-0.10.0 \
		semver-0.11.0 \
		semver-parser-0.7.0 \
		semver-parser-0.10.1 \
		serde-1.0.117 \
		serde_derive-1.0.117 \
		serde_json-1.0.59 \
		simplelog-0.7.6 \
		smallvec-1.5.0 \
		strsim-0.8.0 \
		syn-1.0.50 \
		synstructure-0.12.4 \
		tcmalloc-0.3.0 \
		tempfile-3.1.0 \
		term-0.6.1 \
		textwrap-0.11.0 \
		thiserror-1.0.22 \
		thiserror-impl-1.0.22 \
		thread_local-1.0.1 \
		time-0.1.44 \
		toml-0.5.7 \
		typenum-1.12.0 \
		ucd-trie-0.1.3 \
		unicode-width-0.1.8 \
		unicode-xid-0.2.1 \
		uuid-0.8.1 \
		vcpkg-0.2.10 \
		vec_map-0.8.2 \
		version_check-0.9.2 \
		walkdir-2.3.1 \
		wasi-0.9.0+wasi-snapshot-preview1 \
		wasi-0.10.0+wasi-snapshot-preview1 \
		winapi-0.3.9 \
		winapi-i686-pc-windows-gnu-0.4.0 \
		winapi-util-0.1.5 \
		winapi-x86_64-pc-windows-gnu-0.4.0 \
		zip-0.5.8

PLIST_FILES=	bin/grcov

post-install:
	${STRIP_CMD} ${STAGEDIR}${PREFIX}/bin/${PORTNAME}

.include <bsd.port.mk>
