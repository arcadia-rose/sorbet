cc_import(
    name = "ssl-import",
    shared_library = "lib/x86_64-linux-gnu/libssl.so",
    visibility = ["//visibility:private"],
)

# No headers are exported, as /usr/include is already part of the system include path.
cc_library(
    name = "ssl",
    visibility = ["//visibility:public"],
    deps = [":ssl-import"],
)

cc_import(
    name = "crypto-import",
    shared_library = "lib/x86_64-linux-gnu/libcrypto.so",
    visibility = ["//visibility:private"],
)

# No headers are exported, as /usr/include is already part of the system include path.
cc_library(
    name = "crypto",
    visibility = ["//visibility:public"],
    deps = [":crypto-import"],
)
