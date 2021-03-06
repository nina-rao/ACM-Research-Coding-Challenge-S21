# ACM Research Coding Challenge (Spring 2021)

## No Collaboration Policy

**You may not collaborate with anyone on this challenge.** You _are_ allowed to use Internet documentation. If you _do_ use existing code (either from Github, Stack Overflow, or other sources), **please cite your sources in the README**.

## Submission Procedure

Please follow the below instructions on how to submit your answers.

1. Create a **public** fork of this repo and name it `ACM-Research-Coding-Challenge-S21`. To fork this repo, click the button on the top right and click the "Fork" button.
2. Clone the fork of the repo to your computer using `git clone [the URL of your clone]`. You may need to install Git for this (Google it).
3. Complete the Challenge based on the instructions below.
4. Submit your solution by filling out this [form](https://acmutd.typeform.com/to/uqAJNXUe).

## Question One

Genome analysis is the identification of genomic features such as gene expression or DNA sequences in an individual's genetic makeup. A genbank file (.gb) format contains information about an individual's DNA sequence. The following dataset in `Genome.gb` contains a complete genome sequence of Tomato Curly Stunt Virus. 

**With this file, create a circular genome map and output it as a JPG/PNG/JPEG format.** We're not looking for any complex maps, just be sure to highlight the features and their labels.

**You may use any programming language you feel most comfortable. We recommend Python because it is the easiest to implement. You're allowed to use any library you want to implement this**, just document which ones you used in this README file. Try to complete this as soon as possible.

Regardless if you can or cannot answer the question, provide a short explanation of how you got your solution or how you think it can be solved in your README.md file. However, we highly recommend giving the challenge a try, you just might learn something new!


## Solution
When I first read the coding challenge, I thought that I have no idea what to do, much less how to implement it. But I felt motivated to give the challenge my best attempt.
I started my solution by first doing some extensive research on circular genome maps and the type of data it represents. After learning the context, I went back and studied the 'Genome.gb' file and saw that there were specifications about the start and end parameters of certain genes of the virus. I considered coding the map from scratch, but I realized that would be a hefty task, so I sought out some existing software. Then I found an open source software called Circos which visualizes data in a circular layout. In order to install Circos, I had to learn a lot of things I had never encountered before. I had to install Strawberry Perl for Windows since the software was built in Perl, then I used the Command Terminal and Ubuntu Bash to open the Circos modules and download them. Then I opened the Circos folder in Visual Studio and entered the data about the genes found on the Tomato Curly Stunt Virus Genome file. Then I realized that since the starts and ends of genes overlap, and the full genome is not accounted for, that I was losing some information. Thus I was only able to create a crude genome map. How I would solve this problem if I had more coding background and time to learn the software would be to plot a circle divided into 2766 units to represent the nucleotides. And then I would plot the gene ranges as nodes inside of that circle, in a smaller circle. Then I would take the difference between two overlapping genes and have blocks within that circle to represent the overlapping of genes. 
