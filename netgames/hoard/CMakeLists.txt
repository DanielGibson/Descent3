set(HEADERS hoardaux.h Hoard.h hoardstr.h)
set(CPPS hoard.cpp hoard_ui.cpp)

set (NETGAME_MODULE hoard)

add_library(${NETGAME_MODULE} SHARED ${CPPS} ${HEADERS})
set_target_properties(${NETGAME_MODULE} PROPERTIES PREFIX "")
set_target_properties(${NETGAME_MODULE} PROPERTIES SUFFIX ".d3m")

target_link_libraries(${NETGAME_MODULE} dmfc)
