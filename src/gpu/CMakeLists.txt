add_executable(add-gpu)

target_sources(add-gpu PRIVATE add.cu)

set_target_properties(add-gpu   PROPERTIES
                                POSITION_INDEPENDENT_CODE ON
                                CUDA_SEPARABLE_COMPILATION ON
)
                                   
add_executable(add-block-gpu)

target_sources(add-block-gpu PRIVATE add_block.cu)

set_target_properties(add-block-gpu PROPERTIES 
                                    POSITION_INDEPENDENT_CODE ON
                                    CUDA_SEPARABLE_COMPILATION ON
)

add_executable(add-grid-gpu)

target_sources(add-grid-gpu PRIVATE add_grid.cu)

set_target_properties(add-grid-gpu  PROPERTIES 
                                    POSITION_INDEPENDENT_CODE ON
                                    CUDA_SEPARABLE_COMPILATION ON
)
