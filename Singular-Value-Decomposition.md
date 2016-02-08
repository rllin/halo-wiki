[Singular Value Decomposition](https://en.wikipedia.org/wiki/Singular_value_decomposition)

"If m is much larger than n then it is advantageous to first reduce the matrix M to a triangular matrix with the QR decomposition and then use Householder reflections to further reduce the matrix to bidiagonal form; the combined cost is 2mn2 + 2n3 flops (Trefethen & Bau III 1997, Lecture 31)." [Wikipedia, Calculating the SVD](https://en.wikipedia.org/wiki/Singular_value_decomposition#Calculating_the_SVD)

**Thin SVD**
Only the n column vectors of U corresponding to the row vectors of V* are calculated. The remaining column vectors of U are not calculated. This is significantly quicker and more economical than the full SVD if n≪m. The matrix Un is thus m×n, Σn is n×n diagonal, and V is n×n. [Wikipedia, Thin SVDs](https://en.wikipedia.org/wiki/Singular_value_decomposition#Reduced_SVDs)

**Sign Ambiguity / Indeterminacy**
"Though SVD and EVD are well-established...there is an intrinsic sign indeterminacy that can significantly impact conclusions...we provide a solution to the sign ambiguity problem..."
[Resolving the Sign Ambiguity in the Singular Value Decomposition, pg.3](http://prod.sandia.gov/techlib/access-control.cgi/2007/076422.pdf)

**Comparing Components**
* I think that the magnitude of the eigenvalue is proportional to the amount of variation along the axis (but not sure about this) - [[Patrick Wolber]]

## Names, Acronyms, Misnomers
* SVD, svd, S.V.D