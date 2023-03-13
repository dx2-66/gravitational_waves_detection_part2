# Kaggle Class II Gravitational Wave Detection 

This is a sequel to G2Net, focusing on weak continuous gravitational waves, mostly attributed to rapidly spinning neutron stars. The task is very challenging since the single observation can last for months, the signal is buried deeply in the noise, and the data entries are **huge**: the *test* set takes around 200GB and  you're supposed to generate the synthetic train data on your own.

My solution wasn't overly successful (worth noting top solution was algorithmic) - around the middle of the leaderboard, I triedto focus on keeping it simple:
- spectrograms are simply averaged by time periods to dig out the signal;
- 3 networks were pretrained on my own synthetic data;
- the results were blended together with simple logistic regression using the small original sample train set.

**Required units:**

- pandas
- scikit-learn
- PyTorch
- skorch
- timm
- numpy
- h5py
- Matplotlib
- Seaborn
