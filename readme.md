hivernal
========

Winter scene in pure CSS.

|    |                                                     |
|----|-----------------------------------------------------|
| ▶️  | [play it](https://hen.cat/hivernal)                 |
| 😻 | [look at the source code](https://github.com/hendotcat/hivernal/blob/trunk/hivernal.scss) |

About
-----

This is a pure CSS implementation of a Pythagoras tree with a bit of snow as an
added flourish. By "pure CSS" I mean no extra HTML elements except for the bare
minimum required to deliver the CSS in a valid way, so no `<div class="tree">`
helper elements or anything like that.

The tree is based on the [Pythagoras tree example code on Rosetta Code][Rosetta
Code]. I haven't found anywhere else that someone's built a pythagoras tree in
CSS like this so here's how mine works. I set a brown background on the `:after`
pseudo-element on the body, and then use `clip-path` to hide the parts outside
the tree. To create the wind effect on the branches, I generate two slightly
different trees and use a keyframe animation to bounce back and forth between
them.

The snow uses the same combination of `background-color` and `clip-path` as the
tree, except with circles instead of polygons. The snow moves left as it falls
in time with the swaying of the tree, which is supposed to create a bit of a
wind effect.

This one has slightly better performance than the CPU melting [doomfire]
animation I made a couple of months ago, but it's still not really a technique
you'd want in a production website. Who cares though? It's fun as hell making
these.

And just like with doomfire, one thing I really like about this is that it
takes advantage of one of the unique strengths of CSS. In this case, it's the
swaying tree animation. Almost everywhere you find pythagoras trees, they're
a completely static image. CSS made it fairly easy to bring this one to life
with the keyframe animation, whereas most other technologies would require you
to write a bunch of extra code for that.

Oh and the name "hivernal" is Catalan. It's the adjective form of "winter", so
you could translate it as either "winter" or "wintery" depending on the context.
I like having a `.cat` domain name and I'm keen to "develop activities to
promote the Catalan culture and language" so as to fulfill the requirements of
the TLD in good faith 😇

License
-------

[![License: CC0-1.0](https://licensebuttons.net/l/zero/1.0/80x15.png)](http://creativecommons.org/publicdomain/zero/1.0/)

Hope somebody finds something in here that they find useful or inspiring.
Copy as much as you want.

[Rosetta Code]: https://rosettacode.org/wiki/Pythagoras_tree
[doomfire]: https://hen.cat/doomfire

