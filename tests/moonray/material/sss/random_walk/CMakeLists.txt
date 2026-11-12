# Copyright 2025 DreamWorks Animation LLC
# SPDX-License-Identifier: Apache-2.0

# This tests random_walk Path Traced SSS.

if(IsDarwinPlatform) # macOS
    add_rats_test(
        INPUTS scene.rdla
        CANONICALS scene.exr
        DISABLED_XPU DISABLED_VECTOR # MOONRAY-6157
    )
else()
    add_rats_test(
        INPUTS scene.rdla
        CANONICALS scene.exr
    )
endif()
