
a tool used to create professional-looking documents.

## advantages

1.  very quickly tackle the more complicated parts of typesetting
2. separates the content of the document from the style

## grammar

### basic structure

	\documentclass{article}     %define the type of the document

	\begin{document}
	%document
	\end{document}

### preamble

	\documentclass[letterpaper,12pt]{article}%define type of the document
	\usepackage[utf8]{inputenc}

	%between the \documentclass and \begin{document} are preambles
	\begin{document}
	%document
	\end{document}

#### what are in preambles?

1. define the type of document you are writing
2.the language you are writing in
3.the packages you would like to use
4......

### comments

	% is used for comments

## title, author and date

### title

#### in preamble

	\title{name of the title}

### author

#### in preamble

	\author{Hubert Farnsworth \thanks{funded by the Overleaf team}}
	% author and thanks

### date

#### in preamble

	\date{February 2017}

### body

	\begin{document}

	\maketitle
	% maketitle is used to place title, author and date
	\end{document}

## Bold, italics and underlining

### bold（粗体）

	\textbf{...}

### italics（斜体）

	\textit{...}

### underline（下划线）

	\underline{...}

### 突出文字

inside normal text the emphasized text is italicized, but this behaviour is reversed if used inside an italicized text

	\emph{...}

## adding images

## to see the result

compile the file

### for vim
