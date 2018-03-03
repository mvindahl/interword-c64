# Interword C64 source code

This project contains the original 6510 assembler code for the Commodore 64 port of Interword. The software was written in 1992 on a commision from Interactivision, a software company based in Silkeborg, Denmark. I was 17 at the time. The code is mainly committed to github as an artefact of historical interest.

The files were recovered from an old 5.25 inch floppy disk which had survived the past two decades in my parents' attic. It's a backup disk which was made at some point so it's most likely not the final version of the product.

The original disks, along with all original packaging and manuals, and merchandise for [unrelated software](http://www.lemonamiga.com/games/details.php?id=1900) developed by the same company, unfortunately fell victim to a cleanup back in the late 1990s, adhering to the "Ain't never gonna need this old junk again" principle. Sorry.

## Porting from the Amiga

The software was ported from the Amiga version of Interword, which was also developed by Interactivision. This was the early 1990s, and the Amiga was rapidly replacing the C64, yet it appears that there was still a business case for porting the product.

Among the features of the Amiga were an 80-char screen, menus, windows, and a distinctly blue and white look. I spent a ridiculous amount of time trying to emulate these features; far more time than was spent on features relating to actual usability.

In the end, the code wasn't finished until I had almost called it quits on several occasions, and had visited the Interactivision offices at least twice to work in crunch mode on the code.

The project paid me DKK 6,000. Not a fortune but quite OK given my age. Some of the money was spent on a stereo. Not sure about the rest.

## Code structure

The code consists of the main product, two libraries, and a menu definition file (in Danish; there was probably an English version as well).

The code was split due to memory constraints; it simply wasn't possible to fit the entire thing into memory at the same time, source code and binary and all. Instead, first one library was peeled off (lib.txt) and later another (xl.txt). The modules were linked by a jump table at the top of each library, and a corresponding jump table definition within the client file.

## Building

As far as I recall, the individual sources would be compiled to binary, and the binaries would be loaded to their respective memory locations.

I don't remember any further details and I won't be bothered to try.

## Reviews

Upon its release, the software was reviewed in a Danish computer magazine. As I recall, the gist of the review was that it was a nice achievement but also pretty unusable.

## Interword C64 on Youtube

This guy is pretty nice to the software when you consider the fact that he uncovers several major glitches in less than two minutes:

https://www.youtube.com/watch?v=4W8n6y6cuOU

# Acknowledgements

Thanks to [Mads Darø Kristensen](https://twitter.com/madsdk) for converting the floppy disk to D64 format.

Files retrieved and converted using [DiskImagery64](http://lallafa.de/blog/c64-projects/diskimagery64/) and [TMPview](http://style64.org/release/tmpview-v1.2-style)
