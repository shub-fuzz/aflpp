Bootstrap: docker
From: registry.gitlab.com/rode0day/fuzzer-testing/aflpp_runner:16.04 

%labels
    MAINTAINER Josh Bundt
    DockerTagID bd8069b99

%environment
    AFL_SKIP_CPUFREQ=1
    LC_ALL=en_US.UTF-8
    LANG=en_US.UTF-8
    export AFL_SKIP_CPUFREQ LC_ALL LANG

%runscript
    exec /start_fuzzing "$@"

%post
    # In order to get locales working properly:
    export LANGUAGE=en_US.UTF-8 && \
    export LANG=en_US.UTF-8 && \
    export LC_ALL=en_US.UTF-8 && \
    locale-gen en_US.UTF-8 && \
    dpkg-reconfigure locales
