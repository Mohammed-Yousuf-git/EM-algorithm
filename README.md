# EM-algorithm
“An implementation of the Expectation-Maximization algorithm for Gaussian Mixture Models with synthetic data and parameter estimation.”
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

</head>
<body>
    <h1>EM Algorithm for Gaussian Mixture Models</h1>

   <p>
        This repository contains an implementation of the Expectation-Maximization (EM) algorithm for fitting 
        a Gaussian Mixture Model (GMM) to a dataset. The code demonstrates the iterative approach to estimate 
        the parameters of Gaussian components (means, variances, and weights) using synthetic data.
    </p>

  <h2>Features</h2>
    <ul>
        <li>Initialization of Gaussian parameters (means, variances, and weights).</li>
        <li>Implementation of the E-step to compute responsibilities.</li>
        <li>Implementation of the M-step to update model parameters.</li>
        <li>Convergence based on the log-likelihood function.</li>
    </ul>
    <h2>Requirements</h2>
    <p>Ensure you have the following Python libraries installed:</p>
    <ul>
        <li>numpy</li>
        <li>scipy</li>
    </ul>
    <h2>Setup</h2>
    <pre>
    git clone https://github.com/your-username/em-algorithm-gmm.git
    cd em-algorithm-gmm
    </pre>
    <h2>Usage</h2>
    <ol>
        <li>Run the Python script to fit a Gaussian Mixture Model to the synthetic dataset:</li>
    </ol>
    <pre>
    python em_algorithm.py
    </pre>
    <ol start="2">
        <li>Modify the script to use your own dataset by replacing the <code>data</code> variable with your custom data.</li>
    </ol>
    <h2>Algorithm Details</h2>
    <p>
        The EM algorithm iteratively estimates the parameters of the Gaussian components by alternating between 
        two steps:
    </p>
    <ul>
        <li><strong>E-step:</strong> Calculates the responsibilities (probabilities) of each data point belonging to each component.</li>
        <li><strong>M-step:</strong> Updates the parameters (means, variances, and weights) using the responsibilities calculated in the E-step.</li>
    </ul>
    <p>
        The process continues until the log-likelihood of the data converges or a maximum number of iterations is reached.
    </p>
    <h2>Output</h2>
    <p>The script prints the final parameters of the Gaussian components:</p>
    <ul>
        <li><strong>Means:</strong> The center of each Gaussian component.</li>
        <li><strong>Variances:</strong> The spread of each Gaussian component.</li>
        <li><strong>Weights:</strong> The proportion of data points belonging to each component.</li>
    </ul>
    <h2>Example Output</h2>
    <pre>
    Converged at iteration 10.
    Final means: [0.01, 5.03]
    Final variances: [1.01, 0.98]
    Final weights: [0.50, 0.50]
    </pre>
<section>
  <h3>Acknowledgement</h3>
  <p>I would like to extend my deepest gratitude to Dr. Victor A.I, professor at Maharaja Institute of Technology Mysore,for his invaluable guidance throughout this project</p>
  
</section>
  
</body>
</html>
