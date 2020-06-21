# Relational inductive biases, deep learning, and graph networks
## Peter W. Battaglia, Jessica B. Hamrick, Victor Bapst, Alvaro Sanchez-Gonzalez, Vinicius Zambaldi, Mateusz Malinowski, Andrea Tacchetti, David Raposo, Adam Santoro, Ryan Faulkner, Caglar Gulcehre, Francis Song, Andrew Ballard, Justin Gilmer, George Dahl, Ashish Vaswani, Kelsey Allen, Charles Nash, Victoria Langston, Chris Dyer, Nicolas Heess, Daan Wierstra, Pushmeet Kohli, Matt Botvinick, Oriol Vinyals, Yujia Li, Razvan Pascanu
* https://arxiv.org/pdf/1806.01261.pdf
* Desire *composable models* and also *relational inductive biases*. People did this in the apst before deep learning, now we should bring it back.
* Relations are property between entities - greater than more than etc.
* Structure and Flexibility not at odds
* *Inductive Bias* - if multiple good solutions exist, favor one solution over another is inductive bias. can be understood in bias variance tradeoff. For example, RNNs have sequential inductive bias
* CNN imposes translational invariance along with locality 
* RNNs impose temporal invariance, but also bias for locality
* We often want to represent sets - want to be permutaion invariant, etc. IN particular,w e care about pairwise relational structure, which is a graph 
*Multigraph - more than one edge between vertices, including self edge 
* Nodes and edge functions reused across the graph, and the graph is immune to permutation. it can also operate on graphs of different sizes and shapes 
* An edge-focused GN uses the edges as output, for example to make decisions about interactions
among entities (Kipf et al., 2018; Hamrick et al., 2018).
* A node-focused GN uses the nodes as output, for example to reason about physical systems
(Battaglia et al., 2016; Chang et al., 2017; Wang et al., 2018b; Sanchez-Gonzalez et al., 2018).
* A graph-focused GN uses the globals as output, for example to predict the potential energy of
a physical system
* paper also goes into different architectures for different applications 
