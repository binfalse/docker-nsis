# Docker image for NSIS

The [Dockerfile](Dockerfile) contains a recipe for a Docker image, that can be used to build [NSIS](https://nsis.sourceforge.io/Main_Page) installers.
The image is available precompiled from [binfalse/nsis](https://hub.docker.com/r/binfalse/nsis).

## Usage

Just mount your NSIS build scripts and resources to `/build` and add the relative path to your NSIS script as an argument.
Let's assume your script is called `install.nsi`, then you would call

    docker run --rm -v /path/to/resources:/build binfalse/nsis install.nsi

## License

    MIT License
    
    Copyright (c) 2020 Martin Scharm <https://binfalse.de/contact>
    
    Permission is hereby granted, free of charge, to any person obtaining a copy
    of this software and associated documentation files (the "Software"), to deal
    in the Software without restriction, including without limitation the rights
    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
    copies of the Software, and to permit persons to whom the Software is
    furnished to do so, subject to the following conditions:
    
    The above copyright notice and this permission notice shall be included in all
    copies or substantial portions of the Software.
    
    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
    SOFTWARE.
