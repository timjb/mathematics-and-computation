---
id: 1883
title: 'A Brown-Palsberg self-interpreter for Gödel&#8217;s System T'
date: 2016-01-04T10:40:16+02:00
author: Andrej Bauer
layout: post
guid: http://math.andrej.com/?p=1883
permalink: /2016/01/04/a-brown-palsberg-self-interpreter-for-godels-system-t/
categories:
  - Computation
  - Publications
---
In a paper accepted at [POPL 2016](http://conf.researchr.org/home/POPL-2016) Matt Brown and [Jens Palsberg](http://web.cs.ucla.edu/~palsberg/) constructed a self-interpreter for System $F_\omega$, a strongly normalizing typed $\lambda$-calculus. This came as a bit of a surprise as it is &#8220;common knowledge&#8221; that total programming languages do not have self-interpreters.

Thinking about what they did I realized that their conditions allow a self-interpreter for practically any total language expressive enough to encode numbers and pairs. In [the PDF note accompanying this post](http://math.andrej.com/wp-content/uploads/2016/01/self-interpreter-for-T.pdf) I give such a self-interpreter for Gödel&#8217;s System T, the weakest such calculus. It is clear from the construction that I abused the definition given by Brown and Palsberg. Their self-interpreter has good structural properties which mine obviously lacks. So what we really need is a better definition of self-interpreters, one that captures the desired structural properties. Frank Pfenning and Peter Lee [called such properties **reflexivity**](http://repository.cmu.edu/cgi/viewcontent.cgi?article=2969&context=compsci), but only at an informal level. Can someone suggest a good definition?

**Note:** [self-interpreter-for-T.pdf](http://math.andrej.com/wp-content/uploads/2016/01/self-interpreter-for-T.pdf)