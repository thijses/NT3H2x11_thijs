please put the NT3H1x01 library in a folder named 'lib' inside the platformIO example:

here is the contents of the README file that comes with the lib folder

This directory is intended for project specific (private) libraries.
PlatformIO will compile them to static libraries and link into executable file.

The source code of each library should be placed in a an own separate directory
("lib/your_library_name/[here are source files]").

For example, see a structure of the following two libraries `Foo` and `Bar`:

|--lib
|  |
|  |--Bar
|  |  |--docs
|  |  |--examples
|  |  |--src
|  |     |- Bar.c
|  |     |- Bar.h
|  |  |- library.json (optional, custom build options, etc) https://docs.platformio.org/page/librarymanager/config.html
|  |
|  |--Foo
|  |  |- Foo.c
|  |  |- Foo.h
|  |
|  |- README --> THIS FILE
|
|- platformio.ini
|--src
   |- main.c

and a contents of `src/main.c`:
```
#include <Foo.h>
#include <Bar.h>

int main (void)
{
  ...
}

```

PlatformIO Library Dependency Finder will find automatically dependent
libraries scanning project source files.

More information about PlatformIO Library Dependency Finder
- https://docs.platformio.org/page/librarymanager/ldf.html
