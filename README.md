# imageCompression
Mini project on Image Compression and Decompression
Data Compression is the process of reduction in size of data in order to save
space or transmission time. Information usually contains redundancies i.e
information is often repeated. Examples include reoccurring letters,
numbers or pixels. Compression programs remove this redundancy.

## Arithmetic Coding
Arithmetic coding is a common algorithm used in both lossless and lossy data
compression algorithms. It is an entropy encoding technique, in which the
frequently seen symbols are encoded with fewer bits than rarely seen
symbols.

How does Arithmetic coding work –

• It converts the entire input data into a single floating point number n
where (0.0 <= 1.0).

• The interval is divided into sub-intervals in the ratio of the probability of
occurrence frequencies.

• For a startpoint and endpoint of an entire range the lower-limit of a
character range is the upper-limit of the previous character given by
startpoint + cumulativefrequency X (endpoint -startpoint )

• Therefore, each interval corresponds to one symbol.

• The first symbol restricts the tag position to be in one of the intervals.

• The reduced interval is partitioned recursively as more symbols are
processed.

• Observation: once the tag falls into an interval, it never gets out of it.

## Huffman Coding
Huffman coding is one of the basic compression methods, that have proven
useful in image and video compression standards. When applying Huffman
encoding technique on an Image, the source symbols can be either pixel
intensities of the Image, or the output of an intensity mapping function. The
pixel intensity values in the input Image will be addressed as leaf nodes of
the Huffman tree.

Now, there are 2 essential steps to build a Huffman Tree :

1. Build a Huffman Tree :

  1. Combine the two lowest probability leaf nodes into a new node. 
  
  2. Replace the two leaf nodes by the new node and sort the nodes according to the new probability values.
  
3. Continue the steps (a) and (b) until we get a single node with
probability value 1.0. We will call this node as root

2. Backtrack from the root, assigning ‘0’ or ‘1’ to each intermediate node, till
we reach the leaf nodes

Discrete Cosine Transform A discrete cosine transform (DCT) expresses a
finite sequence of data points in terms of a sum of cosine functions oscillating
at different frequencies. DCTs are important to numerous applications in
science and engineering, from lossy compression of audio (e.g. MP3) and
images (e.g. JPEG) (where small high-frequency components can be
discarded), to spectral methods for the numerical solution of partial
differential equations.

In particular, a DCT is a Fourier-related transform similar to the discrete
Fourier transform (DFT), but using only real numbers. The DCTs are
generally related to Fourier Series coefficients of a periodically and
symmetrically extended sequence whereas DFTs are related to Fourier
Series coefficients of a periodically extended sequence. DCTs are equivalent
to DFTs of roughly twice the length, operating on real data with even
symmetry (since the Fourier transform of a real and even function is real and
even), whereas in some variants the input and/or output data are shifted by
half a sample. There are eight standard DCT variants, of which four are
common
