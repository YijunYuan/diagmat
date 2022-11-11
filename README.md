# diagmat
A latex package to generate (anti)-diagonal matrices easily. Based on [Enrico Gregorio](https://tex.stackexchange.com/users/4427/egreg)'s [answer](https://tex.stackexchange.com/a/539741/107173) on tex.stackexchange.com
## Example
```tex
\documentclass{article}
\usepackage{diagmat}
\begin{document}
$\diagmat{1,2,3,4}$
$\diagmat[fences=b]{1,2,3,4}$
$\diagmat[mask=0]{1,2,3,4}$
$\diagmat[fences=v,mask=\cdot]{1,2,3,4}$

$\antidiagmat{1,2,3,4}$
$\antidiagmat[fences=b]{1,2,3,4}$
$\antidiagmat[mask=0]{1,2,3,4}$
$\antidiagmat[fences=v,mask=\cdot]{1,2,3,4}$
\end{document}
```
### Effect
![image](https://user-images.githubusercontent.com/7012463/201358557-678a6824-74c9-4dae-8a9a-81be0c26fd1d.png)

## Options
* `fences`: accept one of the following value: `p`,`b`,`v`,`B`, which corresponds to `pmatrix`,`bmatrix`,`vmatrix`,`Bmatrix` in `amsmath`. Default: `p`.
* `mask`: entries which are not on the (anti)-diagonal line. Default: empty.

## Credits
All credits are [Enrico Gregorio](https://tex.stackexchange.com/users/4427/egreg)'s. All bugs are mine.
