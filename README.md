# bedrock_floor
only some testing for bedrock_floor at y=0 1.17 like layer

# how to use
for vanilla, use "minecraft"  
for custom dimension, use "bedrock1"

i dont know how to delete data and pack.mcmeta from test2 from this rep btw .. so pls ignore those files


# how is it done
you also can generate your own code, for different vedrock_floor layer height with help of https://misode.github.io/  
just add +64, +48, +23 or +16 to all Y-Values (bedrock_floor layer result: 0, -16, -32, -48)

change Y values in following worldgen:  
Dimension Generator
https://misode.github.io/dimension/?share=FMn8lZnMh3  
Dimension Type Generator
https://misode.github.io/dimension-type/?version=1.19&preset=overworld  
Noise Settings Generator
https://misode.github.io/worldgen/noise-settings/?share=dhQytbRk4P  
Density Function Generator
https://misode.github.io/worldgen/density-function/?version=1.19&preset=overworld%2Fcaves%2Fnoodle  

### IF YOU WANT TO USE IT FOR CUSTOM DIMENSION
dont forget to change the worldgen references betweetn worldgen code files .. 
so for example if your datapack namespace is "custom" and you named your density_function "noodle.json" you have to change "minecraft:overworld/caves/noodle" to "custom:noodle" in your Noise Settings Generator Code.



