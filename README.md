# kmc3-docker
Docker image for kmc3

Docker image containing a running version of kmc v3

The image contains a full install of [kmc](http://sun.aei.polsl.pl/REFRESH/index.php?page=projects&project=kmc&subpage=about), including all necessary dependencies. I am not part of the kmc team - I just made this image.

In detail, the image is set up with:
 - Ubuntu 18.04
 - kmc v3.0

To run [kmc](http://sun.aei.polsl.pl/REFRESH/index.php?page=projects&project=kmc&subpage=about) you can do the following (this will mount the directory `/home/working` of the container to the current working directory on your local machine):
```bash
$ docker run -it --rm -v $(pwd):/home/working -w /home/working chrishah/kmc3-docker kmc
$ docker run -it --rm -v $(pwd):/home/working -w /home/working chrishah/kmc3-docker kmc_tools
```

