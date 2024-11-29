# What this is

I wanted to use the data I collected with my [Environmental Data Collection System](https://github.com/MoodyMarshmallow/Environmental-Data-Collection-System) to train a machine-learning model to predict soil moisture values in high temporal resolution.

# What the code does

![image](flowchart-of-code.png)
<br/><br/>
**1. Pre-Processing** – First, I had to merge the various output files I had extracted into one output file (this included decoding one incorrectly formatted output file). Then I did all the usual pre-processing steps of removing anomalous datapoints and interpolating the small gaps that this created, extracting more features for ML, synchronise datapoints so that each the modalities were logged at the same time, and normalise the data to make the learning porcess easier.

**2. Verification** – I wanted to run a few tests before conducting the actual machine learning porcess to evaluate the suitability of the data for machine learning, so I made some quantile-quantile graphs to
