
# Rostkatze

An offspring of the gfx-rs project, implementing a C++ Vulkan driver on top of D3D12.
Currently, lacks a lot functionality but can run quite a few Vulkan samples already.

## Missing pieces

- Pipeline barriers
- RenderPasses
- Secondary command buffers
- Simultaneous command buffer submission
- Queries
- Validation of the current implementation(!)
- Resource Tier 1 support

... (100+ bullet points)

## Running

To able to use it latest Windows 10 Update is required (atm) and a GPU with Resource Tier 2 hardware (no NVIDIA!).

The library can be built with VS 2017 (C++17 support). In order to use the `rostkatze` ICD set the `VK_ICD_FILENAMES` variable to the path of `rostkatze_debug.json`.

Good luck!


## "Working" samples (SaschaWillems)

- triangle
- pipelines
- texture
- texturearray
- mesh
- specialization constants
- offscreen
- radialblur
- textoverlay
- particlefire (small particles only)
- scenerendering
- HDR
- shadowmappingcascade
- shadowmappingomni
- skeletalanimation
- bloom
- deferred
- pbrbasic
- pbribl
- pbrtexture
- computeshaderparticles
- computeshader
- sphericalenvmapping
- gears
- distancefieldrendering
- vulkanscene
- imgui

## Partially working

- shadowmapping (dynamic depth bias missing)
- computecloth (bugs)
- ssao (bugs)
- pushconstants (push constant array members)

# Almost/Not working

- texturecubmap (texture copy alignment)
- multithreading (seconday buffers not implemented)
- dynamic uniform buffers (not implemented)
- instancing (inverse, ?)
- indirect drawing (not implemented)
- occlusion queries (not implemented)
- mipmap gen (not implemented)
- multisampling (not implemented)
- deferred shadows (geometry shader support)
- n-body (bug either in spirv-cross or samples)
- raytracing (reading structs from byteaddressbuffer not supported)
- culllod (indirect drawing, ..)
- parallax (samples bug?)

- All tessellation and geometry samples
