# Makefile for compiling Xinamine

# Compiler options
SWIFTC = xcrun --sdk iphoneos swiftc
TARGET = -target arm64-apple-ios15

# Paths
SRC_DIR = Sources/Xinamine
ENTITLEMENTS = entitlements.plist
INSTALL_DIR = ../layout/var/jb/usr/local/bin
EXECUTABLE = $(INSTALL_DIR)/Xinamine

all: build

# Build rules
build:
	$(SWIFTC) $(TARGET) -o Xinamine -v \
	-Xlinker -sectcreate -Xlinker __TEXT -Xlinker __entitlements -Xlinker $(ENTITLEMENTS) \
	$(SRC_DIR)/Xinamine.swift
	mkdir -p $(INSTALL_DIR)
	cp Xinamine $(EXECUTABLE)

clean:
	rm -f Xinamine
	rm -f $(EXECUTABLE)
