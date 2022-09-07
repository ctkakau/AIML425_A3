# AIML425_A3

## Assignment 3 - Convolutional Neural networks

Two problems given, Problem 2 selected

### _Problem 1_
 1D convolution (implementation should make gradient explicit):
- Use a linear discrete 1D convolution to create a database with at least
1000 entries. Each entry contains one of five “sounds”. For each entry
linearly convolve a new instance of 2000 iid Gaussian samples with one
of five different filters (impulse responses, kernels). If you play the files
over a loudspeaker (8 kHz sampling) they should sound different. One
method: Take a Hamming window shape (readily available) of suitable
length (short is good) as a first kernel (filter). Then multiply that kernel
by sin(ω t), where t ∈ Z is time, with different frequencies ω ∈ [0, π] to
create four more filters, each passing through a different frequency band.
- Design a simple 1D convolutional network using convolution, pooling and
other tools with a one-hot output that classifies the sounds in the file.
- Test and optimize your setup with suitable methods.
- Extend this toy study in one direction of your choice to provide
additional insight in the behaviour of 1D convolution (for example, what
happens with mixed signals, different file lengths, distorted filters, batch
normalization, etc.). Provide a solid motivation and reasoning.


### _Problem 2_

 Basic 2D convolution (implementation should make gradient explicit):
- Create a database of 28×28 images with at least 1000 images. The
database images each contain one circle, one triangle, or one rectangle.
The triangles and rectangles can all be of the same orientation, size, and
shape but should have random locations (so you only have to create one
basic object).
- Design a simple convolutional network using convolution, pooling and
other tools with a one-hot output to detect the shape of the objects.
- Test and optimize your setup with suitable methods.
- Extend this toy study in one direction of your choice to provide additional
insight in the behaviour of 2D convolution (for example, what happens
with object distortions, varying object orientation, multiple objects,
batch normalization, etc.). Provide solid motivation and reasoning.

