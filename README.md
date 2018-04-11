# kdd99ml
Demo of SciKit ML algorithms using the kdd99 dataset

Based on Charanpal Dhanjal work https://gist.github.com/charanpald/c216800e25480ee838e8

To download dataset:
1) Create directory named "datasets" (you may change the 'data_dir' variable)
   Enter the directory
2) Download KDD Cup 99 dataset with:
   wget http://kdd.ics.uci.edu/databases/kddcup99/kddcup.data.gz
   or
   wget http://kdd.ics.uci.edu/databases/kddcup99/kddcup.data_10_percent.gz

   and uncompress it. The first one occupies about 740MBytes, the second one
   around 71MBytes. Should you use the smaller dataset, please adjust filename
   in code:
   raw_data_filename = data_dir + "kddcup.data"
   change by
   raw_data_filename = data_dir + "kddcup.data_10_percent"
3) run the code with
   python detectAttack.py
4) play with other classifiers, commenting RandomForest creation line
   (around line 45) and uncomment DecisionTreeClassifier.
