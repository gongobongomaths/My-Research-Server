#### Tutor: Atrajit Sarkar
#### Date: 28th March,2025

## Question:
Let
\[
  f(x,y) = \begin{cases} 
    \frac{xy}{x^2+y^2}, & \text{if } x^2+y^2 \neq 0 \\ 
    0, & \text{if } x^2+y^2 = 0 
  \end{cases}
\]
 1. Find directonal derivative at $(0,0)$ at the direction $\beta = (l\hat{i}+m\hat{j})$ [where $l^2+m^2=1$].
 2. Find $f_x(0,0)$ $\&$ $f_y(0,0)$.


 ## Answer:
 1. To find the \textbf{directional derivative} of the function  

\[
  f(x,y) = 
  \begin{cases} 
    \frac{xy}{x^2+y^2}, & \text{if } x^2+y^2 \neq 0 \\ 
    0, & \text{if } x^2+y^2 = 0 
  \end{cases}
\]

at the point $(0,0)$ in the direction $\beta = (l,m)$ with $l^2 + m^2 = 1$, we use the definition:

\[
D_{\beta} f(0,0) = \lim_{h \to 0} \frac{f((0,0) + h\beta) - f(0,0)}{h}
\]

#### Step 1: Expressing the Increment
Since $h\beta = (hl, hm)$, we evaluate the function at this point:

\[
f(hl, hm) = \frac{(hl)(hm)}{(hl)^2 + (hm)^2}
\]

Since $l^2 + m^2 = 1$, we simplify:

\[
f(hl, hm) = \frac{h^2 lm}{h^2(l^2 + m^2)} = \frac{h^2 lm}{h^2} = lm
\]

Since $f(0,0) = 0$, the directional derivative simplifies to:

\[
D_{\beta} f(0,0) = \lim_{h \to 0} \frac{lm}{h}
\]

#### Step 2: Evaluating the Limit

The expression $\frac{lm}{h}$ does \textbf{not} tend to a finite limit as $h \to 0$; rather, it diverges to \textbf{infinity} unless $lm = 0$.

\section*{Conclusion}
- If $lm \neq 0$, the directional derivative \textbf{does not exist} (since the limit does not converge).
- If $lm = 0$, then $D_{\beta} f(0,0) = 0$.

Thus, the **directional derivative at (0,0) exists only if either $l = 0$ or $m = 0$, in which case it is 0**. Otherwise, it **does not exist**.


2. To find the partial derivatives $f_x(0,0)$ and $f_y(0,0)$, we use the definitions:

\[
f_x(0,0) = \lim_{h \to 0} \frac{f(h,0) - f(0,0)}{h}, \quad
f_y(0,0) = \lim_{h \to 0} \frac{f(0,h) - f(0,0)}{h}
\]

#### Finding $f_x(0,0)$:

Substituting $y = 0$ in $f(x,y)$:

\[
f(h,0) = \frac{h(0)}{h^2 + 0^2} = 0
\]

Since $f(0,0) = 0$, we get:

\[
f_x(0,0) = \lim_{h \to 0} \frac{0 - 0}{h} = 0
\]

#### Finding $f_y(0,0)$

Substituting $x = 0$ in $f(x,y)$:

\[
f(0,h) = \frac{0(h)}{0^2 + h^2} = 0
\]

Since $f(0,0) = 0$, we get:

\[
f_y(0,0) = \lim_{h \to 0} \frac{0 - 0}{h} = 0
\]

#### Conclusion

\[
f_x(0,0) = 0, \quad f_y(0,0) = 0
\]


### Notice: 
In the part 1 we dicussed that directional derivative exists iff $lm =0$ that is, either $l=0$ or $m=0$. And $l=0$ means $\beta =(0,m)=m(0,1)$ and $l^2+m^2=1 \implies m^2=1 \implies m=\pm 1,$ but $m=1$ is fine as we are taking $h \to 0+$ and $h \to 0-$, so $\beta =(0,1)$ or in the direction of $y$ axis that is $f_y(0,0)$ and $m=0 \implies \beta=(1,0)$ similarly. And discussed in part 1 we are going to get the directional derivative zero and yes we get that exactly in part 2. So, we can directly calculate part 2 from part 1. No need to calculate again seperately. 