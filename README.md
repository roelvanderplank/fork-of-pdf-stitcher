# FORK of PDF Stitcher.

Reason for fork: I am contemplating using the 'stitcher' app to solve a problem with posterizing Prezi's:
https://getsatisfaction.com/prezi/topics/you_should_sell_poster_sized_prints_of_a_prezi?topic-reply-list[settings][filter_by]=all&topic-reply-list[settings][reply_id]=16611348#reply_16611348


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
