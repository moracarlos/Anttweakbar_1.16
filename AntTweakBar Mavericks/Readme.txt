This version allows you to compile Anttweakbar 1.16 in MacOS 10.10 Yosemite

2 Fixed errors:

1. Fixed:

In file included from TwOpenGLCore.cpp:22:
./LoadOGLCore.h:149:24: error: conflicting types for 'glMultiDrawElements'
ANT_GL_CORE_DECL(void, glMultiDrawElements, (GLenum mode, const GLsizei ...
                       ^
./LoadOGLCore.h:34:36: note: expanded from macro 'ANT_GL_CORE_DECL'
        extern "C" { _Ret APIENTRY _Fct _Params; }
                                   ^
/Applications/Xcode.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX10.10.sdk/System/Library/Frameworks/OpenGL.framework/Headers/gl.h:2836:13: note: 
      previous declaration is here
extern void glMultiDrawElements (GLenum mode, const GLsizei *count, GLen...
            ^
In file included from TwOpenGLCore.cpp:22:
./LoadOGLCore.h:214:24: error: conflicting types for 'glShaderSource'
ANT_GL_CORE_DECL(void, glShaderSource, (GLuint shader, GLsizei count, co...
                       ^
./LoadOGLCore.h:34:36: note: expanded from macro 'ANT_GL_CORE_DECL'
        extern "C" { _Ret APIENTRY _Fct _Params; }
                                   ^
/Applications/Xcode.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX10.10.sdk/System/Library/Frameworks/OpenGL.framework/Headers/gl.h:2923:13: note: 
      previous declaration is here
extern void glShaderSource (GLuint shader, GLsizei count, const GLchar* ...
            ^
2 errors generated.
make: *** [TwOpenGLCore.o] Error 1

2. Fixed: AntTweakBar: OpenGL Core Profile functions cannot be loaded.


AntTweakBar development library
-------------------------------


AntTweakBar is a small and easy-to-use C/C++ library that allows programmers
to quickly add a light and intuitive GUI into OpenGL and DirectX based 
graphic programs to interactively tweak parameters.

This package includes the development version of the AntTweakBar library 
for Windows, GNU/Linux and OSX, and some program examples (sources + binaries).

For installation and documentation please refer to:
http://anttweakbar.sourceforge.net/doc


