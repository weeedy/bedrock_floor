# bedrock_floor
just some testing for custom bedrock_floor layer height  
at y=0 for example, to get it 1.17 like

# how to use
for vanilla, use "minecraft"  
for custom dimension, use "bedrock1"

# how it is done
you can also generate your own code, for different bedrock_floor layer height with help of https://misode.github.io/  
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

#### IF YOU WANT TO USE IT FOR CUSTOM DIMENSION
dont forget to change the worldgen references between worldgen code files .. 
so for example if your datapack namespace is "custom" and you named your density_function "noodle.json" you have to change "minecraft:overworld/caves/noodle" to "custom:noodle" in your Noise Settings Generator Code.

#### WHICH Y VALUES SHOULD I CHANGE?
especially if Y default value is -64 or -60 .. we are in testing phase, maybe you also should change -40, all negative, or all Y values
