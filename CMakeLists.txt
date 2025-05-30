cmake_minimum_required(VERSION 3.20)

function(adafruit_sdfat_add TARGET)
  target_sources(${TARGET} PUBLIC
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/FreeStack.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/MinimumSerial.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/common/FmtNumber.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/common/FsCache.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/common/FsDateTime.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/common/FsName.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/common/FsStructs.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/common/FsUtf.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/common/PrintBasic.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/common/upcase.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/common
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/ExFatLib/ExFatDbg.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/ExFatLib/ExFatFile.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/ExFatLib/ExFatFilePrint.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/ExFatLib/ExFatFileWrite.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/ExFatLib/ExFatFormatter.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/ExFatLib/ExFatName.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/ExFatLib/ExFatPartition.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/ExFatLib/ExFatVolume.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/FatLib/FatDbg.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/FatLib/FatFile.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/FatLib/FatFileLFN.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/FatLib/FatFilePrint.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/FatLib/FatFileSFN.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/FatLib/FatFormatter.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/FatLib/FatName.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/FatLib/FatPartition.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/FatLib/FatVolume.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/FsLib/FsFile.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/FsLib/FsNew.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/FsLib/FsVolume.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/iostream/istream.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/iostream/ostream.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/iostream/StdioStream.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/iostream/StreamBaseClass.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/SdCard/Rp2040Sdio/PioSdioCard.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/SdCard/SdCardInfo.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/SdCard/SdSpiCard.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/SdCard/TeensySdio/TeensySdio.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/SpiDriver/SdSpiArtemis.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/SpiDriver/SdSpiChipSelect.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/SpiDriver/SdSpiDue.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/SpiDriver/SdSpiParticle.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/SpiDriver/SdSpiSTM32.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/SpiDriver/SdSpiSTM32Core.cpp
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src/SpiDriver/SdSpiTeensy3.cpp
    )
  target_include_directories(${TARGET} PUBLIC
    ${CMAKE_CURRENT_FUNCTION_LIST_DIR}/src
    )
endfunction()
