# Inline SVG to PNG

This tool is created because for most HTML to PDF tools([ref SE discussion](https://unix.stackexchange.com/questions/533886/is-there-a-command-line-tool-for-converting-html-files-to-pdf)), they don't support SVG.

The script requires ./static/svg2png.jar, which can be found in https://github.com/sterlp/svg2png/releases (Apache 2.0 License).

Example Usage:
```
python3 ./scripts/inline_svg2png.py ./out/helloworld.html
# ./out/img created with SVGs and PNGs, and  ./out/_helloworld.html created
```

After a HTML doc is created, it can be transformed to PDF via `pandoc`, for example:
```
pandoc -f html -t pdf ./out/_helloworld.html -o ./out/helloworld.pdf
```
