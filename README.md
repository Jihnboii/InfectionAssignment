# Epidemic Simulation
This project contains Java classes for simulating the spread of an epidemic within a population using a grid-based model. It includes two main classes: Individual and InfectionAssignment.

## Individual Class
Description
- The Individual class represents an individual within the simulated population. It encapsulates attributes such as status (susceptible, infected, or recovered) and probabilities of infection and recovery.

Attributes
- status: Current status of the individual ('S' for susceptible, 'I' for infected, 'R' for recovered).
- infectProb: Probability of an individual getting infected based on their interactions with infected neighbors.
- recoveryProb: Probability of an infected individual recovering in a given time step.

Constructors and Methods
- Constructors to initialize an individual with default or specific attributes.
- Accessor and mutator methods for status, infection probability, and recovery probability.
  
Usage
```Java
// Creating an individual with default attributes
Individual person = new Individual();

// Creating an individual with specified attributes
Individual infectedPerson = new Individual('I', 0.6, 0.3);

// Accessing and modifying attributes
person.setStatus('R');
double infectionProbability = person.getInfect();
```

## InfectionAssignment Class
Description
- The InfectionAssignment class executes the epidemic simulation using the grid-based model. It simulates the spread of a disease among individuals over multiple time steps.

Methods
- Functions for initializing the grid, setting up simulation parameters, and running the simulation.
- Methods for generating biased random numbers, calculating infection rates, and handling grid population.
  
Usage
```Java
// Initializing simulation parameters and running the simulation
int individuals = 25;
int timeSteps = 10;
double infectionRate = 0.3;
double recoveryRate = 0.1;
```

# Running the Simulation
To run the simulation, execute the main() method in the InfectionAssignment class. Follow the instructions provided in the console to input parameters like the number of individuals, time steps, infection rate, and recovery rate.
