cmake_minimum_required(VERSION 3.2)
project(imgui)

set(SOURCE_FILES 
	"imgui.cpp"
	"imgui_demo.cpp"
	"imgui_draw.cpp"
	"imgui_widgets.cpp"
)
set(HEADER_FILES 
	"imconfig.h"
	"imgui.h"
	"imgui_internal.h"
	"imstb_rectpack.h"
	"imstb_textedit.h"
	"imstb_truetype.h"
)

include_directories(${CMAKE_CURRENT_SOURCE_DIR})

add_library(imgui STATIC ${SOURCE_FILES} ${HEADER_FILES})