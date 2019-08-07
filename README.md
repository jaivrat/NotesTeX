# Announcement
NotesTeX v3.0 will be here by the end of August, 2019. v3.0 will include expanded language support, a redesign of mathematical environments (e.g., theorems, definitions, and examples), removal of deprecated features, and support on additional latex engines, such as, but not limited to, xetex. This major overhaul will be pushed out to CTAN by the end of September after beta testing and feedback.

<p align="center">

  <h1 align="center"><i>NotesTeX</i></h1>

  <p align="center">
    <b>An All-In-One LaTeX Notes Package For Students.</b>
    <br>
    <i>NotesTeX</i> is a modification of the original Jhep journal <br> format in order to suit the needs of students in university. 
    <br>
    <br>
    &middot;
    <b>NotesTeX v2.1</b>
    &middot;
    <br>
    &middot; 
     <a href="https://ctan.org/pkg/notestex"><strong>CTAN &raquo;</strong></a>
    &middot;
  </p>
</p>

## Table of contents
- [Update](#update)
- [Preview](#preview)
- [Installation](#installation)
- [Usage](#usage)
- [Documentation](#documentation)
- [License](#license)
- [Version and Contact](#version-and-contact) 

## Update
**28/04/2018** 
1. Changed the geometry package conditions to be more flexible.
2. Devoted a subsection to alternative language integration in [NotesTeX.pdf](NoTeX/NotesTeX.pdf), specifically Persian.
3. Discussed an issue with the ```twoside``` option.

## Preview
| ```Jhep``` Formatting | Table of Contents |
|:---:|:---:|
| [![Preview](https://raw.githubusercontent.com/adhumunt/NotesTeX/master/Sample/Sample0.png)](https://raw.githubusercontent.com/adhumunt/NotesTeX/master/Sample/Sample0.pdf)  | [![Preview](https://raw.githubusercontent.com/adhumunt/NotesTeX/master/Sample/Sample1.png)](https://raw.githubusercontent.com/adhumunt/NotesTeX/master/Sample/Sample1.pdf) |

| Margin Notes | ```amsthm``` Integration |
|:---:|:---:|
| [![Preview](https://raw.githubusercontent.com/adhumunt/NotesTeX/master/Sample/Sample2.png)](https://raw.githubusercontent.com/adhumunt/NotesTeX/master/Sample/Sample2.pdf)  | [![Preview](https://raw.githubusercontent.com/adhumunt/NotesTeX/master/Sample/Sample3.png)](https://raw.githubusercontent.com/adhumunt/NotesTeX/master/Sample/Sample3.pdf) |

| Image Integration | New ```part``` Formatting |
|:---:|:---:|
| [![Preview](https://raw.githubusercontent.com/adhumunt/NotesTeX/master/Sample/Sample4.png)](https://raw.githubusercontent.com/adhumunt/NotesTeX/master/Sample/Sample4.pdf)  | [![Preview](https://raw.githubusercontent.com/adhumunt/NotesTeX/master/Sample/Sample5.png)](https://raw.githubusercontent.com/adhumunt/NotesTeX/master/Sample/Sample5.pdf) |

## Installation
Installing just requires the following steps:

1. **Download** the [zip archive](NoTeX.zip).
2. **Build** the NotesTeX.tex file. This compile should work without a problem, and it should look like the pdf attached below.
3. **Move** the NotesTeX.sty file where ever you need it, and let your new notes file call to it as provided in the example below.

## Usage
Here is an example of a test page:

```latex
\documentclass[10pt]{article}
\usepackage{/Path/to/package/NotesTeX} %/Path/to/package should be replaced with package location
\usepackage{lipsum}

\title{{\Huge Test Page Title}\\{\Large{Test Page Subtitle}}}
\author{Author Name\footnote{\href{https://google.com/}{\textit{Author Website}}}}

\affiliation{Affiliation of Author}
\emailAdd{Email of Author}
\begin{document}
  \maketitle
  \flushbottom
  \newpage
  \pagestyle{fancynotes}
  \part{Test Part 1}
  \lipsum[1]
  \section{Subtest Section 1}
  Some notes here.\sn{With some additional sidenotes}
\end{document}
```

For right to left flowing languages, please add the following package and [Persian font](https://fontlibrary.org/en/font/xb-niloofar) just before you start the document.

```latex
\usepackage{xepersian}
\settextfont{XB Niloofar}
\setlatintextfont{Times New Roman}

\begin{document}
 ...
```
| Persian Integration |
|:---:|
| [![Preview](https://raw.githubusercontent.com/Adhumunt/NotesTeX/master/Sample/NoTeX_Persian.png)](https://raw.githubusercontent.com/Adhumunt/NotesTeX/master/Sample/NoTeX_Persian.png) |

## Documentation
All the documentation of this package is given in [NotesTeX.pdf](NoTeX/NotesTeX.pdf) and if you have any questions feel free to contact me.

## License
This material is subject to the [LaTeX Project Public License](LICENSE).

## Version and Contact

> NotesTeX v2.1.  
> Created by Aditya Dhumuntarao.  
> Date: 28 April, 2018.  
> E-mail comments and suggestions to adhumunt@gmail.com.  
