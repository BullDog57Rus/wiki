# Computational logic
## Decoder
A decoder is a logic block that has an n-bit input and
2<sup>n</sup> outputs where only one output is asserted for each input
combination.

Example of 3 to 8 decoder:
![picture of decoder][decoder]
![picture of decoder's truth table][decoder_truth_table]
Example with gates:
![picture of decoder with gates][decoder gates]

## Multiplexers
A multiplexer is a logic block that has 2<sup>n</sup> bit input and n-bit selector
and 1 output which is one of the n inputs based on the selector value 
 
A selector value (or control value) is the control signal
that is used to select one of the input values of a multiplexer as
the output of the multiplexer.

Basically, multiplexers select which value will go through, all others are blocked.

Example of two-input multiplexer on the left and its implementation with
gates on the right:
![picture of multiplexer][multiplexer]

## Demultiplexers
The demultiplexer performs the function of the inverse multiplexer
– it commutes the input signal to the desired output the number
of which is set by the selector. The other outputs are set to 0.

Example of 1-to-4 demux:
![picture of demux][demux]


## Programmable Logic Array
A Programmable Logic Array (PLA) - structured-logic element
composed of a set of inputs and corresponding input complements
and two stages of logic:
 * The first generates product terms of the inputs
 * The second generates sum terms of the product terms.
Therefore, PLAs implement logic functions as a sum of products.
![picture of pla][PLA]

PLA is currently not used because they are not fast enough, consumes a lot of voltage and have large number of gates



[demux]: ./images/demux.png
[PLA]: ./images/pla.png
[multiplexer]: images/multiplexer_example.png
[decoder]: ./images/decoder.png
[decoder_truth_table]: ./images/decoder_truth_table.png
[decoder gates]: ./images/decoder_gates.png