cc_library(
    name = 'libevhtp',
    srcs = [
        'evhtp.c',
        'evthr.c',
        'htparse.c'
    ],
    deps = [
        '#pthread',
        '//thirdparty/libevent:libevent',
    ],
    defs = [
        'EVHTP_DISABLE_REGEX',
        'EVHTP_DISABLE_SSL',
    ],
    warning = 'no',
)

cc_binary(
    name = 'test_basic',
    srcs = 'examples/test_basic.c',
    deps = [
        ':libevhtp',
    ],
    incs = ['.'],
)
