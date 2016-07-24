# multiESS
Compute multivariate effective sample size (*mESS*) of Markov chain, using the multivariate dependence structure of the process.

This is a MATLAB implementation of the *mESS* estimation method described in Vats et al. (2015), with some minor tweaks for the choice of batch size *b* for the computation of the Monte Carlo covariance matrix. Digit `help multiESS` to display the documentation.

See also the R package [mcmcse](https://cran.r-project.org/web/packages/mcmcse/index.html) for a separate implementation.

*Disclaimer:* This is a working version in need of some additional testing. The interface may change in the future.

### Details

The effective sample size of a Markov chain is the size of an i.i.d. sample with the same covariance structure as the current chain.
*mESS* is given by *mESS* = *n* |Λ|^{1/*p*}/ |Σ|^{1/*p*}, where *n* is the current sample size, Λ is the sample covariance matrix, *p* is the number of parameters and Σ is an estimate of the Monte Carlo covariance matrix for the Markov chain (here obtained by batch estimation).

### Reference

Vats, D., Flegal, J. M., & Jones, G. L. "Multivariate Output Analysis for Markov chain Monte Carlo", arXiv preprint arXiv:1512.07713 (2015). ([link](http://arxiv.org/abs/1512.07713))

### License

This is free, open source software released under the GPL-3 License. See LICENSE.txt for details.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

Use this software at your own risk.
