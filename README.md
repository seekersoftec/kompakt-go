# Kompakt

Kompakt is a general-purpose data compression library that aims to achieve a compression ratio of approximately 1024:1. The library uses multi-threaded PAQ-based lossless compression archivers to reduce data by approximately 80% - 100%.

For a compression ratio of 1024:1, we have 1GB - 1MB. This means that the compressed data will be approximately 1/1024th of the original size. For example, if you have 1GB (1024 megabytes) of data, after compression with a compression ratio of 1024:1, the compressed data will be approximately 1MB.

## COmpression size Goals
- 100MB (~10% of 1GB)
- 10MB (~1% of 1GB)
- 1MB (~0.10% of 1GB)

## Some Ideas

**Hash-based compression:** If a hash can be reversed, data can be compressed into the tiniest pieces, i.e., hashing data before compression can help reduce its size by a thousand-fold.

**Neural Network-based compression:** Using Deep learning by harnessing Neural Network-based modeling combined with arithmetic coding; For this, the models are first trained, and the trained models shipped along with the compression/decompression program i.e each model has a unique number (hashed and encoded). That number is what identifies the model that was used to compress that data so that the data can be decompressed by the appropriate model(Referenced from DZip-torch).

**Dictionary-based compression:** Group data into 4 hexadecimal forms, then generate a dictionary based on it. i.e 16 Permutation 4

**Questions:**

- How to reverse a hash data to its original form?
- Would the mixture of encoding algorithms such as Shannon, huffman, and Lempel-Ziv give a middle-out compression algorithm?

**Algorithms:**

- Shannon
- Huffman
- Lempel-Ziv
- Prediction by Partial Matching (PPM)



## Basic Benchmark Goal
 - Use the one from [Hutter Prize](http://prize.hutter1.net/) => might be too ambitious 
