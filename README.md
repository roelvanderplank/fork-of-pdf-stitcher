#Use of this program: this program is used to change a specially crafted PDF file into 1 single ('huge') PDF file.
For more info see e.g.
https://getsatisfaction.com/prezi/topics/you_should_sell_poster_sized_prints_of_a_prezi?topic-reply-list[settings][filter_by]=all&topic-reply-list[settings][reply_id]=16611348#reply_16611348

## Usage:
* Download the exe file (from the bin folder)
* Download the pattern.txt file (from the bin folder)
* Put both of them in the same directory
* Create the specially crafted PDF file, put it in the same directory
* Assuming the specially crafted PDF file is named 'yourprezi.pdf' open a CMD window and type:
* Prezi_poster_pdf_stitcher.exe yourprezi.pdf pattern.txt prezi_poster.pdf
This should give you a prezi_poster.pdf file, in which the 16 pages (or actually: 20 pages) from the original pdf file (yourprezi.pdf) is stitched together in one pdf file, which you could e.g. print on a large poster.

# FORK of PDF Stitcher.

Reason for fork: I am contemplating using the 'stitcher' app to solve a problem with posterizing Prezi's:
https://getsatisfaction.com/prezi/topics/you_should_sell_poster_sized_prints_of_a_prezi?topic-reply-list[settings][filter_by]=all&topic-reply-list[settings][reply_id]=16611348#reply_16611348

Licences etc: as this program is a 99% copy of the Lageos/pdf-stitcher project (and uses libraries and licences from other projects), the licence is essentially the same as that of the Lageos/pdf-stitcher.
The exe file is created from the py file in the bin-folder, using the pyinstaller package (see e.g. http://www.pyinstaller.org/).

Text below is from original project (Lageos/pdf-stitcher)
---------------------------------------


# PDF Stitcher

Different means to stitch sewing patterns (or any pdf file) delivered in single sheets to a whole plan (file).

## Prerequisites
* Python (tested with python 2.7.10 Anaconda 64-bit)
* PyPDF2 (tested version 1.25.1, https://pypi.python.org/pypi/PyPDF2/1.25.1 )
        install with `pip install PyPDF2`

## Usage
`python pdf_stitcher.py input.pdf Pattern.csv output.pdf`

With Pattern.csv decribing the placement of the pages (specified with the page
number) in the output-file:
![pdf_stitcher flow](https://smidgeonpigeon.files.wordpress.com/2016/01/pdf_stitcher_flow1.png "pdf_stitcher flow")

The easiest way to create this file is with a simple text editor.

Stitching is done with no spacing between pages.
