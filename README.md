# The `fetchcls` package

With standard LaTeX you are able to check for the class in use
invoking the kernel command `\@ifclassloaded`.
However, doing so you can't get the explicit class name
(unless you want to loop over every possible class name
until `\@ifclassloaded` returns true -- don't do that!)
With the present package you can get the name with significantly less effort.
Just load the package as usual:

    \begin{flushleft}
      \cs{usepackage}\{fetchcls\}
    end{flushleft}
    
Then, the control sequence `\classname` will hold the name of the current class.

This is version 1.0 of the package.

Copyright (C) 2015 by Ruben Giannotti

---

This work may be distributed and/or modified under the conditions of the LaTeX Project Public License, either version 1.3c of this license or (at your option) any later version. The latest version of this license is in http://www.latex-project.org/lppl.txt and version 1.3 or later is part of all distributions of LaTeX version 2005/12/01 or later.

This work has the LPPL maintenance status `maintained'.

The Current Maintainer of this work is Ruben Giannotti.

This work consists of the files
  fetchcls.dtx
  fetchcls.ins
and the derived file fetchcls.sty.

To install the package

 1. run latex `fetchcls.ins`
 2. move 'blocktable.sty' to locations where LaTeX will find it
