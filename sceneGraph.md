remove traversal


remove driver


polygon split a huge small spieces


pakcing once for all data 

batch multiple draw to less call

minimize cpu/gpu interaction


// batch draw

1.4 glMultiDrawElemetns 

vertex format desc 

2.1  VBO
multiple buffer, 1 pos + normal
2. tex


gl4.3 VAO

Buffer separate with binding. 

glVertexAttribFormat
glVertexAttribBinding

glBindingVertexBuffer



Nv_vertex_buffer_unifiedmemory 

glEnableClientState

glBufferAddressRangeNV


Shader Parameter change frequency

Too many glUnifrom call bad ? 

// use uniform buffer (ubo)

glBindBufferBase
glNamedBufferSubDataEXT
glBufferSubData
glBindBufferRange   

shader side use uniformBloaCL



// case small portion of large buffer needs update frame by frame
SSBO (use shader to write into buffer ssbo)
compute shader

update transofrm tree 

level by level udpate 

TextureBufferObject

sampleBuffer pass in all the matrix array 


previous each matrial group fire a batch call 


now combine them one call ? 

MultiDrawIndirect

GL_DRAW_INDIRECT_BUFFER

gl_baseInstanceARB


nvidia nv_bindless_multidraw_indirect 
glMultiDrawElementsInddirectBindlessNV

on call per shader



API Related to textures

GL4.4 glBindTextures bind array of texture

nv_bindless_texture
arb_bindless_texture    

glGetTextureHandle
glMakeTextureHandleResident
glUniformHandleui64ARB

uint64 address for each texture

combine them into one buffer 
access it in fragment with right index for each object



Occulusion culling
Matrix buffer
boundingbox buffer 
object refrence matrix buffer

Single gpu culling 

bit stream back to cpu 

or GPU-gpu Indiretg




