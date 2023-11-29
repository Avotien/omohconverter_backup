# omohconverter_backup
Tool to convert MOHAA's .bsp files to .fbx format.

=== Help ===

?
    - Shows help.

anim_delta
    - [SKC] Exports animation delta.

bsp_doublesided
    - [BSP] Exports faces as double-sided.

bsp_missingsurfaces
    - [BSP] Attempts to recreate missing surfaces (EXPERIMENTAL).

bsp_nosky
    - [BSP] Ignores sky.

bsp_no_connection
    - [BSP] Prevents brushes from being connected when they are touching and sharing at least one same shader.
      [BSP] Warning: Not recommended for performance.

bsp_uniquefaces
    - [BSP] Treats each faces as unique instead of merging faces by shaders.
      [BSP] Warning: This feature is expensive.

dontrecomputenormals
    - Prevent recomputing normals of each verts.

expansions
    - Includes assets from expansions (maintt and mainta game directories).

file( String file, [ String ref ] )
    - Adds a file to the export list.

gamepath( String gamedir )
    - Sets the game directory.

help
    - Shows help.

model_not_doublesided
    - [MODEL] Prevents models from being double-sided.

nomaterial
    - Disables the creation of materials.

outdir( String outdir )
    - Sets the output directory.

skipexistingtextures
    - Skips extraction of existing textures from maps/models on the disk.

skiptextures
    - Skips the extraction of textures from maps/models (useful if you already have extracted them).

tiki_export_anims
    - [TIKI] Exports all animations from the tiki file.

uniquematerial
    - Uses unique materials instead of merging duplicate materials (useful for models, not for levels).

Example Usage:

- Open cmd in the folder where omohconverter is installed
- Run it in the cmd e.g.:
  omohconverter_x64 -gamepath "E:/games/MOHAA" -outdir "E:/omohconverter/output" -file "maps/dm/mohdm6.bsp" -bsp_nosky -nomaterial
