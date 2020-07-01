********
Log-PDFs
********

.. currentmodule:: pints

:class:`LogPDFs<pints.LogPDF>` are callable objects that represent
distributions, including likelihoods and Bayesian priors and posteriors.
They are unnormalised, i.e. their area does not necessarily sum up to 1, and
for efficiency reasons we always work with the logarithm e.g. a log-likelihood
instead of a likelihood.

Example::

    p = pints.GaussianLogPrior(mean=0, variance=1)
    x = p(0.1)

Overview:

- :class:`LogPDF`
- :class:`LogPrior`
- :class:`LogPosterior`
- :class:`ProblemLogLikelihood`
- :class:`SumOfIndependentLogPDFs`
- :class:`HierarchicalLogPosterior`


.. autoclass:: LogPDF

.. autoclass:: LogPrior

.. autoclass:: LogPosterior

.. autoclass:: ProblemLogLikelihood

.. autoclass:: SumOfIndependentLogPDFs

.. autoclass:: HierarchicalLogPosterior

