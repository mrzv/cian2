add_executable              (coupling coupling.cpp mesh_gen.cpp)
target_link_libraries       (coupling ${libraries})

install(TARGETS coupling
        DESTINATION ${CMAKE_INSTALL_PREFIX}/coupling/
        PERMISSIONS OWNER_READ OWNER_WRITE OWNER_EXECUTE GROUP_READ GROUP_WRITE GROUP_EXECUTE WORLD_READ WORLD_WRITE WORLD_EXECUTE)

install(FILES COUPLING_TEST
        DESTINATION ${CMAKE_INSTALL_PREFIX}/coupling/
        PERMISSIONS OWNER_READ OWNER_WRITE OWNER_EXECUTE GROUP_READ GROUP_WRITE GROUP_EXECUTE WORLD_READ WORLD_WRITE WORLD_EXECUTE)
