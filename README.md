```
  _____                    _                           _
 |  __ \                  | |                         (_)
 | |  | | ___  ___ _ __   | |     ___  __ _ _ __ _ __  _ _ __   __ _
 | |  | |/ _ \/ _ \ '_ \  | |    / _ \/ _` | '__| '_ \| | '_ \ / _` |
 | |__| |  __/  __/ |_) | | |___|  __/ (_| | |  | | | | | | | | (_| |
 |_____/ \___|\___| .__/  |______\___|\__,_|_|  |_| |_|_|_| |_|\__, |
                  | |                                           __/ |
                  |_|                                          |___/
```


## What is include
- Python 3.6
- NumPy
- Pandas
- SciPy
- Scikit-learn
- Matplotlib
- Seaborn
- XGBoost
- TensorFlow
- Keras
- PyTorch
- Torch Vision
- MXNet
- Jupyter Notebook

To work with this personal branch, You just first need to clone the Repo. 
```sh

~$ git clone -b personal https://github.com/this-is-r-gaurav/docker-python-deep-learning.git
~$ cd docker-python-deep-learning
~/docker-python-deep-learning$
```

## Building the Image
Replace Image_name name with name of your choice(No space allowed) : 
```sh
~/docker-python-deep-learning$docker build -t Image_name
```

## Running the container
**host_path**: Replace the host_path with the path you want to mount volume in if you want to to mount volume in home directory within a pynb directory then host_path with ~/pynb

**Image_name**: Replace Image_name with the name you give it while building the Image

```sh
docker run -it --name deep-learning \
           -v host_path:/home/notebooks \
           -p 8888:8888 -d \
           Image_name
```
