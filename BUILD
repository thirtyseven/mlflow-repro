load("@rules_python//python:pip.bzl", "compile_pip_requirements")

compile_pip_requirements(
    name = "requirements",
    requirements_in = "requirements.in",
    requirements_txt = "requirements_lock.txt",
)

py_test(
    name = "test",
    srcs = ["test.py"],
    legacy_create_init = False,
    deps = ["@pypi//mlflow"],
)
