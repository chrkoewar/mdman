# pdftk

PDF Toolkit. Manipulate .pdf files

## commands
- `combine`     pdftk in1.pdf in2.pdf cat output out1.pdf
- `rotate`      pdftk in.pdf cat 1-end south output out.pdf
- `burst`       pdftk in.pdf burst
- `remove`      pdftk in.pdf cat 1-12 14-end output out1.pdf
- `decrypt`     pdftk secured.pdf input_pw foopass output unsecured.pdf
- `encrypt`     pdftk 1.pdf output 1.128.pdf owner_pw foopass

## examples
- `replace cover`    pdftk A=cover.pdf B=text.pdf cat A1 B2-end output final.pdf
