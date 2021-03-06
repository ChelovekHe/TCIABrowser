cmake_minimum_required(VERSION 2.8.9)

project(TCIABrowser)

#-----------------------------------------------------------------------------
set(EXTENSION_HOMEPAGE "http://www.slicer.org/slicerWiki/index.php?title=Documentation/Nightly/Extensions/TCIABrowser")
set(EXTENSION_CATEGORY "Informatics")
set(EXTENSION_CONTRIBUTORS "Alireza Mehrtash(SPL and BWH), Andrey Fedorov (SPL and BWH)")
set(EXTENSION_DESCRIPTION "A Module to connect to TCIA archive, browse the collections, patients and studies and download DICOM files to 3D Slicer.")
set(EXTENSION_ICONURL "http://wiki.slicer.org/slicerWiki/images/9/92/TCIABrowser_logo.png")
set(EXTENSION_SCREENSHOTURLS "http://www.slicer.org/slicerWiki/images/b/bf/TCIABrowser-screenshot.png")

#-----------------------------------------------------------------------------
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
add_subdirectory(TCIABrowser)

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_CPACK})
