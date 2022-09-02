# SLOPE-Solver--Newt_ALM
This Matlab package solves the SLOPE model:

      min { 0.5*||Ax - b||^2 + kappa_lambda (x) }

from the dual pespective: 

     - min {0.5*||xi||^2 + b'*xi + kappa^*_lambda (u): A'*xi + u = 0}

where kappa_lambda(x)=lambda'*sort(abs(x),'descend')  
and kappa^*_lambda is the conjugate function, [m,n]=size(A) with m<n


It was created based on the algorithm proposed by 

"Ziyan Luo, Defeng Sun, Kim-Chuan Toh and Naihua Xiu, Solving the OSCAR and SLOPE models using a semismooth Newton-based augmented Lagrangian method, Journal of Machine Learning Research, 20 (106) (2019) 1-25".

Please give credits to this paper if you use the code for your research.
