# TexturePacker

Single file packing algorithm for packing a collection of textures (rectangles) into one single "Atlas" texture (container rectangle)

The input buffer has a stride of 3: [id | width | height] tightly packed. But It's capacity must accomodate the output format:
The inpuffer is read then cleared to store the output with stride 5: [id | width | height | x position | y position],
Where the position is the (bottom left) position in the Atlas (container rectangle).
