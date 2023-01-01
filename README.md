# TexturePacker

Single file packing algorithm for packing a collection of textures (rectangles) into one single "Atlas" texture (container rectangle)

The input buffer has a stride of 3: [id | width | height] But It's capacity must accomodate for the output format:
The buffer is read then cleared to store the output rectancles of stride 5: [id | width | height | x position | y position],
Where the position is the (bottom left) position in the Atlas (container rectangle).

![packing](https://user-images.githubusercontent.com/66935412/210165211-074c0443-a27f-44de-9a5b-040a69767eb3.gif)
