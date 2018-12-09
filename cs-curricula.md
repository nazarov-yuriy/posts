[Original material](http://sharpc.livejournal.com/67583.html) by Denis Ostapenko

[Original translation](http://vissi.su/translations/programmer-teormin.php) by Vissi

Most apprentice software developers, especially those, who study in colleges, do
not know how to develop their skills, and what they should know to work 
effectively. Surprisingly, everyday usage of products and technologies, 
invented by other developers and based on well-developed knowledge areas, 
does not give them an idea how they work, and how they are implemented.

Queueing theory and GSM-based mobile networks; PHP scripts, running at remote 
servers, transfering generated content through Ethernet using TCP/IP protocol 
to network cards with NDIS interface on user PCs; CPUs, reordering and 
speculatively executing instructions to compensate semiconductor electronics 
limitations on clock rate and light speed; computer-designed cars and planes, 
drugs and DNA sequenced by computers; computer games, where a tiny patch of 
reflected light need megabytes of scientific articles full of Fresnel integrals;
electronic movies and books; NLP and TreeNet algorithms, retrieving search 
results from huge databases — these are the things we use every day, that were
created by ingenious software developers, by virtue of their fundamental 
knowledge and talent, and, of course, software development and complexity 
management methodology, proven over the years.

My friends and I have taken the trouble of preparing a software developers' 
theoretical minimum based on remarkable IT areas, some parts of which are 
already included in CS university programmes, the others are taken from 
interviews and practical experience. Some items require only Wikipedia and 
take 5 minutes to learn, others would take up months, but this is exactly what
you need to know and understand. You are welcome to suggest corrections 
and additions.

1. [**C++**](https://en.wikipedia.org/wiki/C%2B%2B),
[standard](https://www.iso.org/standard/25845.html),
[Comeau](https://en.wikipedia.org/wiki/Comeau_C/C%2B%2B),
[1TBS](https://en.wikipedia.org/wiki/Indentation_style#Variant:_1TBS_%28OTBS%29),
[Stroustrup](http://www.stroustrup.com/4th.html) /
[D&E](http://www.stroustrup.com/dne.html) /
[Josuttis](http://www.josuttis.com/libbook/) /
[Vandevoorde](https://www.pearson.com/us/higher-education/product/Vandevoorde-C-Templates-The-Complete-Guide/9780201734843.html) , 
[Dewhurst](https://www.pearson.com/us/higher-education/program/Dewhurst-C-Common-Knowledge-Essential-Intermediate-Programming/PGM209409.html) /
[Mayers](https://books.google.com/books/about/Effective_C++.html?id=eQq9AQAAQBAJ) /
[Sutter](https://en.wikipedia.org/wiki/Herb_Sutter),
[RAII](https://en.wikipedia.org/wiki/Resource_acquisition_is_initialization),
[rule of three](https://en.wikipedia.org/wiki/Rule_of_three_%28C%2B%2B_programming%29),
[exception-safety](https://en.wikipedia.org/wiki/Exception_safety), 
[Alexandrescu](https://en.wikipedia.org/wiki/Andrei_Alexandrescu#Bibliography) /
[Abrahams-Gurtovoy](https://discourse-production.oss-cn-shanghai.aliyuncs.com/original/3X/0/0/00329b35761ebb8cefec388d4423481dc836486f.pdf),
[type erasure](https://en.wikipedia.org/wiki/Type_erasure),
[CRTP](https://en.wikipedia.org/wiki/Curiously_recurring_template_pattern),
[NVI](https://en.wikipedia.org/wiki/Non-virtual_interface_pattern),
[SFINAE](https://en.wikipedia.org/wiki/Substitution_failure_is_not_an_error),
[Koenig lookup](https://en.wikipedia.org/wiki/Argument-dependent_name_lookup), 
[Duff's device](https://en.wikipedia.org/wiki/Duff%27s_device),
[Boost](https://en.wikipedia.org/wiki/Boost_%28C%2B%2B_libraries%29),
[Siek-Lumsdaine](https://dl.acm.org/citation.cfm?id=1167499) /
[Karlsson](http://www.xwood.net/docs/pdf/Beyond%20the%20C++%20Standard%20Library_201611291716.pdf),
[TR1](https://en.wikipedia.org/wiki/C%2B%2B_Technical_Report_1),
[TR on C++ performance](http://www.open-std.org/jtc1/sc22/wg21/docs/18015.html),
[ABI](https://en.wikipedia.org/wiki/Application_binary_interface),
[Stepanov test](http://www.open-std.org/jtc1/sc22/wg21/docs/D_3.cpp),
[forwarding problem](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2002/n1385.htm),
[SPECS](http://users.monash.edu/~damian/papers/HTML/ModestProposal.html),
[C++0x](https://www.iso.org/standard/38110.html)

2. **Compilers**, standard implementation differences, 
implementation limitations, intrinsics, 
standard library differences (containers, rand), ABI, 
implementation of virtual functions, virtual inheritance, exceptions, RTTI, 
switch, function and method pointers; optimizations, copy elision (RVO, NRVO),
sizeof on different platforms, defines of compilers and environments, 
__declspec, compiler command line, empty-base optimization, 
static and dynamic linking, mangling, distributed compilation, 
precompiled header, single compilation unit, (strict) aliasing/restrict,
inline/_forceinline, volatile

3. **Multithreading**, dining philosophers problem,
deadlock/race condition/starvation, atomicity, CPU lock instructions,
CAS or LL/SC, wait/lock/obstruction-free, ABA problem, 
lock-free container implementation, spin-lock, TLS/per-thread data, OpenMP, 
MPI, map-reduce, critical section/mutex/semaphore/condition variable,
WaitForSingleObject/WaitForMultipleObjects, green thread/coroutine, pthreads,
actor model

4. **x86 assembly language**, Zubkov/Hyde/Drepper/Kasperski/Fog/Abrash, 
AT&T and Intel syntax, masm32, macro instructions, stack, heap/heap manager,
calling conventions, hex-codes, machine data representation, IEEE754,
little/big endian, SIMD, hardware exceptions, interrupts, virtual memory,
reversing, stack and heap overflow, return oriented programming, 
alphanumeric shellcode, L1/L2/RAM/page fault and their timings

5. **Hardware**, Horowitz-Hill, semiconductor electronics/spintronics/photonics,
transistor, circuitry, microcode, processor technology, VID/PID, FPGA, 
Verilog/VHDL/SystemC, SISAL, Arduino, 
memory (ROM → EEPROM, RAM, SSD, HDD, DVD), RISC/CISC, 
Flynn's taxonomy ([SM]I[SM]D), Harvard and Princeton computer architecture, 
CPU architectures, x86 architectures

6. **Processors**, pipelining, hyper-threading, out-of-order execution, 
speculative execution, branch predict, prefetching, set-associative cache, 
cache-line/cache-miss, clock cycle, protection rings, 
multiprocessor systems memory models (SMP, NUMA), memory timings

7. **Discrete math**, K2, Post theorem, circuits, finite automata, 
cellular automata, Kalashnikov rifle, DFA and NFA

8. **Computability**, Turing machine, Markov algorithms, Post machine,
Hilbert's tenth problem, Church lambda functions, 
Clini partial recursive functions, Schönfinkel combinatory logic, Brainfuck, 
Turing tarpit equivalence, halting and self-applicability problems, 
countability of computable functions set, RAM-machine, Tarsky algorithm, 
SAT/SMT-solvers, formal systems theory

9. **Programming languages**, grammars, Chomsky hierarchy, 
Myhill-Nerode theorem, pumping lemma for regular languages and Ogden's lemma,
Clini algebra, NFA → DFA, undecidable problems in formal languages, Dragonbook,
Friedl, regular expressions and their complexity, PCRE/POSIX RE, BNF, 
Boost.Spirit + Karma + Qi/Ragel, LL, LR/SLR/LALR/GLR, PEG/packrat, 
yacc/bison/flex/antlr, static code analysis, 
compilation/decompilation/obfuscation/deobfuscation, Clang/LLVM/XMLVM, GCCXML,
OpenC++, VM implementation, JiT/AoT/GC, DSL/DSEL

10. **Algorithms and combinatorial optimization**, 
Cormen/Skiena/Sedgewick/Knuth/Aho-Hopcroft-Ullman/Papadimitriou/Shriver-Goldberg/Preparata-Shamos,
data structures, algorithms, complexity and Landau symbols, complexity classes, 
NP-complete problems, graphs and trees, network flows, Kirchhoff matrix,
search trees (especially RB-tree and B-tree), occlusion detection, binary heap,
hash tables and perfect hash, Petri nets, 
Russian peasant multiplication algorithm, 
Karatsuba method and Winograd-Strassen matrix multiplication, 
sorting algorithms, greedy algorithms and matroids, dynamic programming, 
linear programming, diff algorithms, randomized and fuzzy search algorithms, 
pseudorandom numbers, fuzzy logic

11. **Numerical methods**, dichotomy/Newton method, inter- and extrapolation, 
splines, Gauss/Jakobi/Seidel methods, QR and LU-decomposition, SVD, 
Least squares, Runge-Kutta methods, Adams method, Newton-Cotes formulas, 
Monte-Carlo method, Ritz method, Bubnov-Galerkin method, 
finite difference/element method, FFT/STFT, convergence and stability

12. **Machine learning**, machine vision, OpenCV, image processing, OCR, 
Zobel filters, Haar-like features, introduction to vision psychophisiology, 
TreeNet, neural networks, Kohonen self-organizing map, genetic algorithms,
ant colony algorithms, 
information retrieval/data mining/natural language processing, 
optimization algorithms, PCA, SVM, gradient boosting, simulated annealing, 
hill climbing, AI modeling methods

13. **Information theory**, compression, Huffman, RLE, LZ, ECC,
lossy compression (images, audio, video), information entropy, Shannon formula,
Kolmogorov complexity

14. **Cryptography**, Yaschenko, symmetric (DES, AES), asymmetric (RSA),
Diffie-Hellman, elliptic curves, hashing (MD5, SHA, CRCn), DHT, 
cryptographically strong systems, cryptographic attacks, 
WEP/WPA/WPA2 and attacks, digital signatures and certificates, HTTPS/SSL, 
zero-knowledge proof

15. **Math**, Knuth-Graham-Patashnik/Zorich/Winberg/
Rudin (Real and complex analysis, not Principles)/Lang, calculus, 
linear algebra, complex analysis, functional analysis, differential geometry, 
number theory, PDE/ODE/integral equations/variations calculus/optimal control, 
generating functions, series, combinatorics,
probability theory/mathematical statistics/random processes/queueing theory,
Markov chains, integral transforms (Fourier, Laplace, wavelet), NZQRCHOS, 
computer algebra (Mathematica, Maple)

16. **Physics**, Kirchoff rules, electrical impedance,
velocity and frequency of light, Lagrangian

17. **Chemistry**, stoichiometry, silicon chemistry :)

18. **Architecture and code style**, 
McConnell/Fowler/Leblanc/Gamma/Alexandrescu-Sutter/Booch, 
defensive programming, patterns, GRASP, UML, OOP (Smalltalk), OOD/OOA, 
Liskov substitution principle, code metrics

19. **Software development methodologies**, Waterfall/RUP/Agile/Scrum/Kanban/XP,
TDD/BDD, CASE

20. **Testing**, unit tests, functional, load, integration testing, UI testing

21. **IDE**, IntelliSense, 
debuggers (VS/Olly/WinDbg/kdb/gdb) and tracers (strace/ltrace), 
DWARF2 debug information format, valgrind, vcs (SVN, GIT), merge/branch/trunk, 
file and branch naming systems, continuous integration, ant, code coverage, 
static analysis,
software verification and validation (Frama-C, RAISE (RSL), Coq), profiling,
lint, bug trackers, documentation generators, build systems (cmake)

22. **Frameworks**, Qt, moc and metainformation, signals and slots construct, 
Summerfield-Blanchett/Schlee, PoCo, common libraries: GMP, i18n, lapack, fftw,
pcre

23. **Operating systems**, Silberschatz/Richter/Solomon-Russinovich/Robachevsky/
Vahalia/Stevens/Linux Kernel Internals, memory manager, 
heap manager and its internals (LAL/LFH/slab), process manager, context switch, 
real and protected mode, executable formats (PE/ELF/Mach), kernel objects, 
debug hooks (strace/ptrace/dtrace/pydbg, Debug API) and minidumps, bash,
network stack and high-load web servers, netgraph, CR0, IPC, window subsystem, 
security: ACE/ACL and access rights, virtualization technologies, RTOS (QNX), 
driver development, IRQL, IRP, file systems, BigTable, 
NDIS/miniport/FS drivers/filter driver, Mm-, Io-, Ldr-functions, 
DKOM and rootkits, GDT/IDT/SDT, Windows/Linux/BSD kernel, POSIX

24. **COM**, OLE/ActiveX/COM+, ATL, Rogerson/Tavares, apartments, monikers, 
MIDL, DCOM RPC, CORBA, D-bus, TAO

25. **Networking**, OSI model/Internet model, Ethernet, TCP/IP, TCP window, 
Nagle algorithm, sockets, Protocol buffers/Thrift/Avro/ASN.1, AMQP, ICMP, 
routing/BGP/OSPF, ARP, Mitnick attack, syn flood, HTTP/FTP, P2P, DHCP, SMB/NBNS, 
IRC/XMPP, POP3/SMTP/ESMTP/IMAP, DNS, WiFi/WiMax/GSM/CDMA/EDGE/Bluetooth, ACE,
Wireshark

26. **Graphics**, Bresenham algorithm, color models, 
ray tracing vs polygonal graphics, OpenGL/GLSL/Open Inventor, 
DirectX/DirectShow/DirectAudio/HLSL, stencil/depth/alpha-test, 
DirectX 11 graphics pipeline, shaders, lighting models (Phong), throughput,
fillrate, OpenCL/CUDA, landscapes, LODs, shadows, textures and filtering, 
antialiasing, HDR, tone mapping

27. **Formats**, XML/XSLT/XPath/XMLStarlet/DOM/SAX, RTF/ODF, JSON/BSON, torrent,
YAML, JPEG/PNG/WebP, AVI/MPEG/RIFF/WAV/MP3/OGG/WebM, SVG, Unicode, 
single-byte encodings/UTF-8/UTF-16/UCS-2/UTF-32

28. **RDBMS**, Gruber, ANSI SQL, T-SQL, ODBC, 
MySQL/PostgreSQL/MS SQL/BDB/SQLite/Sphinx, stored procedures, triggers, 
Codd/А algebras, Tutorial D, normal forms, query optimization and execution, 
index data structures, transactions and ACID, Brewer's CAP theorem, NoSQL, 
key-value storage, sharding, ORM (C++ ODB), ERD, OLAP

29. **Application programming**, C#/F#/Nemerle, Schildt/Troelsen/Richter, 
generic programming, yield, linq/plinq, reflection, AST, WCF, 
WinForms/WPF/Silverlight, AOP, logging frameworks, .NET assembly

30. **Quantum computing**, Shor's algorithm, quantum cryptography

31. **Functional programming**, Haskell/Ocaml/Scheme/Alice or Oz, 
SICP/TaPL/YAHT/Purely Functional Data Structures/Harrison-Field, 
HOF (map/fold/filter), Hindley-Milner type system, monads, typeclasses, 
algebraic data types, dependent types, lazy/eager evaluation, 
logic programming (Prolog or Mercury), concurrent programming (Erlang or Oz)

32. **Web development and scripting languages**, 
Flanagan/Zend PHP5 Certification Course + Study Guide, Apache/nginx, 
CGI/FastCGI, PHP/Zend Framework/phpDaemon/Zend Engine/Doctrine or 
Propel/CodeIgniter or Symphony or Yii, Python/Django/Twisted, Ruby/RoR, 
ASP.NET MVC, JavaScript/jQuery/ExtJS/node.js, JS OOP, 
HTML5/XHTML/doctype/table and div layouts/CSS3, RSS, canvas/WebGL, 
Ajax/Comet/WebSockets, security issues (XSS, SQL injection, CSRF), 
highload, SWIG

33. **GUI design**, Raskin, usability, design and typography basics, 
Fitts's law, layout principles, LaTeX.
