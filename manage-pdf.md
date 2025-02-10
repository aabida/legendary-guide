# Prerequisite
To be able to use commands, please install ImageMagick : https://imagemagick.org/script/download.php


## To merge pdf files :
pdfunite file1.pdf file2.pdf fileN.pdf output-file.pdf

## To reduce file size :
Use ghostscript
Example :
```bash
gs -sDEVICE=pdfwrite -dCompatibilityLevel=1.4 -dPDFSETTINGS=/ebook -dNOPAUSE -dQUIET -dBATCH -sOutputFile=output.pdf input-file.pdf
```
where : 

-   `-dPDFSETTINGS=/screen`  lower quality, smaller size. (_72 dpi_)
-   `-dPDFSETTINGS=/ebook`  for better quality, but slightly larger pdfs. (_150 dpi_)
-   `-dPDFSETTINGS=/prepress`  output similar to Acrobat Distiller "Prepress Optimized" setting (_300 dpi_)
-   `-dPDFSETTINGS=/printer`  selects output similar to the Acrobat Distiller "Print Optimized" setting (_300 dpi_)
-   `-dPDFSETTINGS=/default`  selects output intended to be useful across a wide variety of uses, possibly at the expense of a larger output file

## To convert an image to a pdf file :

```bash
convert image-file.jpg output-file.pdf
```

## Murge multiple jpg to one pdf :
```bash
convert `ls -v *.jpg` output.pdf
```

## Rotate an image
```bash
convert file.jpg -rotate 90 output.jpg
```

## Scale an image
```bash
convert image.png -scale 30% new-image.png
```
