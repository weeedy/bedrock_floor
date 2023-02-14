# bedrock_floor
just some minecraft 1.19 datapack testing for custom bedrock_floor layer height  
at y=0 for example, to get it 1.17 like

# how to use
for vanilla, use "minecraft"  
for custom dimension, use "custom"

# how it is done
you can also generate your own code, for different bedrock_floor layer height with help of https://misode.github.io/ thanks@https://github.com/misode  
just add +64, +48, +23 or +16 to all Y-Values (bedrock_floor layer result: 0, -16, -32, -48)

change Y values in following worldgen:  
Dimension Generator  
https://misode.github.io/dimension/?share=FMn8lZnMh3  
Dimension Type Generator  
https://misode.github.io/dimension-type/?version=1.19&preset=overworld  
Noise Settings Generator  
https://misode.github.io/worldgen/noise-settings/?share=dhQytbRk4P thanks@https://github.com/BluePsychoRanger  
Density Function Generator  
https://misode.github.io/worldgen/density-function/?version=1.19&preset=overworld%2Fcaves%2Fnoodle  

# Q&A
#### HOW TO USE IT FOR CUSTOM DIMENSION?
dont forget to change the worldgen references between worldgen code files .. 
so for example if your datapack namespace is "custom" and you named your density_function "noodle.json" you have to change "minecraft:overworld/caves/noodle" to "custom:noodle" in your Noise Settings Generator Code.

#### WHICH Y VALUES SHOULD I CHANGE?
especially if Y default value is -64 or -60 .. we are in testing phase, maybe you also should change -40, all negative, or all Y values

#### WHAT ABOUT WORLDBLENDING?
If you want to use Minecraft Worldblending feature, this will generate holes in bedrock floor layer. Here is a small manually "workaround" datapack:
execute as PAYERNAME at @s if entity PLAYERNAME[dimension=minecraft:overworld] run fill ~-16 0 ~-16 ~15 1 ~15 bedrock
Replace PAYERNAME with you name and minecraft:overworld with dimension you want to use it. Then fly along the worldborder, to fill the holes between old and new chunks, where worldblending does its job. The Datapack generates 2x16x16 area .. you can change it by adjusting -16 and 15 values

## what is planned?
it would be nice to create a datapack, where you can set a variable (e.g. "floor") in a config file, which indicates your wanted bedrock_floor layer height ..
as a result, it would generate a second variable (e.g. "add"), which will add the needed value to the Y-Values in existing worldgen code.  
another question would be, if it makes more sense to add some "relative" values to Y .. and not "absolute" values

i think that way it would be possible to get 4 scenarios, user could change:  
"floor"=	0		    "add"=	64  
"floor"=	-16		"add"=	48  
"floor"=	-32		"add"=	32  
"floor"=	-48		"add"=	16  

#### for more info, join conversation on MinecraftCommands discord https://discord.gg/QAFXFtZ here https://discord.com/channels/154777837382008833/1070953594288881724   or Misode's github rep https://github.com/misode/misode.github.io/discussions/208#discussioncomment-4897621
