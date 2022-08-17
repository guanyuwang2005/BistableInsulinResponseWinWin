# BistableInsulinResponseWinWin

This is a MPI parallel computation application written in c++
It contains the source codes of [1].

(1) The file Basic.cpp is a single-node program for the basic simulation of the glucose dynamics model (Eq. (3) of the paper).
It does not need parallel compuation.

(2) The file Opt.cpp is a multiple-nodes program (the user can choose the number of nodes used) to optimize the parameters of the mathematical model.

(3) The subfolders are specific to individual groups of [2]. NOB_Normal, OB_Normal, NOB_DB, OB_DB correspond to IGT-OB-, IGT-OB+, IGT+OB-, and IGT+OB+ of [1], respectively. They also correspond to groups 1, 2, 3, and 4 of [1], respectively.

In each subfolder, the .txt files contain the experimental data and the results of computation; the PSB files instruct the file opt.cpp to employ a certain amount of computer nodes to do the computation. For example, OptQM1200 means that the optimization was completed by using 1200 nodes in the HPC cluster QM; OptTY1200 means that the optimization was completed by using 1200 nodes in the HPC cluster TY.


References:

[1] Bistable insulin response: the win-win solution for glycemic control, submitted

[2] Mitrakou, A. et al. Role of reduced suppression of glucose production and diminished early insulin release in
impaired glucose tolerance. New Eng J Med 326, 22–29 (1992).
