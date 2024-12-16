This is a class project turned algorithm I wrote that I had done realted to parallel programming(vanilla piece of code turned to this), due to the need of making another project. I realized the need of kmeans for data visualization for my webapp. which runs a connection to EC2 instance.
Due to EC2's limits, it ain't no quatum computer, I use this piece of code in C to aid my python flask server that serves over websocket to achieve acceptable performance for data visualization for my web app.

Pthread multi-threaded, efficient Kmeans with Kmeans++ initializations as well as elbow method to determine the best k possible all in one piece of code. that can be ran on linux as a single executable

to compile: gcc -lrt kmeansv1.c -o kmeans -lm -lpthread
no warnings

Highlghts: 1.initKMeans++ O(nlogn) implementation where normal rand kmeans is not scientific and applicable due to some undefined behavior by rand() (its always predefined interms of predicability and undefined in terms of the effect you wan to achieve)
              |
              |
              v
              with this we dont need n^2 imeplementation and can make it as efficient as possible
          2.Pure hand written imeplementation of the vannilla version of kmeans WITH pthread(which took me hours to finish and days to debug)

          3.cpu multithreaded for aided speed

          4. In pure C to provide speed.

          5.Self adjusted K for optimal results as well as combined k elbow implementations and theoretical best wcss with limits MAX limit to K
          ![image](https://github.com/user-attachments/assets/44094f31-36c8-4999-a32b-94e9d6d76aab)
