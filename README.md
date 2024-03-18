## Qiskit Runtime Lab

## TODO: Update/delete links
## TODO: do we want to keep the IBMQ platform bits? or do we want to just showcase qiskit as a python package
## TODO: we probably want to dress up the theme a little bit more through the jupyter notebooks

### Introducing this hands-on lab

This hands-on lab is a gentle introduction to quantum computing with Qiskit. This lab leverages some the latest innovations from IBM Quantum, such as Qiskit Runtime, and will help you get up to speed on the following topics and skills:

- Creating quantum circuits using Qiskit 
- Executing quantum circuits by using Qiskit Runtime
- Leveraging Qiskit Runtime Sampler and Estimator primitives, and Runtime sessions
- Executing circuits in quantum simulators as well as on IBM Quantum computers

### Creating and running quantum circuits using Python, Qiskit libraries, and Qiskit Runtime

From the File Browser pane on the left side of the IBM Quantum Lab, navigate to the **tutorials** folder and double-click on the **how-to-getting-started-with-sampler.ipynb** file. A Jupyter notebook entitled **Get started with the Sampler primitive** should appear. Go ahead and learn from that tutorial by running each notebook cell using the triangular run icon ▷ at the top of the notebook.

### Developing a program that leverages Qiskit, Qiskit Runtime and the Sampler primitive
## TODO: Update

***Subtitle: “Life is like a box of chocolates”***

Now it time to get your hands dirty with Python and Qiskit code. Your assignment, should you choose to accept it, will be to develop a program that samples one piece from a box that contains two chocolate candies. The circuit that chooses the piece of candy will be the singlet Bell state that you created earlier in this lab. 

*Note: If you want more than two pieces of candy in the box, create a* [*W-state*](https://en.wikipedia.org/wiki/W_state) *that contains one qubit for each piece of chocolate from which it may choose one piece.*

## TODO: we probably need more info on W states here

To get started on this assignment, perform the following steps:

1. Navigate to the **Lab files** folder and create a new folder (using the New Folder icon) named **qiskit-runtime-lab**
2. Create a Jupyter notebook in that folder by clicking the **New file +** button and selecting **Python 3 (ipykernel)** from the **Notebook** section of the **Launcher** pane.
3. In the Quantum Lab file browser, right-click on the **Untitled.ipynb** file and **Rename** it to something like **sampler-lab-exercise.ipynb**
4. Leverage the **Using Qiskit Runtime Sampler** section of the **how-to-getting-started-with-sampler.ipynb** notebook as a guide for coding this assignment. Adding a histogram visualization of the quasi-distribution would be a nice touch, so here's a code snippet you could add to the **4. Invoke the Sampler and get results section** if you'd like:

`from qiskit.visualization import plot_histogram`
`plot_histogram(job.result().quasi_dists[0].binary_probabilities())`


## TODO: keeping or deleting paragraph bellow?
Good luck, and please ask for help at any time! When you've finished this exercise, compare it to the [class solution](https://github.com/JavaFXpert/qiskit-runtime-lab/blob/main/sampler_lab_exercise_solution.ipynb), realizing that it is one of many possible solutions. Here is the [W state version of the class solution](https://github.com/JavaFXpert/qiskit-runtime-lab/blob/main/sampler_lab_exercise_w_state.ipynb).

### Leveraging the Qiskit Runtime Session and the Estimator Primitive

From the File Browser pane on the left side of the IBM Quantum Lab, navigate to the **tutorials** folder and double-click on the **how-to-getting-started-with-estimator.ipynb** file. A Jupyter notebook entitled **Get started with the Estimator primitive** should appear. Go ahead and learn from that tutorial by running each notebook cell using the triangular run icon ▷ at the top of the notebook. When you're ready, we'll look at an example program that leverages Session and Estimator to optimize a box of chocolates.

### Examining a program that leverages Qiskit Runtime Session and the Estimator primitive

***Subtitle: “You never know what you're gonna get”***

Continuing with our box of chocolates theme, please examine [a simple program](https://github.com/JavaFXpert/qiskit-runtime-lab/blob/main/estimator_lab_exercise_solution.ipynb) that leverages Qiskit Runtime and the Variational Quantum Eigensolver (VQE) to assemble a box of chocolates that hopefully meets our expectations. 

This program draws upon code from an example that experimental physicist & IBM Quantum researcher Nick Bronn created for the [Coding with Qiskit Runtime video series](https://www.youtube.com/playlist?list=PLOFEBzvs-VvqAC8DnVoLOzg2bKE4C7ARM), specifically in [Episode 05 Primitives & Sessions](https://youtu.be/yxuH8eb4MS4?si=e3trSORNjooWlQXu).



### Thanks for playing along!
