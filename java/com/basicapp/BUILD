load("@rules_android//android:rules.bzl", "android_binary", "android_library")
load("@rules_kotlin//kotlin:android.bzl", "kt_android_library")

android_binary(
    name = "basic_app",
    manifest = "AndroidManifest.xml",
    deps = [":basic_lib", ":basic_lib_kt"],
)

android_library(
    name = "basic_lib",
    srcs = ["BasicActivity.java"],
    manifest = "AndroidManifest.xml",
    resource_files = glob(["res/**"]),
)

kt_android_library(
    name = "basic_lib_kt",
    srcs = glob(["*.kt"]),
)