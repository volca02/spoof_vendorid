# Spoof vendorid

This small vulkan layer will spoof vendorid to be of AMD rather than NVidia. It is a quick and dirty hack to enable No Man's Sky to work well on Nvidia Cards.
The repository is a direct copy of a part of Vulkan SDK by LunarG, with only the vendorid layer code added by me, all licensing and rights are as specified by LunarG.

To use this layer, after building it place a copy of the two built files (libVkLayer_vendorid_layer.so and VkLayer_vendorid_layer.json) to your chosen "/some/path", and edit the launch options of No Man's Sky in steam as follows, while replacing /some/path with your chosen path:

    VK_LAYER_PATH=/some/path/ VK_INSTANCE_LAYERS=VK_LAYER_LUNARG_vendorid_layer %COMMAND%

All credits go to ZeroFault, who discovered this fix. I was just too impatient to wait for him to post a working solution so I re-implemented what he described.

[![LunarG][1]][2]

[1]: https://vulkan.lunarg.com/img/LunarGLogo.png "www.LunarG.com"
[2]: https://www.LunarG.com/

Copyright &copy; 2015-2019 LunarG, Inc.

[![Creative Commons][3]][4]

[3]: https://i.creativecommons.org/l/by-nd/4.0/88x31.png "Creative Commons License"
[4]: https://creativecommons.org/licenses/by-nd/4.0/
