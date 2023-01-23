# Language

_What is the name of the language? Link the name to its webpage
(if appropriate)._

Hipacc
https://hipacc-lang.org/
https://ieeexplore.ieee.org/abstract/document/7017495

# Domain

_Describe the language's domain in five words._

Image processing for heterogenerous hardware. 

# Computational model

_We don't yet have a great definition of the term "computational model".
For now, try to come up with the clearest, most concise explanation of
what happens when a program in your DSL runs._

An image or the alternative pyramid, which is where the image's pixels
are stored, is created. The storage data structure is dependant on the target
platform.
Then there are classes which work to allow one to read and write to
an image, edit the boundaries of the pixles and iterate over windows in the
image.
Additionally there are operators which define the computation done in the
image processing.
The DSL returns an image processing algorithm, which is then compiled.
Hippac provides a source-to-source compiler which optimizes for the
specific GPU hardware for the target device/hardware.

# DSL-ness

_Fowler writes about a spectrum of languages, from general-purpose languages to
"purely" domain-specific. Where does the DSL you chose fall on this spectrum,
and why?_

Hipacc is interesting, because it created so that image processing can be
completed efficiently on a variety of devides with parallel GPUs. So, it is
in a specific domain because it is focused on efficient image processing,
but it is more broad because it works efficiently for a variety of hardware
options. Therefor, I would place it as highly but not purely domain-specific.

# Internal or external?

_Is the language implemented as an internal or external DSL?
Justify your answer._

Internal, because the components of the DSL are C++ classes, so all of the
internal Hipacc code is also valid code in C++, the general purpose language. 

# Host language

_What language(s) was (were) used to implement the DSL?_

C++

# Benefits

_Identify one potential benefit of the DSL: how is a programmer's life made
easier by the existence of this language?_

A programmer can write one image processing algorithm and given information
about the architecture of the hardware, the algorithm when compiled will be
optimized for the specific hardware.

# Drawbacks

_Identify one potential drawback of the DSL: what does a programmer
lose by using this DSL instead of a general-purpose language?_

The programmer looses ability to see the underlying data structure of the image
while coding the algorithm. The data structure is dependant on the hardware.
