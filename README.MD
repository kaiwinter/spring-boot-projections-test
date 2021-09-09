# Spring Boot Projections Test

## Requirements
1. Java 8

## Nice to have
1. Lombok plugin

## Starting the project
Using gradle wrapper:

- `gradlew clean build bootRun`

## Running the experiment:
1. Initialize database data by calling: localhost:8080/sample/init
2. Test the projections by calling: localhost:8080/sample/test

The test may take around 1 minute to complete with the default settings (also depends on your machine).

To change the settings, navigate to SampleController and update `ITERATIONS` and `OBJECTS_PER_ITERATION` variables.

## Results (on my machine)
### Spring Boot 2.1.0
Entity projections took 198.17 ms on average out of 100 iterations.  
Constructor projections took 26.99 ms on average out of 100 iterations.  
Interface projections took 226.94 ms on average out of 100 iterations.  
Tuple projections took 24.13 ms on average out of 100 iterations.  
Dynamic projections took 27.27 ms on average out of 100 iterations.

### Spring Boot 2.2.0
Entity projections took 465.27 ms on average out of 100 iterations.  
Constructor projections took 61.92 ms on average out of 100 iterations.  
Interface projections took 476.02 ms on average out of 100 iterations.  
Tuple projections took 53.97 ms on average out of 100 iterations.  
Dynamic projections took 59.15 ms on average out of 100 iterations.

### Spring Boot 2.3.0
Entity projections took 504.13 ms on average out of 100 iterations.  
Constructor projections took 53.57 ms on average out of 100 iterations.  
Interface projections took 478.11 ms on average out of 100 iterations.  
Tuple projections took 48.7 ms on average out of 100 iterations.  
Dynamic projections took 52.96 ms on average out of 100 iterations.

### Spring Boot 2.4.4
Entity projections took 491.42 ms on average out of 100 iterations.  
Constructor projections took 56.88 ms on average out of 100 iterations.  
Interface projections took 392.39 ms on average out of 100 iterations.  
Tuple projections took 49.63 ms on average out of 100 iterations.  
Dynamic projections took 55.59 ms on average out of 100 iterations.

### Spring Boot 2.5.0
Entity projections took 464.76 ms on average out of 100 iterations.  
Constructor projections took 53.32 ms on average out of 100 iterations.  
Interface projections took 403.91 ms on average out of 100 iterations.  
Tuple projections took 46.12 ms on average out of 100 iterations.  
Dynamic projections took 51.72 ms on average out of 100 iterations.

### Spring Boot 2.5.3
Entity projections took 465.8 ms on average out of 100 iterations.  
Constructor projections took 57.03 ms on average out of 100 iterations.  
Interface projections took 407.38 ms on average out of 100 iterations.  
Tuple projections took 49.52 ms on average out of 100 iterations.  
Dynamic projections took 56.03 ms on average out of 100 iterations.
