This file shows you how to run the simulations in "Housing First or Treatment First", by Shahar Rotberg.

Before running each simulation you will have to run the following commands:

Write the command in the line below and press enter:
gfortran housing_first_or_treatment_first_SR_v1.f90 -I/usr/local/include -lm -mcmodel=medium -fopenmp -g -o housing_first_or_treatment_first

Write the command in the line below and press enter:
./housing+_first_or_treatment_first

At the very top of the Fortran code there is a module titled "Global_Vars". At the top of this module you will see six variables, which we describe below how to set for each simulation.

For generating the benchmark, please set:

		is_counterfactual=0
        partial_equilibrium=0
        probability_of_voucher_benchmark_used=0.054
        increased_prob_of_voucher_if_homeless_and_addicted=1
        how_many_iterations_to_do_on_distribution=0
		compare_to_original_benchmark=1

Experiments 1, 2, 3, and 4

1. For Experiment 1, please set:
	
	a. GE (LR)

		is_counterfactual=1
        partial_equilibrium=0
        probability_of_voucher_benchmark_used=0.054
        increased_prob_of_voucher_if_homeless_and_addicted=0
        how_many_iterations_to_do_on_distribution=0
		compare_to_original_benchmark=1

	b. PE (1)

		is_counterfactual=1
        partial_equilibrium=1
        probability_of_voucher_benchmark_used=0.054
        increased_prob_of_voucher_if_homeless_and_addicted=0
        how_many_iterations_to_do_on_distribution=1
		compare_to_original_benchmark=1

	c. PE (5)

		is_counterfactual=1
        partial_equilibrium=1
        probability_of_voucher_benchmark_used=0.054
        increased_prob_of_voucher_if_homeless_and_addicted=0
        how_many_iterations_to_do_on_distribution=5
		compare_to_original_benchmark=1

	d. PE (LR)

		is_counterfactual=1
        partial_equilibrium=1
        probability_of_voucher_benchmark_used=0.054
        increased_prob_of_voucher_if_homeless_and_addicted=0
        how_many_iterations_to_do_on_distribution=100
		compare_to_original_benchmark=1


2. Experiment 2:

		is_counterfactual=1
        partial_equilibrium=0
        probability_of_voucher_benchmark_used=1
        increased_prob_of_voucher_if_homeless_and_addicted=1
        how_many_iterations_to_do_on_distribution=0
		compare_to_original_benchmark=1


3. Experiment 3:
	
	a. GE (LR)

		is_counterfactual=1
        partial_equilibrium=0
        probability_of_voucher_benchmark_used=1
        increased_prob_of_voucher_if_homeless_and_addicted=0
        how_many_iterations_to_do_on_distribution=0
		compare_to_original_benchmark=0

	b. PE (1)

	is_counterfactual=1
        partial_equilibrium=1
        probability_of_voucher_benchmark_used=1
        increased_prob_of_voucher_if_homeless_and_addicted=0
        how_many_iterations_to_do_on_distribution=1
	compare_to_original_benchmark=0

	c. PE (5)

		is_counterfactual=1
        partial_equilibrium=1
        probability_of_voucher_benchmark_used=1
        increased_prob_of_voucher_if_homeless_and_addicted=0
        how_many_iterations_to_do_on_distribution=5
		compare_to_original_benchmark=0

	d. PE (LR)

		is_counterfactual=1
        partial_equilibrium=1
        probability_of_voucher_benchmark_used=1
        increased_prob_of_voucher_if_homeless_and_addicted=0
        how_many_iterations_to_do_on_distribution=100
		compare_to_original_benchmark=0
	

4. Experiment 4:

	a. GE (LR)

		is_counterfactual=1
        partial_equilibrium=0
        probability_of_voucher_benchmark_used=1
        increased_prob_of_voucher_if_homeless_and_addicted=0
        how_many_iterations_to_do_on_distribution=0
		compare_to_original_benchmark=1	

	b. PE (1)

		is_counterfactual=1
        partial_equilibrium=1
        probability_of_voucher_benchmark_used=1
        increased_prob_of_voucher_if_homeless_and_addicted=0
        how_many_iterations_to_do_on_distribution=1
		compare_to_original_benchmark=1

	c. PE (5)

		is_counterfactual=1
        partial_equilibrium=1
        probability_of_voucher_benchmark_used=1
        increased_prob_of_voucher_if_homeless_and_addicted=0
        how_many_iterations_to_do_on_distribution=5
		compare_to_original_benchmark=1

	d. PE (LR)

		is_counterfactual=1
        partial_equilibrium=1
        probability_of_voucher_benchmark_used=1
        increased_prob_of_voucher_if_homeless_and_addicted=0
        how_many_iterations_to_do_on_distribution=100
		compare_to_original_benchmark=1


	


	
