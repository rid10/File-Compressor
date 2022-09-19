# File-Compressor
A minimal text file compression program using Huffman algorithm.

<h2>Theory</h2>
Huffman’s algorithm takes a very simple idea and finds an elegant way to implement it. At its heart is the observation that the more a thing is mentioned, the shorter its name should be. Translated to the world of computers, it means that if a chunk of data repeats itself more than another chunk of data in the same group, it is best to encode the more occurring chunk with smaller code word. Practically what it means is that the compressed file has two parts. First there is a dictionary of code words and their corresponding chunks of data. And then there is a the data itself, encoded using codewords (often called payload in compression jargon). During decompression, the dictionary is read and the codewords are sequentially translated into actual data.

<h2>Implementation</h2>
The implementation is simple. It is very slow and not optimized for anything except coding efficiency. The alphabets are always bytes, for the sake of simplicity.

<h2>References</h2>
<link>https://www.geeksforgeeks.org/huffman-coding-greedy-algo-3</link>
<br>
<link>https://en.wikipedia.org/wiki/Huffman_coding</link>
