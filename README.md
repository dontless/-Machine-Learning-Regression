# -Machine-Learning-Regression


Installing the recommended software tools

If you choose to use the recommended tools, you have two options: downloading and installing the required software or 
using a prepackaged version on a free instance on Amazon EC2.

Option 1: Downloading and installing all software on your own machine

         Download and install Python, IPython Notebook, Numpy, SFrame and GraphLab Create. You can find the instructions here.

Option 2: Using a free Amazon EC2 with all the software pre-installed

            If you do not have a 64-bit computer, you will not be able to run GraphLab Create. Additionally, 
           some of you may want a simple experience where you don't have to download the course content and 
           install everything locally. Here, we'll address these situations!

          Amazon EC2 offers free cloud computing hours with what they call micro instances.
          These instances are all we need to do the work for this course. We have created an image for one such
          instance that is easy to launch and contains all the course content. This will allow you to run everything 
          you need for this course in the cloud for free, without having to install anything locally.
          (You do need to create an Amazon EC2 account and have internet access.)

You can find step-by-step instructions here:

              https://turi.com/download/install-graphlab-create-aws-coursera.html

We note that installing all the software on your own local machine may be the right option for most people; 
especially since you can run locally everything without needing to be online to do the homeworks. But, the option 
using Amazon EC2 should be a great alternative.
Github repository with starter code
In each module of the course, we have a reading with the assignments for that module as well as some starter code.
For those interested, the starter code and demos used in this course are also available in a public Github repository:

          https://github.com/learnml/machine-learning-specialization

Using other software packages

We strongly encourage you to use the recommended software packages for this course, since they will allow you to learn
the fundamental concepts more quickly. However, you are welcome to use others. Here are a few notes if you do so.

Installing other software tools

In the instructions above, you will be using the Graphlab Launcher, which will automatically install Python,
IPython Notebook, Numpy, Matplotlib, SFrame and GraphLab Create. If you don’t use the Graphlab Launcher, you will 
need to install each of these tools separately, by following the pages linked above. Anaconda is a good tool to help
simplify some of this installation.

If you are using SFrame, but not GraphLab Create
GraphLab Create uses SFrame under the hood, but you can use just SFrame for most assignments. If you choose to do so, 
in the starter code for the assignments, you should change the line

                        
                        import graphlab
                        
                          import sframe            
     and everything should work with just some small modifications, e.g., the calls:
                       graphlab.SFrame(...)
                       
If you are using other software tools out there
You are welcome to use other packages, e.g., scikit-learn instead of GraphLab Create, or Pandas instead of SFrame,
or even R instead of Python. If you choose to use all these different packages, we will provide the datasets
(in standard CSV format) and the assignment questions will not depend specifically on the recommended tools.


#Regression - A Machine Learning Approach.

This course focuses regression, one of the most important types of data analysis,
with a wide range of applications. After successfully completing this course, you will be able to use regression methods in
practice, implement some of the most fundamental algorithms in this area, and choose the right model for your task. 
In addition, you will become proficient in core ML concepts that transcend regression settings: you will understand the 
practical implications of fundamental ML concepts, such as the bias-variance tradeoff, key ML data analysis techniques, 
such as cross validation, and the most important optimization techniques used to learn ML models, gradient descent and 
coordinate descent.


# Useful software tools

Although you will be implementing algorithms from scratch in various assignments, some software tools will be useful in the process. In particular, there are four types of data tools that would be helpful:

# Data manipulation: 
to help you slice-and-dice the data, create new features, and clean the data.
Matrix operations: in the inner loops of your algorithms, you will do various matrix operations, and libraries focus on these will speed-up your code significantly.
Plotting library: so you can visualize data and models.
Pre-implemented ML algorithms: in some assignments where we are focusing on fundamental ML concepts, such as cross-validation or the bias-variance tradeoff, you will use a pre-implemented ML algorithms to help focus your efforts on the fundamentals.



# Tools for data manipulation:-
For data manipulation, we recommend using SFrame, an open-source, highly-scalable Python library for data manipulation. 
An alternative is the Pandas library. A huge advantage of SFrame over Pandas is that with SFrame, you are not limited to
datasets that fit in memory, which allows you to deal with large datasets, even on a laptop.
(The SFrame API is very similar to Pandas' API. Here is a doc showing the relationship between the two of them.)

# Tools for matrix operation:-
For matrix operations, we strongly recommend Numpy, an open-source Python library that provides fast performance, 
for data that fits in memory.

# Tools for plotting:-
For plotting, we strongly recommend you use Matplotlib, an open-source Python library with extensive plotting functionality.

# Tools with pre-implemented ML algorithms:-
For the few assignments where you will be using pre-implemented ML algorithms, we recommend you use GraphLab Create,
which we used in the first course, a package we have been working on for many years now, and has seen an exciting 
adoption curve, especially in industry with folks building real applications. A popular alternative is to use 
scikit-learn. GraphLab Create is more scalable than scikit-learn and simpler to use when your data is not numeric vectors.
On the other hand, scikit-learn is open-source.

In this course, most of the assignments are about implementing algorithms from scratch, so this choice is more flexible 
than in the first course. We are happy, however, for you to use any tool(s) of your liking. As you will notice,
we are only grading the output of your programs, so the specific software tool is not the focus of the course. 
More details on using other tools are at the end of this doc.

It's important to emphasize that this specialization is not about providing training for a specific software package. 
The goal of the specialization is for your effort to be spent on learning the fundamental concepts and algorithms 
behind machine learning in a hands-on fashion. These concepts transcend any single package. What you learn here you 
can use whether you write code from scratch, use any existing ML packages out there, or any that may be developed 
in the future. We are happy to hear that so many of you are enjoying this approach so far!

                          
                          
                          
                          
              
