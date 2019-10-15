Bootstrap: docker
From: registry.gitlab.com/rode0day/fuzzer-testing/aflpp_runner:16.04 

%labels
    MAINTAINER Josh Bundt
    DockerTagID 1c774174d 

%environment
    AFL_SKIP_CPUFREQ=1
    LC_ALL=C
    LANG=C
    export AFL_SKIP_CPUFREQ LC_ALL LANG

%runscript
    exec /start_fuzzing "$@"

