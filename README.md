# Timetable Generator Using Genetic Algorithm

## Overview
This project implements a **University Exam Timetable Generator** using a **Genetic Algorithm (GA)**. The system automates the scheduling process while ensuring compliance with constraints and optimizing satisfaction criteria, such as minimizing conflicts and balancing resource allocation.

---

## Features
- **Automated Exam Scheduling**: Generates optimized exam timetables.
- **Constraint Handling**:
  - **Hard Constraints**: Enforces critical rules, such as no overlapping exams for invigilators.
  - **Soft Constraints**: Strives for preferences like minimizing back-to-back exams for students.
- **Genetic Algorithm**:
  - **Population Initialization**: Creates diverse schedules.
  - **Fitness Function**: Evaluates solutions based on constraint adherence.
  - **Selection, Crossover, and Mutation**: Enhances and evolves schedules.

---

## Technology Stack
- **Programming Language**: Python
- **Core Libraries**:
  - `numpy` for numerical operations.
  - `random` for stochastic processes.
  - `matplotlib` for visualizations (if needed).

---

## Installation
### Prerequisites
1. Install Python (>= 3.8).
2. Ensure the following libraries are installed:
   ```bash
   pip install numpy
   pip install matplotlib
   ```

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/fardeenfarhat/timeTable_Gen.git
   ```
2. Navigate to the project directory:
   ```bash
   cd timeTable_Gen
   ```
3. Enjoy the code

---

## Usage
1. **Input Dataset**: Provide a dataset containing courses, teachers, classrooms, and time slots.
2. **Run Algorithm**: Execute the Genetic Algorithm to generate a timetable.
3. **Outputs**:
   - Optimized timetable as a text file or visual chart.
   - Fitness scores for each generation.

---

## Genetic Algorithm Workflow
1. **Initialization**:
   - Create a population of chromosomes, each representing a potential timetable.
   - Each chromosome consists of genes specifying:
     - Course Code
     - Time Slot
     - Classroom
     - Invigilating Teacher
2. **Fitness Evaluation**:
   - Assign scores based on constraint adherence.
   - Lower scores indicate better schedules.
3. **Selection**:
   - Use **Roulette Wheel Selection** to choose parent chromosomes.
4. **Crossover**:
   - Apply **Uniform Crossover** to generate offspring.
5. **Mutation**:
   - Introduce random changes to genes to explore new solutions.
6. **Iteration**:
   - Repeat steps 2-5 until the termination condition is met (e.g., max generations or optimal solution).

---

## Outputs
- **Generated Timetable**:
  - A conflict-free schedule meeting hard constraints.
  - Optimized for soft constraints.
- **Fitness Progression**:
  - Graph showing fitness scores over generations.

---

## Example
### Input Dataset
| Course Code | Teacher ID | Classroom | Time Slot |
|-------------|------------|-----------|-----------|
| CS101       | T01        | C01       | 9:00 AM   |
| MA102       | T02        | C02       | 11:00 AM  |

### Output Timetable
| Course Code | Teacher ID | Classroom | Time Slot |
|-------------|------------|-----------|-----------|
| CS101       | T01        | C01       | 9:00 AM   |
| MA102       | T02        | C02       | 11:00 AM  |

---

## Future Enhancements
- Support for multi-campus scheduling.
- Integration with student management systems.
- Interactive UI for input and output visualization.

---

## Contributing
1. Fork the repository.
2. Create a new branch for your feature or bugfix:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add feature-name"
   ```
4. Push to the branch:
   ```bash
   git push origin feature-name
   ```
5. Submit a pull request.

---

## License
This project is licensed under the [MIT License](LICENSE).

---

## Contact
- **Author**: Fardeen Farhat
- **Email**: fardeenfarhat@gmail.com
- **GitHub**: [fardeenfarhat](https://github.com/fardeenfarhat)
