# "Don’t just sit idly by, watching as robotic overlords take over the world. Create your own army of sentient machines and beat them at their own game! And keep being awesome, cloud gurus!"

https://github.com/ACloudGuru-Resources/Course_AWS_Certified_Machine_Learning

https://github.com/ACloudGuru-Resources/Course_AWS_Certified_Machine_Learning/blob/master/Chapter7/ufo-algorithms-lab.ipynb

Interesting process for shuffling a dataset:

np.random.seed(0)
rand_split = np.random.rand(len(df))
train_list = rand_split < 0.8
val_list = (rand_split >= 0.8) & (rand_split < 0.9)
test_list = rand_split >= 0.9

 # This dataset will be used to train the model.
data_train = df[train_list]

# This dataset will be used to validate the model.
data_val = df[val_list]

# This dataset will be used to test the model.
data_test = df[test_list]
