# Speech-recogniton-using-RNN
Speech is human’s most efficient communication
modality. Beyond efficiency, humans are comfort and
familiar with speech. Other modalities require more
concentration, restrict movement and cause body strain due
to unnatural positions. Research work on English speech
recognition, although lagging that other language, is
becoming more intensive than before and several researches
have been published in the last few years . Automatic
speech recognition is a process by which a machine
identifies speech. The conventional method of speech
recognition insist in representing each word by its feature
vector & pattern matching with the statistically available
vectors using neural network . The promising technique
for speech recognition is the neural network based
approach. Artificial Neural Networks, (ANN) are
biologically inspired tools for information processing.
Speech recognition modeling by artificial neural networks
(ANN) doesn’t require a priori knowledge of speech process
and this technique quickly became an attractive alternative
to HMM . RNN can learn the temporal relation ship of
Speech – data & is capable of modeling time dependent
phonemes.

#RECURRENT NEURAL NETWORK ARCHITECTURE FOR SPEECH RECOGNITION
RNN have feedback connections and address the temporal
relationship of inputs by maintaining internal states that
have memory. RNN are networks with one or more
feedback connection. A feedback connection is used to pass
output of a neuron in a certain layer to the previous layer(s).
The difference between MLP and RNN is RNN have
feedforward connection for all neurons (fully connected).
Therefore, the connections allow the network show the
dynamic behavior. RNN seems to be more natural for
speech recognition than MLP because it allows variability in
input length .
The motivation for applying recurrent neural
network to this domain is to take advantage of their ability
to process short-term spectral features but yet respond to
long-term temporal events. Previous research has
confirmed that speaker recognition performance improves
as the duration of utterance is increased . In addition, it
has been shown that in identification problems. RNNs may
confer a better performance and learn in a shorter time than
conventional feedforward networks.
Recently a simple recurrent neural network, which has
feedback connections of self-loop type around hidden layer
units, has been proposed as an attractive tool for
recognizing speech sounds including voiced plosive sounds
.This network has three layers such as input layer,
hidden layer and output layer. Each of the output layer
units has feedback connection with itself, i.e., a self-loop as
shown in below figure.
Fully recurrent networks feed back the hidden layer to
itself. Partially recurrent networks start with a fully
recurrent net and add a feedforward connection that
bypasses the recurrency, effectively treating the recurrent
part as a state memory. These recurrent networks can have
an infinite memory depth and thus find relationships
through time as well as through the instantaneous input
space. Most real-world data contains information in its time
structure. Recurrent networks are the state of the art in
nonlinear time series prediction, system identification, and
temporal pattern classification.

<img width="339" align="centre" alt="Screenshot 2023-09-08 at 5 02 54 PM" src="https://github.com/Innovativeanku/Speech-recogniton-using-RNN/assets/130054612/7389b9ff-1beb-4187-97db-045014bcfa70">

Fig RNN Architecture

Actually this architecture has been used in visual
pattern recognition but we use this architecture for
speech recognition especially for English speech recognition
by using Backpropagation Through Time (BPTT)as learning
algorithm. This architecture also have been proved that
this architecture is better than MLP in phoneme
recognition accuracies by using Backpropagation
algorithm.
The Backpropagation Through Time (BPTT) algorithm
is based on converting the network from a feedback
system to purely feedforward system by folding the
network over time. Thus, if the network is to process a
signal that is time steps long, then copies of the network are
created and the feedback connections are modified so that
they are feedforward connections from one network to the
subsequent network. The network can then be trained if it is
one large feedforward network with the modified weights
being treated as shared weight.
