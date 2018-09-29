


This is an experimental font for makinig J look like APL.

Currently based on the Menlo font, looking to do something different later.


# https://en.wikipedia.org/wiki/APL_syntax_and_symbols
# https://code.jsoftware.com/wiki/NuVoc
# https://news.ycombinator.com/item?id=8605606

#### Dyads

#  Add    A+B +
#  Subtra A−B -
#  Multip A×B *
#  Divide A÷B %
#  Expone A⋆B ^
#  Circle A○B o.
#  Deal   A?B ?
#  Member A∈B e.
sub e period by element;

#  Maximu A⌈B >.
#  Minimu A⌊B <.
#  Reshap A⍴B $
#  Take   A↑B {.
sub braceleft period by arrowup;

#  Drop   A↓B
sub braceright period by arrowdown;

#  Encode A⊤ΤB p..
# Not the best choice of unicode,
# but menlo doesn't have Top
sub p period period by Tau;

#  Decode A⊥B p.
# Not the best choice of unicode,
# but menlo doesn't have Bottom
sub p period by SF070000;

#  Residu A∣|B |
#  Catena A,B
#  Expans A\B
# No direct correspondence,
# but prefix should be similar to dyadic backslash

#  Compre A/B
# No direct correspondence,
# But similar to table

#  Index  A⍳B i.
#  Matrix A⌹B %.
#  Rotati A⌽B |.
#  Rotati A⊖B |."1
#  Logari A⍟B *.
#  Dyadic A⍕⏁⍕₮B ":
# Not perfect due to Apl functional symbol up tack jot
# not being supported in menlo
sub quotedbl colon by uni20AE;

#  Genera A⍉B |:
#  Combin A!B !
#  Diaere A¨B
sub e a c h space by dieresis;

#  Less t A<B <
#  Less t A≤B <:
sub less colon by lessequal;

#  Equal  A=B =
#  Greate A≥B >:
sub greater colon by greaterequal;

#  Greate A>B >
#  Not eq A≠B ~:
sub similar colon by notequal;

#  Or     A∨B +.
sub plus period by logicalor;

#  And    A∧B *.
sub asterisk period by logicaland;

#  Nor    AṽB +:
sub plus colon by uni1E7D;

#  Nand   A⌅B ⊼*:
sub asterisk colon by uni2305;

#  Left   A⊣⇽B [
sub bracketleft by uni21FD;

#  Right  A⊢⇾B⊢˫ͱ ]
sub bracketright by uni21FE;


#### Monads

# Assignment A←B =:
sub equal colon by arrowleft;

#  Roll    ?B
#  Ceiling ⌈B >.
sub greater period by uni2308;

#  Floor   ⌊B <.
sub less period by uni230A;

#  Shape,  ⍴B $
sub dollar by uni2374;

#  Not, Ti ∼B ~
sub asciitilde by similar;

#  Absolut ∣| B # not represented in menlo
#  Index g ⍳B i.
sub i period space by uni2373;
sub i period by uni2373;

#  Negatio −B -
sub hyphen by minus;

#  Identit +B +
#  Signum  ×B *
sub asterisk by multiply;

#  Ravel,  ,B ,
#  Matrix Inverse  ⌹B %.
sub percent period by uni2339;

#  Recipro ÷B %
sub percent by divide;

#  Pi time ○B
sub o period by circle;

#  Logarit ⍟B *.
sub asciicircum period by uni235F;

#  Exponen ⋆B *
sub asciicircum by uni22C6;

#  Reversa ⌽B |."1
sub bar period quotedbl one by uni233D;

#  Reversa ⊖B |.
sub bar period by uni2296;

#  Grade u ⍋B /:
sub slash colon by uni234B;

#  Grade d ⍒B
sub backslash colon by uni2352;

#  Execute ⍎B ??? No known analog
#  Monadic ⍕B ???
#  Monadic ⍉B |:
sub bar colon by uni2349;

#  Factori !B !

