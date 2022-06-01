# thesis
Python code which automates the process of simulating orbits and collecting the data from them.

# collect_data

collect_data.py is used to collect data by simulating random orbits. The data is then saved to "data.csv".

## Usage

The collect_data.py module is meant to be used by calling its main function.

```
main creates samples of random initial conditions, simulates the
corresponding orbits, and collects data from them. This data is then saved to "data.csv".

It has the following parameters:

num_samples: number of samples to generate. Must be an integer. The default is 500.

#### Simulation Parameters
num_years: number of years to simulate. The default is 100.0.
num_steps: number of steps to simulate. Must be an integer. The default is 10**6.

It is recommended that the ratio of num_steps to num_years
remains close to the ratio of default values.

#### System Parameters
star_mass: mass of the star in kg. The default is the mass of the Sun.

planet_mass: mass of the planet in kg. The default is the mass of the Earth.

The constants sun_mass and earth_mass may be imported from the file constants.py.

planet_distance: distance from the star to the planet in AU. The default is 1.0.


filename: name of the file to save the data to. The default is "data.csv".

Note that a large fraction of orbits are rejected because they get too close to the planet.
This means that the number of samples recorded will be less than num_samples.

This function will take 3 minutes when called with default arguments

The time taken is linear in both num_steps and num_samples.
```
