# PROJECT(Gnuplot)

USING(PNG ZLIB)

ADD_DEFINITIONS()

SET(HEADERS
  Gnuplot.h
)

SET(SOURCES
  Gnuplot.cpp
)

SET(EXTRASOURCES
  Gnuplot.h
)

ADD_COVISE_MODULE(Tools  Gnuplot ${EXTRASOURCES} )
TARGET_LINK_LIBRARIES(Gnuplot  coApi coAppl coCore ${EXTRA_LIBS})
COVISE_INSTALL_TARGET(Gnuplot)
