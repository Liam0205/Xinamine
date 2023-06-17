# Theos optimisations

ARCHS = arm64 arm64e

# Processes die if they are killed

INSTALL_TARGET_PROCESSES = SpringBoard

# Define included files, imported frameworks, etc.

LIBRARY_NAME = Xinamine
$(LIBRARY_NAME)_FILES = Sources/load.s $(wildcard Sources/Xinamine/*.swift)

# Theos makefiles to include

include $(THEOS)/makefiles/common.mk
include $(THEOS_MAKE_PATH)/aggregate.mk
include $(THEOS_MAKE_PATH)/library.mk
