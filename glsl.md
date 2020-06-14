# Notes

Thoughts on build a library to deal with shader management


## Separate Shader Objects is a must

## SPIR-V to distribute shader

glsl form
spir-v form

spir-v modules
may have many entry points for the same stage


portability 

reduce size

protection obfuscation

runtime compiler performance 
no parsing time


### Two steps

1. associate model with shader object
2. associate entry point with shader object
glShaderBinary
glSpecializeShader()
glAttachShader
glLinkProgram

### Offline Tools
SPIRV-Tools for validation

Glslang for generate SPIRV

### Changes to make in GLSL to generate valid SPIR-V
specialized constant

subroutine is not supported
depracated feature: textrue2D

glsl has to be use feature from the core profile 




### Design the library 

program ===> one stage

pipeline  ===> combine multiple program to a full-blown working pipeline

each shader object how to "CRUD" 

manage pipelines


different object may use different pipeline , 

uniform
uniform block for each program


### scenegraph travseral 

recent pipeline + uniform to the model/mesh

how to group the models to minimize the pipeline switch ? 


each frame scene update

can we optimize the scene graph here

each frame scene render

SoGroup and SoSeparator from open inventor 








