(Note that all functions and files should stay in same folder.)
To reproduce the results, type following commands in Matlab 7.0:


% load arrow heads
load arrowHeads.mat;
% (or data = load('arrowHeads.txt'); )

% euclidean distance test on arrow heads
% num_of_runs is the number of random runs
% in our VLDB paper we ran 50 times
avgPerformanceTest(data, num_of_runs);
% results (best_so_far_dist, best_so_far_index, and cost of each approach)
% of each run are recorded in query1.mat, query2.mat, ...
% note that in the paper we show the average performance over 50 runs

% DTW distance test on arrow head (similiar as above)
DTW_avgPerformanceTest(data, num_of_test);
% results of each run are recorded in dtw_try1.mat, dtw_try2.mat, ...

% load heterogenous data
load heterogenous.mat
% the resulting variable is CombineTS
% (or load('heterogenous.txt'); )
% use the same commands above for euclidean and DTW tests


