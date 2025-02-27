# SPDX-License-Identifier: GPL-3.0-only
# MuseScore-CLA-applies
#
# MuseScore
# Music Composition & Notation
#
# Copyright (C) 2021 MuseScore BVBA and others
#
# This program is free software: you can redistribute it and/or modify
# it under the terms of the GNU General Public License version 3 as
# published by the Free Software Foundation.
#
# This program is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Public License for more details.
#
# You should have received a copy of the GNU General Public License
# along with this program.  If not, see <https://www.gnu.org/licenses/>.

set(MODULE audio)

set(MODULE_QRC audio.qrc)

set(MODULE_QML_IMPORT ${CMAKE_CURRENT_LIST_DIR}/qml)

set(MODULE_SRC
    ${CMAKE_CURRENT_LIST_DIR}/audiostubmodule.cpp
    ${CMAKE_CURRENT_LIST_DIR}/audiostubmodule.h
    ${CMAKE_CURRENT_LIST_DIR}/audioconfigurationstub.cpp
    ${CMAKE_CURRENT_LIST_DIR}/audioconfigurationstub.h
    ${CMAKE_CURRENT_LIST_DIR}/synthresolverstub.cpp
    ${CMAKE_CURRENT_LIST_DIR}/synthresolverstub.h
    ${CMAKE_CURRENT_LIST_DIR}/fxresolverstub.cpp
    ${CMAKE_CURRENT_LIST_DIR}/fxresolverstub.h
    ${CMAKE_CURRENT_LIST_DIR}/soundfontrepositorystub.cpp
    ${CMAKE_CURRENT_LIST_DIR}/soundfontrepositorystub.h
    ${CMAKE_CURRENT_LIST_DIR}/audiodriverstub.cpp
    ${CMAKE_CURRENT_LIST_DIR}/audiodriverstub.h
    )                           

include(${PROJECT_SOURCE_DIR}/build/module.cmake)
