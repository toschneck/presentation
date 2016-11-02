## Convert slides to PDF with decktap

https://github.com/astefanutti/decktape

`docker run -u 1000:1000 --rm -v $(pwd):/slides astefanutti/decktape --size 1920x1200 -p 2000 --slides 4  /slides/index.html /slides/slides.pdf`
