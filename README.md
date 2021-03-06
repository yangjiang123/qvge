## Qt Visual Graph Editor 
[![Github All Releases](https://img.shields.io/github/downloads/ArsMasiuk/qvge/total.svg?style=for-the-badge)](https://github.com/ArsMasiuk/qvge/releases/latest)
![GitHub release](https://img.shields.io/github/release/ArsMasiuk/qvge.svg?style=for-the-badge)
[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=Z35EHHJ3729GG&source=url)


**qvge** is a multiplatform graph editor written in C++/Qt. Its main goal is to make possible visually edit two-dimensional graphs
in a simple and intuitive way.

Please note that **qvge** is not a replacement for such a software like Gephi, Graphvis, Dot, yEd, Dia and so on. It is neither a tool for "big data analysis" nor a math application. It is really just a simple graph editor :)

![Screenshot1](https://user-images.githubusercontent.com/19762856/85934275-2a985480-b8e1-11ea-81a9-a5b81f3365e2.PNG)

### Main Features

- Easy creation and parameterising of small-sized till middle-sized graphs
- Hierarchical attribute model for nodes and edges
- Dynamically maintained list of commutations between nodes
- Directed, undirected and mixed graphs supported
- Node ports supported as well
- Search among the graph elements and their attributes
- Auto-creation and auto-layout of graphs (via [OGDF](https://ogdf.uos.de/))
- Export into PDF and popular image formats
- Graph file format support:
  - Native graph persistence format (XGR)
  - GEXF
  - GraphML
  - GML
  - [GraphViz DOT](https://graphviz.org/) (partially)
 
### Some users' feedback

>"Qt Visual Graph Editor is a fairly straightforward, open-source tool that enables users to design relatively simple graphs for their >projects. It comes with a decent set of features and is very intuitive." 

>"It seems to me that my development have become more efficient after when I began using QVGE. This is much more useful than UML, because that I don't have to change sheets and to remember several usages and I can draw graphs swiftly."

>"Lightweight, multi-platform graph editor that allows users to edit two-dimensional graphs in a quick and intuitive way, as an alternative to more complex software."

> "It's user experience is very good. It's because how to operate is sophisticated so intuitive and very simple. Because of that, it's easy to begin using. A user can entirely concentrate to essence of content the whole time. Because of simpleness, the content is not noisy and easy to understand, and usable much generally to design, refactor and output a structure such as a organization, a software, logic, routes and all other relationships without learning usage separately."

### Installation

Prebuild Windows binaries can be loaded from here:

[![Github All Releases](https://img.shields.io/github/downloads/ArsMasiuk/qvge/total.svg?style=for-the-badge)](https://github.com/ArsMasiuk/qvge/releases/latest)

Or you can get qvge's sources and build them by yourself. In this case you need to have installed Qt 5.x toolkit and corresponding C++ compiler with C++11 support. qvge uses native Qt build system (main project file is qvgeapp.pro) so it should look like:

~~~~
cd <directory-with-qvgeapp.pro>
qmake -r
~~~~

Linux GCC:
~~~~          
make 
~~~~

or Windows MinGW:
~~~~
mingw32-make 
~~~~

or Windows MSVC:
~~~~
nmake 
~~~~

or by Jom:
~~~~
jom 
~~~~

### Enabling OGDF 

In order to build **qvge** with OGDF support (shipped with qvge together): 
before running qmake, open src/config.ini file and make sure that the following option is present:
~~~~
CONFIG += USE_OGDF 
~~~~

Then run qmake + make as desribed in the step before. *Please note:* OGDF is really big, so its compilation takes some time. 


### Supported compilers

Recent version of **qvge** has been built with:
- Microsoft Visual Studio 2017 (Community Edition)
- MinGW 7.3
- GCC 7.5 (Linux)
- GCC 6.4.0 (Cygwin) 
- Clang C++ (FreeBSD)

Hopefully it can also be compiled with others compilers. If not please do not hesitate to provide description of the issue.

### Supported OS

**qvge** has been tested on Microsoft Windows 10 and several Linux OS (Mint, Mageia etc). Theoretically it should run on (almost) any OS which have Qt 5.x installed.

**qvge** can be compiled & run under Cygwin.

### Supported Qt

**qvge** has been tested with Qt 5.9-5.14. But it should work with any newer 5.x version too. 

### Credits

**qvge** uses following 3rd party components:

- [Qt](https://www.qt.io)
- [Qt property browser](https://github.com/qtproject/qt-solutions)
- [QProcessInfo](https://github.com/baldurk/qprocessinfo) 
- [QSint widgets library](https://sourceforge.net/projects/qsint) 
- [OGDF - Open Graph Drawing Framework](http://www.ogdf.net)
- SVG icons from [Inkscape](https://inkscape.org)

Special thanks to:

- Dr. prof. [Vladimir A. Svjatnyj](https://wiki.donntu.edu.ua/view/%D0%A1%D0%B2%D1%8F%D1%82%D0%BD%D0%B8%D0%B9_%D0%92%D0%BE%D0%BB%D0%BE%D0%B4%D0%B8%D0%BC%D0%B8%D1%80_%D0%90%D0%BD%D0%B4%D1%80%D1%96%D0%B9%D0%BE%D0%B2%D0%B8%D1%87), head of [computer engineering chair](https://donntu.edu.ua/knt/kafedra-ki) at [DonNTU](https://donntu.edu.ua/en/donntu2020) and my scientific supervisor
- [Tatsuro Ueda](https://github.com/weed), founder of [Feel Physics](https://feel-physics.jp), for comrehensive testing, feedback and suggestions 

### Extenal Links

**qvge** at [![Download qvge](https://sourceforge.net/sflogo.php?type=13&group_id=2914953)](https://sourceforge.net/p/qvge/)

**qvge** at [Softpedia.com](https://www.softpedia.com/get/Multimedia/Graphic/Graphic-Others/Qt-Visual-Graph-Editor.shtml)

### Support

Since **qvge** is a free software, it is developed in the free time on my own costs only. If you like the software and wish to support its further development, you could make a small donation using the button below:

[![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=Z35EHHJ3729GG&source=url)

Thank you!
