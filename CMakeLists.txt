cmake_minimum_required(VERSION 3.5)
project(hasm)

set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} --std=gnu11")


set(SOURCE_FILES
        hasm.c
        parser.c parser.h
        hdr.c hdr.h
        optab.c optab.h
        symtab.c symtab.h
        lexer.c lexer.h
        utils.c utils.h
        )
add_executable(hasm ${SOURCE_FILES})
