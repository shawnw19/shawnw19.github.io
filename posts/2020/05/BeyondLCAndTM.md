## 2020-05-30

# Beyond Lambda Calculus and Turing Machine

Like most learners I was introduced with Turing Machine as the first ubiquitous computation model upon commencement of my programming journey while Lambda Calculus remained mysterious for a period.

Later I got to know Lambda Calculus and was attracted its simplicity and intricate strong power of expression. 

During my recent stint of a small project which can be labelled as distributed computing, I searched numerous materials for computation models which I might use. I spontaneously proposed the possibility of using semilattice and Kleene algebra for modelling stream computation as in [this thesis](https://publikationen.bibliothek.kit.edu/1000012049) and shortly astonished to know that such formal methods have been used as general program analysis (some of applications are labelled as slicing problems), such like also in [here](https://pascal-group.bitbucket.io/teaching.html).

The semilattice is nothing magic but a mundane abstraction of the ‘flow’ - the foregoing irreversible forward-going process of computation, i.e. the change of status (by Dijkstra) of something. A variable, in this process, although may remain constant, is always being changed either to a different value or the same one as last step (in cpu clock).

The equality of Lambda Calculus and Turing Machine is known since the latter was invented. LC generally abstracts the computation from returning a value from one of two input variables and builds the edifice by further abstracting common procedures like iteration (by recursion to be exact) as combinators. It is like the atom-to-molecure synthesis. On the other hand, TM using several predefined structures like the reading head, status, emphasises the linear process without direct discussing the primordial computation elements.

LC is like constructing a circuit from logical gates and TM is like proving its essence of status changing. 

It is apparent that many computation models and theories after these two are also equivalent to them. Semilattice is only abstraction of the nature of flow, with nothing special as add-ons, but it causes a lot of drudgery to be used to formalise basic and simple computation process as in the foregoing thesis.

Like things that I don’t like such as Larch and other formalised languages, they never proved to be a better tool or a good supplement comparing to most existing programming languages. The programming language itself is enough to deal with complex rationale behind it and can be self-explanatory without recourse to vague and esoteric formal languages.

So does models for reactive programming, stream processing, functional programming... The concept of functional programming is much old and full of idiosyncratic credos, but in essence it is nothing but directly based on LC and TM (more on LC according its form). 

Therefore I began to realise that we need theories and thoughts that are higher based than LC and TM. The latter, of course, are the cornerstone of modern computer, is nevertheless too general to model things outside the basic framework. Just like basic rules in physics especially particle physics are seldom directly used in biology to explain phenomena of organisms, LC and TM does not go beyond the basic rules of computer physics.

It would be very interesting to rethink various theories in computation from this perspective. Object-orientedness may be one good example of parallel theory as I don’t find any clue that it can be deducted from LC/TM directly. The attributes of objects remain stable or prone to be altered but are always hooked to the object, which is against the change of status. Each process can be regarded as an abstract computing machine during its execution, so even does the concept object. The saying by Alan Kay that for him OO messaging suggests that communication exists among more than one abstract machine. LC/TM generally is about what happens on a single machine.

Using theories that are in essence same for analysis of situations beyond them can be dangerous and leads to futility. In fact inventors of early computers are electrical engineers who were not familiar with Alonzo Church or Alan Turing. Logical gates and status storage which were both available for decades provided room for imagination of more subtle usage of them which is actually general digital computers. Von Neumann architecture is not genius invention from void but development of existing ideas.

To conclude we should keep a balance view of major theories behind the computing machines. Many new things, programming paradigms are disguised by decades-old even century-old conventional things. It's impossible to have new emerged problems solved with LC/TM level abstraction. The real innovation is precious.

ps In Computation: finite and infinite machines by Marvin Minsky, a book appeared 2 years before his book on neural networks, is an elaboration of TM that is obscure by nature. I highly doubt that his and most subsequent people's treatment of neural networks is the same that none of them went beyond simple TM model. An example is The pattern on the stone: the simple ideas that make computers work by Hillis, W. Daniel.
