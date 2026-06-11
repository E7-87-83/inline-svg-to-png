The script requires ./static/svg2png.jar, which can be found in https://github.com/sterlp/svg2png/releases (Apache 2.0 License).


Example Usage:
```
python3 ./scripts/inline_svg2png.py ./out/helloworld.html
# ./out/img created with SVGs and PNGs, and  ./out/_helloworld.html created
pandoc -f html -t pdf ./out/_helloworld.html -o ./out/helloworld.pdf
```
