# Copyright 2026 DreamWorks Animation LLC
# SPDX-License-Identifier: Apache-2.0

# Tests mip selection / texture filter scale using a texture with unique images per mip level.
# Based on the mip_selector test, but uses UsdUVTexture (and UVTransformMap) instead of ImageMap to exercise USD texture mip selection.

add_rats_test(
    INPUTS scene.rdla
    CANONICALS scene.exr
)
