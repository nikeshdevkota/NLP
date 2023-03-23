# Natural Language Processing
## Lesson 10

<h3> Byte Pair Encoding Algorithms </h3>

The BPE algorithm proceeds as follows:

* Initialize the vocabulary with all of the single-byte characters in the text.

* Compute the frequency of all pairs of adjacent bytes in the text.

* Find the most frequent byte pair in the text, and add it to the vocabulary as a single, unused byte.

* Replace all occurrences of the most frequent byte pair in the text with the new byte.

* Repeat steps 2-4 until a predetermined number of iterations have been completed, or until the desired level of compression has been achieved.
