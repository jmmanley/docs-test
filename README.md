An example of how to use readthedocs with sphinx-multiproject!
No guarantee this is optimal, this was just my playground to get things working.

## package1
[![Documentation Status](https://readthedocs.org/projects/testingoutthedpocs/badge/?version=latest)](https://docs-test-project2.readthedocs.io/projects/package1/en/latest/?badge=latest)

## package2

[![Documentation Status](https://readthedocs.org/projects/docs-test-project2/badge/?version=latest)](https://docs-test-project2.readthedocs.io/en/latest/?badge=latest)

Note: you need a separate readthedocs project for each package.
Ensure that you specify the `PROJECT` [environmental variable](https://docs.readthedocs.io/en/stable/reference/environment-variables.html) with the name of the desired package to build.
If desired, you can add one project as a [subproject](https://docs.readthedocs.io/en/stable/subprojects.html) of another.
For example, I set `project1` as a subproject of `project2`.
Therefore, `project1` is available at both [`testingoutthedpocs.readthedocs.io`](https://testingoutthedpocs.readthedocs.io) and [`docs-test-project2.readthedocs.io/projects/package1/`](https://docs-test-project2.readthedocs.io/projects/package1/).
