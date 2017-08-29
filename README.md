# Data-Science-Stuff-Useful-Links

Deep Learning Courses (2017):

* Natural Language Processing with Deep Learning (https://www.youtube.com/watch?v=OQQ-W_63UgQ&list=PL3FW7Lu3i5Jsnh1rnUwq_TcylNr7EkRe6)
* Tensorflow and deep learning - without a PhD by Martin Görner
* CS231n Winter 2016 https://www.youtube.com/watch?v=NfnWJUyUJYU&list=PLkt2uSq6rBVctENoVBg1TpCC7OQi31AlC
* CS205A Numerical Analysis (with Justin Solomon) MIT
https://www.youtube.com/watch?v=dkT8yuI2d50&list=PLHrg69yaUAPeiLEsa-1KauSe2HaA0Wf6I
* Alex Smola (Oxford):
.....
.....
* David Rosenberg (DS GA 1003)
https://davidrosenberg.github.io/ml2017
* Nano De Freitas https://www.cs.ox.ac.uk/people/nando.defreitas/
* machine learning UG course: https://www.youtube.com/playlist?list=PLE6Wd9FR--Ecf_5nCbnSQMHqORpiChfJf
* Deep Learning https://www.youtube.com/playlist?list=PLE6Wd9FR--EfW8dtjAuPoTuPcqmOV53Fu

## Algorithms:
* 6.854/18.415 Advanced Algorithms by Ankur Moitra (http://people.csail.mit.edu/moitra/854.html) Youtube Playlist (https://www.youtube.com/playlist?list=PL6ogFv-ieghdoGKGg2Bik3Gl1glBTEu8c)


## Basics
* MIT - Probability 110 Joe Blitztein (https://projects.iq.harvard.edu/stat110/home)

* Gilbert Strang (http://www-math.mit.edu/~gs/)
His Student: 

## Data Science Stuff General Lectures and Conferences:
* Open Data Science Iniative https://www.youtube.com/user/ProfNeilLawrence/videos

## Interview Prep Material

https://www.analyticsvidhya.com/blog/2016/09/40-interview-questions-asked-at-startups-in-machine-learning-data-science/

Very Nice Ebook stuff:
http://ebook-dl.com/computers-technology/page/8



Difference between variable_scope and name_scope in TensorFlow
https://stackoverflow.com/questions/34215746/difference-between-variable-scope-and-name-scope-in-tensorflow


LSTM, good blogs:
http://colah.github.io/posts/2015-08-Understanding-LSTMs/ -- Jump to this part: Step-by-Step LSTM Walk Through


An all-in-one Docker image for deep learning. Contains all the popular DL frameworks (TensorFlow, Theano, Torch, Caffe, etc.) 
https://github.com/floydhub/dl-docker

Remove Docker Image:
docker rmi <Image ID>

remove docker container:
docker rm <container_name>

All containers must be stopped before being removed:

to shutdown gracefully: docker stop <container_name>
to kill a ruuning cont: docker kill <container_name>

List all containers, running and stopped:
docker ps -a

you can remove a single image with:

docker rmi the_image

However, if you need to remove multiple you could use:
Remove all images

docker rmi $(docker images -qf "dangling=true")

Kill containers and remove them:
docker rm $(docker kill $(docker ps -aq))

Note: Replace kill with stop for graceful shutdown
Remove all images except "my-image"

You could use grep to remove all except my-image and ubuntu
docker rmi $(docker images | grep -v 'ubuntu\|my-image' | awk {'print $3'})

Or (without awk)
docker rmi $(docker images --quiet | grep -v $(docker images --quiet ubuntu:my-image))


# Computer Science Course List of Top ranked Universities, useful to find new free online material from classroom lectures
1. Georgia Tech: http://www.omscs.gatech.edu/current-courses
  1. Course on ML for Trading, FREE: It has three courses:
    1. http://quantsoftware.gatech.edu/Machine_Learning_for_Trading_Course
    1. http://quantsoftware.gatech.edu/Learning_Algorithms_for_Trading
    1. http://quantsoftware.gatech.edu/Computational_Investing
    1. http://quantsoftware.gatech.edu/Manipulating_Financial_Data_in_Python
    

## Concepts and misclleneous:
* Machine learning tips and tricks: 
http://web.archive.org/web/20161017074325/http://blog.david-andrzejewski.com/machine-learning/practical-machine-learning-tricks-from-the-kdd-2011-best-industry-paper/
* Gaussian processes tutorial: http://katbailey.github.io/post/gaussian-processes-for-dummies/


Articles to be read:
http://blog.david-andrzejewski.com/machine-learning/practical-machine-learning-tricks-from-the-kdd-2011-best-industry-paper/

Dockers, Linux, General Stuff:

https://linuxconfig.org/docker-container-backup-and-recovery
