lib_LTLIBRARIES     = libfko.la

libfko_source_files = \
    base64.c base64.h cipher_funcs.c cipher_funcs.h digest.c digest.h \
    fko_client_timeout.c fko_common.h fko_digest.c fko_encode.c \
    fko_decode.c fko_encryption.c fko_error.c fko_funcs.c fko_message.c \
    fko_message.h fko_nat_access.c fko_rand_value.c fko_server_auth.c \
    fko.h fko_limits.h fko_timestamp.c fko_hmac.c hmac.c hmac.h \
    fko_user.c fko_user.h md5.c md5.h rijndael.c rijndael.h sha1.c \
    sha1.h sha2.c sha2.h fko_context.h fko_state.h fko_context.h \
    gpgme_funcs.c gpgme_funcs.h strlcpy.c strlcat.c fko_util.c fko_util.h

libfko_la_SOURCES   		= $(libfko_source_files)
libfko_la_LDFLAGS   		= -version-info 1:0:0 $(GPGME_LIBS) -export-symbols-regex '^fko_'

AM_CPPFLAGS         		= $(GPGME_CFLAGS) -I $(top_srcdir)/common

include_HEADERS     		= fko.h
