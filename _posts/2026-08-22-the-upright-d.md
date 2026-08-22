---
layout: post
title: "The upright d for derivative"
date: 2026-08-22
categories: [mathematics]
---

Few years ago when I was still quite young in research, I didn't pay much attention on the mathematical conventions when writing proofs. After all, symbols serve as _symbols_- a representation of _something_- and as long we define the _terms_ and the _operators_ used, it should be fine. 

But, I realized, I don't really have to define them all the time. 

Like how the term `d` in derivative; it is well understood to be an operator for _differentiation_. 

Then, I notice something. 

## Part 1: The 'd' in derivative
Upon reading various mathematics inputs throughout my research journey, I can't help but to notice one subtle change in the writing of the _"derivative of"_ across some maths papers;

$$ \frac{\mathrm{d}y}{\mathrm{d}t} \hspace{5mm} \text{and} \hspace{5mm} \frac{dy}{dt}.$$

**The observation**: _The symbol d is slanted in the second part (old), whereas the symbol d is upright in the first one (new)_.

### The Latex Code
> to write the `d` first part, write down in latex with mathrm concatenated to it: `\mathrm{d}`. For example, the `dy/dt` can be written as below in LaTeX
```latex
\frac{\mathrm{d}y}{\mathrm{d}t} 
```
> which gives:
> $$ \frac{\mathrm{d}y}{\mathrm{d}t}.  $$

## Part 2: The First Notice
It is not _obvious_ at first. The first realization is when I played the [**TeXnique**](https://texnique.xyz). 

![TexNique](images/TexNique.png)

Briefly, TeXnique is a LaTeX Typsetting game where you have to write the LaTeX code from given equation. After you coded the given equation correctly, new equation will appear. The equations ranges from easy to hard, and the scores depends on the difficulty of the equations; if the equationis lengthy and complex, high score is given, and vice versa. 

I was thrilled when I first met the game. So, I tried, and after few equations, I stucked at writing below equation (or as I remembered):
 
 $$ \frac{\mathrm{d}x}{\mathrm{d}t} = x.$$

I was quite confused that my provided code is incorrect (mine gave _slanted_ `d` instead of upright). After a google search, I realized that the `d` 'has' to be upright. Then, I wondered.

> Does everyone (paticularly, LaTex-users mathematician) coded the `d` like this? Is it common?

Another observation is made when I watched Grant Senderson when he explained the process behind his animation in one Youtube [video](https://www.youtube.com/watch?v=rbu7Zu5X1zI&t=1995s) (minute 45:22). The defined Lorenz equation there used the operator `\mathrm{d}` for upright `d`.
 
## Part 3: Is it neccesary to upright-ed the d?

Stumbled upon that, I started to go through a number of papers to see if the `d` in the equation is upright; mostly I looked up some Ordinary Differential Equations (ODE) papers to see the 'derivative' symbol in their defined models. Old papers using the convention of the slanted one, but the new papers start to apply the upright `d`. 

Is it necessary?

Perhaps, just to stadardize in defining an _operator_ (so that, `d` is not a variable). So, making the symbol `d` upright is necessary.

## Part 4: Closing remark

Overall, standardizing is a good practice, even it is miniscule; to be slanted or to be upright-ed. It will be helpful for the reader to digest it, without wondering if the `d` is an operator or variable (although, personally, _d_ is well known to represent 'derivative'. But, for the sake of standardization, I agree with the convention).

Lowkey, writing the `\mathrm{d}` is rather lengthy. Some user consider applying the command 

```latex
\newcommand{\dd}{\mathop{}\!\mathrm{d}} 
```
in LaTex file, so that instead of writing `\mathrm{d}`, user can type `\dd` for upright `d` for derivative. For me, the `\mathrm{d}` slowly becomes a part of my muscle memory whenever I write an upright `d`.  

p.s: Different fields have different 'attitude' on the necessity of an upright 'd'. Anyway, whatever works, works. Aye, cheers~

