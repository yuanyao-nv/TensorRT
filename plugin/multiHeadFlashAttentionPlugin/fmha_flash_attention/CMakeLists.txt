#
# SPDX-FileCopyrightText: Copyright (c) 1993-2022 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
# SPDX-License-Identifier: Apache-2.0
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
# http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
#
file(GLOB SRCS src/*.cpp)
set(PLUGIN_SOURCES ${PLUGIN_SOURCES} ${SRCS})
set(PLUGIN_SOURCES ${PLUGIN_SOURCES} PARENT_SCOPE)
file(GLOB CU_SRCS src/*.cu)
set(STABLE_DIFFUSION_CU_SOURCES ${STABLE_DIFFUSION_CU_SOURCES} ${CU_SRCS})
set(STABLE_DIFFUSION_CU_SOURCES ${STABLE_DIFFUSION_CU_SOURCES} PARENT_SCOPE)
