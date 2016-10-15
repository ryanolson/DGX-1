

## FAQ

- Why is cuDNN not installed in the provided CUDA container?

  cuDNN is a rapidly evolving library to provide the best performance for deep learning frameworks and applications.   As such, the API and ABI have been changing on approximately a 6 month cadence.   Not all DL frameworks can make use of the latest version of cuDNN.   Therefore, we feel it’s best for a user building a custom application from the base CUDA container to install cuDNN separately.

  Here are some examples of extending the CUDA container for [cuDNN 5.1](https://github.com/ryanolson/DGX-1/blob/master/dockerfiles/cudnn/5.1/Dockerfile).
