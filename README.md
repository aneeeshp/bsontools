These are simple utilities for manipulation of bson documents.

bcount   - count # of bson documents in a bson file
fromjson - convert JSON to BSON
hex      - hex dump of any input, with a tiny bit of bson format awareness.  
           also provided as a convenience for any OS where 'hexdump' is not already present.

Note: many of these utilities expect input from stdin, to facilitate piping.  Use -h to 
      get help.

## Building

You will need the bson-cxx library (a dependancy) to build the tools.  It is available in github. 
Place it as a peer level directory on disk with bsontools.  (That is you will see 
include "../../../bson-cxx/" in the source code of these tools...)

As written these tools lightly use C++11.  This is mainly to avoid any external dependencies; for 
example unique_ptr is used from C++11.  It would not be hard to adapt back to C++03.

With Visual Studio, start by opening build/fromjson/fronjson/sln.

