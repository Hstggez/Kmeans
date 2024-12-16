This is a class project turned algorithm I wrote that I had done realted to parallel programming(vanilla piece of code turned to this), due to the need of making another project. I realized the need of kmeans for data visualization for my webapp. which runs a connection to EC2 instance.
Due to EC2's limits, it ain't no quatum computer, I use this piece of code in C to aid my python flask server that serves over websocket to achieve acceptable performance for data visualization for my web app.

Pthread multi-threaded, efficient Kmeans with Kmeans++ initializations as well as elbow method to determine the best k possible all in one piece of code. that can be ran on linux as a single executable

to compile: gcc -lrt kmeansv1.c -o kmeans -lm -lpthread
no warnings
