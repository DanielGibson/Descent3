set(HEADERS )
set(CPPS
		Collide.cpp
		FindIntersection.cpp
		newstyle_fi.cpp
		physics.cpp)

add_library(physics STATIC ${HEADERS} ${CPPS})