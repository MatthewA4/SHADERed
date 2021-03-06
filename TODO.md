# PLAN
 1.2.*  -> polishing & fixing

 1.3    -> shader debugger

 1.3.*  -> improve debugger
 
# TODO
List of features I want to implement:
 - multiple cameras
   - this feature would allow you to render same scene from multiple angles
   - maybe add it as "Camera snapshot" and have a variable value function that takes in cam snapshot name
 - node shader editor that can export to GLSL and HLSL
 - shader & theme "store"
   - a place where you can upload your shaders or themes and see other peoples creations
 - "Export as DirectX/OpenGL application" option (.cpp file)
 - "import from ShaderToy" option
 - render your shader to a video file
 - pixel inspector
 - audio shaders
 - debugger

Except those features, I am also looking to do some small QoL changes and fixes:
 - file "Compile" option compiles shader pass twice (one with the Recompile and another time if the "Recompile on file change" is on)
 - rework variables (so that the type can be changed)
 - list all system variables
 - openning Sobel after Edge -> doesn't render anything
 - crashes when opening cubemap example only on Linux and only in Release mode!
 - prevent crashes (loading wrong 3d model, compute shaders not supported, etc...)
 - color compute shader labels light/dark green
 - bring all Preview tools to ObjectPreview window
 - CodeEditorUI loses focus when pressing ALT keys on linux
 - move 3D models to ObjectManager
 - show tips on startup & 'whats new' on first startup
 - create UI/Tools directory (for CubemapPreview, Magnifier, PixelInspect, etc...)
 - recompile the shader after we change shader path in a shader pass
 - when adding a shader pass, decompile the shader and detect input variables
 - when loading a texture it might not be loaded if not bound to any shader pass
 - ability to change warning, message and error text colors
 - lower down std::map and std::unordered_map usage
 - right click in code editor
 - why isn't first arg in CodeEditorUI::m_open a pointer?
 - PipelineUI::GetSelectedShaderPass() -> add Geometry and other options under "Create" menu item in GUIManager
 - ability to edit the buttons that show up in the toolbar
 - shift+drag with right click to move ArcBallCamera focus point
 - add an option to hide and/or lock certain shader pass
 - improve the overall code (enum for shader type, etc...)
 - fix memory leaks
 - undo/redo
 - languages (english, croatian, etc...)
 - switch from sdl to sfml (?)
 - dragging items from one pass to another, duplicating them, etc...