# Python-package
Project Description
Gaussian and Binomial Distributions

This package provides functionality for basic mathematical operations on Gaussian and Binomial distributions. Operations include calculating the mean and standard deviation for both sample and population data, as well as plotting histograms for Gaussian distributions and frequency bar charts for Binomial distributions.

Dummy Input Data
For testing the Gaussian distribution module, use the following dummy input data:

1, 3, 99, 100, 120, 32, 330, 23, 76, 44, 31

For the Binomial distribution module, here's some dummy data representing the outcomes of 13 trials: 0 denotes failure, and 1 denotes success:

0, 1, 1, 1, 1, 1, 0, 1, 0, 1, 0, 1, 0

Testing the Code
To test the Gaussian distribution module, use the following code snippet:

python
Copy code
from dg_probability import Gaussian

gaussian = Gaussian(10, 5)
print(f"Gaussian mean = {gaussian.mean}")
print(f"Gaussian standard deviation = {gaussian.stdev}")
For the Binomial module, use this snippet:

python
Copy code
from dg_probability import Binomial

binomial = Binomial(0.25, 60)
print(f"Binomial mean = {binomial.mean}")
print(f"Binomial standard deviation = {binomial.stdev}")
Testing the Entire Binomial Distribution Module
To test the entire Binomial distribution module, follow these steps:

Create a file named data_binomial.txt and add the dummy data for the Binomial distribution to it.
Save the file in the same directory as your code.
Use the following code:
python
Copy code
from dg_probability import Binomial

binomial = Binomial()
binomial.read_data_file('data_binomial.txt')
binomial.calculate_mean()
binomial.calculate_stdev()
binomial.replace_stats_with_data()
binomial.plot_bar()
binomial.plot_bar_pdf()
Contributions
Contributions to this project are welcome. Please feel free to create pull requests (PRs) for any improvements or enhancements.

Source Code
You can find the source code for this project on GitHub:
GitHub - dg1223/object-oriented-programming
