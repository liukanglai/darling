project(CoreMIDI)

set(DYLIB_COMPAT_VERSION "1.0.0")
set(DYLIB_CURRENT_VERSION "69.0.0")

add_framework(CoreMIDI
    FAT
    CURRENT_VERSION
    VERSION "A"

    SOURCES
        src/CoreMIDI.m
        src/MIDICIProfile.m
        src/MIDICIProfileState.m
        src/MIDICISession.m
        src/BLEMIDIAccessor.m
        src/MIDINetworkSession.m
        src/MIDINetworkHost.m
        src/MIDINetworkConnection.m

    DEPENDENCIES
        system
        objc
        Foundation
)
